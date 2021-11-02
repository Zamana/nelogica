# Estratégia HILO

Esta estratégia usa o indicador HILO originalmente de 6 períodos e no tempo gráfico **SEMANAL** como referências para entrada e saída de trades.

# Critérios

## Critério para compra

Um sinal de entrada na ponta da compra (operação LONG) é gerado quando:

1) O HILO de 6 períodos no gráfico SEMANAL para para BAIXO dos preços;

## Critério para venda

O sinal de saída do trade ocorre quando:

1) O HILO de 6 períodos no gráfico SEMANAL para para CIMA dos preços;


# Backtest

Utilizando o [InvestCharts](https://investcharts.com/), os resultados obtidos foram esses, de acordo com os critérios a seguir:

1) Período: últimos 5 anos (referência: outubro/2021)
2) Capital inicial: R$ 70.000,00
3) Entrada em cada trade: 10% do capital total (reinvestindo os lucros), máximo de 7 trades simultâneos
4) Portfólio: IBXX
5) Tempo gráfico: **SEMANAL**

## Resumo
![image](https://user-images.githubusercontent.com/6900313/139922120-54f927d5-2f0d-414e-8743-a27e2239d58c.png)


## Curva de capital
![image](https://user-images.githubusercontent.com/6900313/139922163-433d4609-7c59-4bc7-b063-14be1393f78a.png)

## Desempenho individual

### Melhores resultados
![image](https://user-images.githubusercontent.com/6900313/139922203-1406b4b8-5e06-451b-95a2-2b3f6615031d.png)


### Piores resultados
![image](https://user-images.githubusercontent.com/6900313/139922228-15d7e5d3-f2f1-45d6-8eb8-8c3d605ddc44.png)

## Backtest individual

### Melhores resultados
![image](https://user-images.githubusercontent.com/6900313/139922269-886cb33e-aba5-48c8-93b4-ae20dfcdd8ae.png)

## Piores resultados
![image](https://user-images.githubusercontent.com/6900313/139922312-f78148fc-94bb-40ff-a303-171d2a662acd.png)

> **OBSERVAÇÃO IMPORTANTE:**
> 
> Lucros passados não são garantia de lucros futuros.
> 
> Faça seus próprios *backtests* e opere na conta simulada antes de investir seu dinheiro real em estratégias automatizadas.
>
> Atente para ações "fora da curva" no período, como MGLU3 e BID4, por exemplo, que distorcem o retorno da estratégia.
> 
