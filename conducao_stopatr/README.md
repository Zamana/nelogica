# Condução por STOP ATR

Este código não deve ser usado como estratégia pura de compra e venda de ativos.

O objetivo deste código é facilitar a condução de um *trade* pelo método do **STOP ATR**, conforme preconizado pelo Fabrício Lorenz da L&S Educação, mentor da ACADEMIA DO TRADER.

Independentemente do método utilizado para a entrada no trade, o restante da condução pode ser verificado com este facilitador.

# IMPORTANTE
> Esta estratégia de execução, coloração e seleção trabalha apenas na modalidade *long* ("ponta da compra").

# IMPORTAÇÃO
Consulte o arquivo INSTRUCOES.md na raiz deste projeto para verificar como fazer a importação da estratégia.

# USO
Após ter entrado no trade na modalidade *long* ("ponta da compra"), o acompanhamento da evolução do *trade* pode ser feito com esta estratégia de execução vinculada ao gráfico.

Quando for o momento de vender o ativo, aparecerá no gráfico a indicação "SelltoCover", conforme este exemplo:
![image](https://user-images.githubusercontent.com/6900313/114630397-df450c00-9c90-11eb-86b6-7a326f387a1f.png)

Veja que no círculo VERDE não houve indicação de venda, porque o valor mínimo após a virada do StopATR (barra AMARELA acima dos *candles*) não foi rompida.

Já no círculo VERMELHO, a mínima foi rompida e a indicação de VENDA foi ativada.

# IMPORTANTE
> Esta estratégia não contempla a realização parcial; ela presta-se apenas a indicar o momento exato no qual um *trade* que está sendo conduzido pelo STOP ATR de acordo com o método do Lorenz deve ser vendido.
