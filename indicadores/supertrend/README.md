# SuperTrend

O indicador SuperTrend, conforme consta em se próprio nome, é um indicador da categoria de tendência, e foi criado por (Olivier Seban)[!https://www.olivier-seban.com/].

É um indicador simples de usar (mas não tão simples de calcular...). Ele não prevê a tendência do mercado, mas a mostra claramente uma vez que tenha sido estabelecida. Por isso mesmo e também como qualquer outro indicador de tendência, fornece sinais falsos quando o ativo está lateralizado, e portanto sem tendência.

Particularmente acredito que não possa ser usado isoladamente como um sinal de compra e venda, mas sempre acompanhando de algum outro indicador de outra categoria para filtrar ou confirmar o sinal.

# Parâmetros

## Período e "Multiplicador"

Classicamente o indicador é usado com os parâmetros de 10 períodos e um "multiplicador" (que na verdade é o desvio-padrão da média utilizada) de 3.

Como o indicador é fortemente baseado e influenciado pela média to True Range (o Average True Range, ou ATR), o tipo de média utilizado acaba tendo impacto também. Por esta razão, acrescentei mais um parâmetro para que o tipo de média possa ser escolhido.

## Tipo de Média
Tradicionalmente é utilizada a média de (Welles Wilder)_[!https://en.wikipedia.org/wiki/J._Welles_Wilder_Jr.]_, o próprio criador de vários indicadores, entre eles o ATR, mas resolvi deixar a possibilidade de se utilizar outras médias, como Aritmética Simples e Exponencial.

## Tipo de Linha
Este parâmetro é mais um solução de contorno do que um parâmetro em si. Explicando melhor...

No Profit, da Nelogica, é possível, ao invocar certos indicadores, como o StopATR ou o HiLoActivator, passar um sufixo "|1|" para se indicar que se está interessado apenas em saber se o indicador está abaixo ou acima dos preços. Exemplo:

### StopAtr
![image](https://user-images.githubusercontent.com/6900313/141683999-4e4fc293-e4f8-4256-ae29-f4daab378db4.png)

### HiLoActivator
![image](https://user-images.githubusercontent.com/6900313/141684061-268559eb-ff8d-401a-9cf5-06c107a480bf.png)

Infelizmente, porém, este recuro, que auxilia bastante na codificação de estratégias de execução, seleção e coloração, não é fornecido na linguagem de programação disponível para os usuários. Diante desta limitação acrescentei então este parâmetro para que se possa escolher se o indicador deve plotar os valores no gráfico de preços:

![image](https://user-images.githubusercontent.com/6900313/141684220-4b9ef85a-b752-4fbb-b1d2-4ccf5f7cd281.png)

Ou apenas retornar "0" ou "1" para indicar se a tendência é de alta ou baixa.

Resumindo, esses são os parâmetros do indicador:

![image](https://user-images.githubusercontent.com/6900313/141684273-eada88df-9a9c-4e36-b73b-0a9c59764b00.png)

1) Período (default: 10)
2) Desvio (ou multiplicador; default: 3)
3) Tipo (de média; default: 2, ou "Welles Wilder")
4) Linha (default: 0, ou plotagem no gráfico de preços. Utilize 1 para uso em estratégias)

