# Estratégia "Tio Larry" do Lorenz

Em 0407/2021 o Fabrício Lorenz do canal "No Pain, No Gain" apresentou um vídeo (juntamente com sua esposa) entitulado ["Dinheiro e CONSISTÊNCIA - Como atingir"](!https://youtu.be/QrxUReBhjko), mostrando uma estratégia extremamente simples que, se seguida fielmente, forneces excelentes retornos financeiros no médio a longo prazo.

Codificação da estratégia de execução, seleção e coloração
chamada "Tio Larry" (aqui chamada de "Uncle Larry") apresentada
pelo Lorenz neste vídeo: https://youtu.be/QrxUReBhjko
 
Acrescentei uma FLAG (Faz_DayTrade) para aqueles que querem
fazer Day Trade, ou seja, entrar e sair do trade no mesmo dia
caso as condições de compra e venda sejam atingidas no mesmo
dia. Esta flag não faz sentido na seleção, e precisa ser alterada
diretamente no código caso queira que ela seja refletida no gráfico
se for aplicada como estratégia de execução.

Acrescentei também os parâmetros de quantidade de negócios
e volume financeiro para eliminar papéis com menor liquidez

OBS.: o setup não foi apresentado com STOP, de tal forma que
às vezes há um drawdown violento (experimente fazer o backtest
passando pelo período do início da pandemia - 03/2020 - por exemplo)
