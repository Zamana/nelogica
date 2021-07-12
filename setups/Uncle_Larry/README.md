# Estratégia "Tio Larry" do Lorenz

Em 04/07/2021 o Fabrício Lorenz em seu canal "No Pain, No Gain" apresentou um vídeo (juntamente com sua esposa) entitulado ["Dinheiro e CONSISTÊNCIA - Como atingir"](https://youtu.be/QrxUReBhjko), mostrando uma estratégia extremamente simples que, se seguida fielmente, fornece excelentes retornos financeiros no médio a longo prazos.

Resolvi codificar a estratégia (veja os arquivos LORENZ_UNCLE_LARRY.src para o fonte e LORENZ_UNCLE_LARRY.psf para importação no Profit) e fiquei impressionado, tanto com a taxa de acerto como também com o *payoff*.

## Adaptações 
Tomei a liberdade de acrescentar 2 ajustes para deixar a estratégia mais flexível:

## 1) Day Trade
Acrescentei uma *flag* (Faz_DayTrade) para aqueles que querem fazer **Day Trade**, ou seja, entrar e sair do trade no mesmo dia caso as condições de compra e venda sejam atingidas no mesmo dia. Esta *flag* não tem efeito na seleção, e precisa ser alterada diretamente no código caso queira que ela seja refletida no gráfico se for aplicada como estratégia de execução.

## 2) Número de negócios e Volume financeiro
Acrescentei também os parâmetros de quantidade de negócios e volume financeiro para eliminar papéis com menor liquidez 

# ALERTA
> O *setup* não foi apresentado com **STOP**, de tal forma que às vezes há um *drawdown* violento (experimente, por exemplo, fazer o *backtest* passando pelo período do início da > pandemia - 03/2020).

Mantive a estratégia assim mas posso adaptá-la para contemplar um **STOP** caso haja interesse.
