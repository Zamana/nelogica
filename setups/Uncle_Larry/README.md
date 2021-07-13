# Estratégia "Tio Larry" do Lorenz

Em 04/07/2021 o Fabrício Lorenz em seu canal "No Pain, No Gain" apresentou um vídeo (juntamente com sua esposa) intitulado ["Dinheiro e CONSISTÊNCIA - Como atingir"](https://youtu.be/QrxUReBhjko), mostrando uma estratégia extremamente simples que, se seguida fielmente, fornece excelentes retornos financeiros no médio a longo prazos.

Resolvi codificar a estratégia (veja os arquivos LORENZ_UNCLE_LARRY.src para o fonte e LORENZ_UNCLE_LARRY.psf para importação no Profit) e fiquei impressionado, tanto com a taxa de acerto como também com o *payoff*.

Esse, definitivamente, não é um *setup* "ganhar de balde e perder de colherinha"; está mais para o "de grão em grão a galinha enche o papo".

## Adaptações 
Tomei a liberdade de acrescentar 2 ajustes para deixar a estratégia mais flexível:

## 1) Day Trade
Acrescentei uma *flag* (Faz_DayTrade) para aqueles que querem fazer **Day Trade**, ou seja, entrar e sair do trade no mesmo dia caso as condições de compra e venda sejam atingidas no mesmo dia. Esta *flag* não tem efeito na seleção, e precisa ser alterada diretamente no código caso queira que ela seja refletida no gráfico se for aplicada como estratégia de execução.

## 2) Número de negócios e Volume financeiro
Acrescentei também os parâmetros de quantidade de negócios e volume financeiro para eliminar papéis com menor liquidez 

# ALERTA
> O *setup* não foi apresentado com **STOP**, de tal forma que às vezes há um *drawdown* violento (experimente, por exemplo, fazer o *backtest* passando pelo período do início da > pandemia - 03/2020).

Mantive a estratégia assim mas posso adaptá-la para contemplar um **STOP** caso haja interesse.

# *Backtests*

Aplicando a estratégia como filtro de seleção após o pregão do dia 12/07 com os requisitos *default* (número de negócios acima de 500 e volume financeiro acima de 1 milhão de reais), obtive a seguinte seleção de ativos no período diário:

![image](https://user-images.githubusercontent.com/6900313/125369282-52beee00-e352-11eb-9d37-f620354aea1b.png)

Fazendo o *backtest* no período exato dos últimos 12 meses (de 11/07/2020 a 11/07/2021) obtive esses resultados para as primeiras ações (ordenadas em ordem decrescente de rentabilidade nos últimos 3 meses) para uma quantidade fixa de 500 ações:

## PTBL3

### Resumo
![image](https://user-images.githubusercontent.com/6900313/125369551-d7117100-e352-11eb-88c1-fecd2b6f91c6.png)

### Lista de operações
![image](https://user-images.githubusercontent.com/6900313/125369602-edb7c800-e352-11eb-8f42-4984d9d2778b.png)

### Gráfico de operações
![image](https://user-images.githubusercontent.com/6900313/125369639-0aec9680-e353-11eb-8ff0-5cc4881fefbf.png)

### Curva de capital
![image](https://user-images.githubusercontent.com/6900313/125369682-2061c080-e353-11eb-8004-1841edd89d2b.png)

---

## TOTS3

### Resumo
![image](https://user-images.githubusercontent.com/6900313/125369926-abdb5180-e353-11eb-97c9-444cfcfa8640.png)

### Lista de operações
![image](https://user-images.githubusercontent.com/6900313/125369953-bbf33100-e353-11eb-8928-d1ef56da3b6c.png)

### Gráfico de operações
![image](https://user-images.githubusercontent.com/6900313/125369980-d0cfc480-e353-11eb-8f4e-ae3c8462bfe9.png)

### Curva de capital
![image](https://user-images.githubusercontent.com/6900313/125370010-e349fe00-e353-11eb-8113-a2a57dc0dda9.png)

---

## SQIA3

### Resumo
![image](https://user-images.githubusercontent.com/6900313/125370049-fa88eb80-e353-11eb-8322-941957daad06.png)

### Lista de operações
![image](https://user-images.githubusercontent.com/6900313/125370072-096f9e00-e354-11eb-8adc-567c369ae971.png)

### Gráfico de operações
![image](https://user-images.githubusercontent.com/6900313/125370107-18eee700-e354-11eb-8ee0-09bd0fc00511.png)

### Curva de capital
![image](https://user-images.githubusercontent.com/6900313/125370145-2b692080-e354-11eb-8ee1-83ab380ead13.png)


