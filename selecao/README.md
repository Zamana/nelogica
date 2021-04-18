# Seleção & Coloração de "Barras de Ignição" (A.K.A. "Barras Elefante")

Este código de seleção e coloração identifica de maneira exclusivamente **quantitativa** a ocorrência de barras de ignição, levando em conta apenas:

1) Se o candle atual tem um CORPO maior que os dos últimos candles
2) Se o pavio em cada ponta está dentro de uma porcentagem limite estabelecida (configurável)

Os seguintes parâmetros podem ser configurados:
- Período (para comparação da série de candles)
- Volume Mínimo para entrar na seleção
- Se é ou não para usar o tamanho do pavio na comparação, e em caso afirmativo...
- Qual é a porcentagem aceitável

![image](https://user-images.githubusercontent.com/6900313/115163920-480df900-a082-11eb-9c9b-8e119cb0a421.png)

OBS.: esta seleção é estritamente **QUANTITATIVA** e não leva em considerações outros fatores necessários para a caracterização deste tipo de candle. 

Use com discernimento.
