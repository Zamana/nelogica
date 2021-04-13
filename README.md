# Nelogica
Estratégias de execução, coloração e seleção para o Profit da Nelógica

Este repositório tem por objetivo armazenar códigos de execução, coloração e seleção para o produto Profit da Nelógica.

Ao contrário do MetaTrader, por exemplo, que possui recursos nativos para execução de robôs através da linguagem MQL, o Profit da Nelógica possui apenas recursos para codificação de estratégias de execução, coloração e seleção, através de uma linguagem à qual eu desconheço o nome, mas que, sintaticamente, possui muita semelhança com Pascal.

Estas estratégias no Profit, ao contrário de um robô, não efetuam os trades automaticamente, mas apenas:

1) indicam no gráfico os pontos nos quais as compras e vendas devem ser executadas (no caso de estratégias de execução) ou,
2) indicam os candles que satisfazem as condições definidas (para o caso das estratégias de coloração) ou,
3) indicam as ações que satisfazem os critérios definidos (para o caso das estratégias de seleção).

OBSERVAÇÃO: nenhuma estratégia aqui apresentada deve ser usada como "setup" para trade. Todo e qualquer risco ou perda envolvido no uso destes códigos é de inteira responsabilidade de quem decidiu utilizá-los.
