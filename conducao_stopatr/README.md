# Condução por STOP ATR

# ATENÇÃO
> Este código não deve ser usado como estratégia pura de compra e venda de ativos.

O objetivo deste código é facilitar a condução de um *trade* pelo método do **STOP ATR**, conforme preconizado pelo Fabrício Lorenz da L&S Educação, mentor da ACADEMIA DO TRADER.

Independentemente do método utilizado para a entrada no *trade*, o restante da condução pode ser verificada com este facilitador.

# IMPORTANTE
> Esta estratégia de execução, coloração e seleção trabalha apenas na modalidade *long* ("ponta da compra").

# IMPORTAÇÃO
Consulte o arquivo [INSTRUCOES.md](https://github.com/Zamana/nelogica/blob/2c2781093988e4eb594d61d0dd43e12ed96fa931/INSTRUCOES.md) na raiz deste projeto para verificar como fazer a importação da estratégia.

# USO
Após ter entrado no *trade* na modalidade *long* ("ponta da compra"), o acompanhamento da evolução do *trade* pode ser feito com esta estratégia de execução vinculada ao gráfico.

Quando for o momento de vender o ativo, aparecerá no gráfico a indicação **"SelltoCover"**, conforme este exemplo:

![image](https://user-images.githubusercontent.com/6900313/114633258-97c17e80-9c96-11eb-984f-1c824a5cf38f.png)

Veja que no círculo VERDE não houve indicação de venda, porque o valor mínimo após a virada do **STOP ATR** (barra AMARELA acima dos *candles*) não foi rompido.

Já no círculo VERMELHO, a mínima foi rompida e a indicação de VENDA foi ativada.

# IMPORTANTE
> Esta estratégia não contempla a realização parcial; ela presta-se apenas a indicar o momento exato no qual um *trade* que está sendo conduzido pelo **STOP ATR** de acordo com o método do Lorenz deve ser vendido.
 
# BÔNUS
Esta estratégia pode ser aplicada na coloração para indicar o *candle* de saída (será colorido de AMARELO por default), e também como estratégia de seleção, que pode ser aplicado sobre o conjunto dos ativos comprados que estão indicando venda.
