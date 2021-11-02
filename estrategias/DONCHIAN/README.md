# Estratégia DONCHIAN

Esta estratégia usa o indicador DONCHIAN originalmente de períodos 10 para as máximas e 5 para as mínimas, no tempo gráfico **SEMANAL**, como referências para entrada e saída de trades.

> OBSERVAÇÃO:
> 
> Para visualizar corretamente esta estratégia no Profit é necessário usar o indicador ["donchian_correto"](https://github.com/Zamana/nelogica/tree/main/indicadores/donchian).
> 

# Critérios

## Critério para compra

Um sinal de entrada na ponta da compra (operação LONG) é gerado quando:

1) O primeiro candle fechar ACIMA da linha SUPERIOR do Donchian de 10 períodos; a entrada efetivamente será na abertura do candle seguinte.

## Critério para venda

O sinal de saída do trade ocorre quando:

1) O primeiro candle fechar ABAIXO da linha INFERIOR do Donchian de 5 períodos; a saída efetivamente será na abertura do candle seguinte.


# Backtest

Utilizando o [InvestCharts](https://investcharts.com/), os resultados obtidos foram esses, de acordo com os critérios a seguir:

1) Período: últimos 5 anos (referência: outubro/2021)
2) Capital inicial: R$ 70.000,00
3) Entrada em cada trade: 10% do capital total (reinvestindo os lucros), máximo de 7 trades simultâneos
4) Portfólio: IBXX
5) Tempo gráfico: **SEMANAL**

## Resumo
![image](https://user-images.githubusercontent.com/6900313/139925884-fa72e66b-254d-4985-bd58-75b7674db5e1.png)


## Curva de capital
![image](https://user-images.githubusercontent.com/6900313/139925948-ab864a85-98f0-452b-9a75-5e5387ed5271.png)

## Desempenho individual

### Melhores resultados
![image](https://user-images.githubusercontent.com/6900313/139925984-e075a6e4-83a7-4751-b94f-c9a48075825f.png)


### Piores resultados
![image](https://user-images.githubusercontent.com/6900313/139926007-ac58414f-96fc-478b-ad5e-84b5be9fdbc4.png)

## Backtest individual

### Melhores resultados
![image](https://user-images.githubusercontent.com/6900313/139926053-c26e194e-6e3f-4534-8ee2-4814eaafd670.png)

## Piores resultados
![image](https://user-images.githubusercontent.com/6900313/139926086-c5f8c7fc-5273-419a-b50f-16deb0139f98.png)

## Exemplo da estratégia aplicada no Profit
![image](https://user-images.githubusercontent.com/6900313/139926488-2a58c119-76f3-4a57-8eda-13a4f4f8f570.png)


> **OBSERVAÇÕES IMPORTANTES**
> 
> Lucros passados não são garantia de lucros futuros.
> 
> Faça seus próprios *backtests* e opere na conta simulada antes de investir seu dinheiro real em estratégias automatizadas.
>
> Atente para ações "fora da curva" no período, como MGLU3 e BIDI4, por exemplo, que distorcem o retorno da estratégia.
> 
