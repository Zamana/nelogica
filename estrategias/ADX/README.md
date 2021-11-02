# Estratégia ADX

Esta estratégia usa o indicador ADX e as linhas DI+ e DI- como referências para entrada e saída de trades.

# Critérios

## Critério para compra

Um sinal de entrada na ponta da compra (operação LONG) é gerado quando:

1) A linha DI+ cruza e fica ACIMA da linha DI-;
E
3) A linha ADX está ascendente

## Critério para venda

O sinal de saída do trade ocorre quando:

1) A linha DI+ cruza e fica ABAIXO da linha DI-;
OU
2) A linha ADX fica descendente(1)

> (1) este último critério é uma adaptação minha e não consta na estratégia original; pode ser removido, bastando comentar a parte "OR" do código no critério de venda.

# Backtest

Utilizando o [InvestCharts](https://investcharts.com/), os resultados obtidos foram esses, de acordo com os critérios a seguir:

1) Período: últimos 5 anos (referência: outubro/2021)
2) Capital inicial: R$ 70.000,00
3) Entrada em cada trade: 10% do capital total (reinvestindo os lucros), máximo de 7 trades simultâneos
4) Portfólio: IBXX
5) Tempo gráfico: diário

## Resumo
![image](https://user-images.githubusercontent.com/6900313/139920210-54194c44-8fd0-4c43-b1da-40445cfc54b7.png)


## Curva de capital
![image](https://user-images.githubusercontent.com/6900313/139920109-50da5e11-42ab-4e46-8b0c-2a6a9e3ac0cb.png)

## Desempenho individual

### Melhores resultados
![image](https://user-images.githubusercontent.com/6900313/139920378-cfe84680-4b4b-4087-b9bd-7affc870ac94.png)


### Piores resultados
![image](https://user-images.githubusercontent.com/6900313/139920417-55f9d207-0c50-4112-af7f-298fd7f84e31.png)

## Backtest individual

### Melhores resultados
![image](https://user-images.githubusercontent.com/6900313/139920503-919015fa-20c0-483b-b82e-f4a86f660f1d.png)

## Piores resultados
![image](https://user-images.githubusercontent.com/6900313/139920540-3582215d-a8bb-44b0-a657-6f0515c7212d.png)

> **OBSERVAÇÃO IMPORTANTE:**
> 
> Lucros passados não são garantia de lucros futuros.
> 
> Faça seus próprios *backtests* e opere na conta simulada antes de investir seu dinheiro real em estratégias automatizadas.
