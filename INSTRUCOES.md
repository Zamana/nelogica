# Importação de estratégias no Profit

Um arquivo .PSF contém uma estratégia exportada, que pode ser usado para se importar a estratégia diretamente no Profit.

Para importar uma estratégia em formato .PSF:

1. Clique em Estratégias -> Gerenciador de Estratégias:

![image](https://user-images.githubusercontent.com/6900313/114624995-f9c6b780-9c87-11eb-9e13-749bf0c48cad.png)

2. Clique em Importar:

![image](https://user-images.githubusercontent.com/6900313/114625232-4f9b5f80-9c88-11eb-9e40-13b46361c784.png)

3. Clique no ícone de PASTA após o campo Arquivo, e procure pelo arquivo .PSF no local onde o salvou:

![image](https://user-images.githubusercontent.com/6900313/114625734-157e8d80-9c89-11eb-8f64-a9f5d9b914f3.png)

E em seguida clique no botão "Importar".

# COPIA & COLA

Outra alternativa é criar uma estratégia nova e colar o código no editor, salvando com o nome desejado.

1. Clique em Estratégias -> Gerenciador de Estratégias

2. No editor, cole o código que foi obtido, e salve clicando no ícone do disquete:

![image](https://user-images.githubusercontent.com/6900313/114627355-81fa8c00-9c8b-11eb-9e41-0b45683c5cd1.png)

# Usando estratégias

Para inserir uma estratégia de execução, clique com o botão DIREITO do mouse sobre um *candle*, e selecione a opção "Inserir Estratégia de Execução":

![image](https://user-images.githubusercontent.com/6900313/114627707-12d16780-9c8c-11eb-9782-f627d0fe076b.png)

Em seguida procure pela estratégia que deseja inserir.

Para remover basta clicar com o botão DIREITO do mouse sobre um *candle* e clicar em "Excluir Estratégia de Execução".

# Regra de coloração

Para inserir uma regra de coloração, o procedimento é o mesmo da regra de execução: clique com o botão direito do mouse sobre um *candle* e selecione o item "Inserir Regra de Coloração". Para excluir, o procedimento é idêntico.

# Regra de seleção (SCREENING)

No Profit existe um recurso chamado **SCREENING** (Estratégias->Screening), que permite a seleção de ativos baseados em regras.

![estrategias_screening](https://user-images.githubusercontent.com/6900313/123527518-bb516e00-d6b6-11eb-8444-691c15f197ec.png)

As regras podem ser criadas usando-se um *wizard*, ou então codificadas. Para editar uma estratégia existente ou criar uma nova, clique no ícone do filtro:

![screening_filtro](https://user-images.githubusercontent.com/6900313/123527593-4c284980-d6b7-11eb-9e43-a0baa179010e.png)

Para criar uma nova, clique no ícone com o sinal de "+" em VERDE, dê um nome para a estratégia; para editar uma estratégia existente, selecione-a na lista à esquerda. 

![screening_novo_editar](https://user-images.githubusercontent.com/6900313/123527706-0324c500-d6b8-11eb-907f-9c2f11282c59.png)


Para usar o Wizard (limitado a 5 condições), deixe o "Usar Filtro" selecionado. Caso tenha uma estratégia codificada, mude para "Usar estratégia de Seleção" e selecione a estratégia desejada.

Para aplicar a estratégia, selecione a periodicidade, a lista de ações sobre as quais deseja aplicar a seleção ("COMPLETO" no exemplo) e então clique em "APLICAR".

DICA: colocar a janela do SCREENING no mesmo grupo das outras janelas permite que a ação seja alterada de acordo nas outras janelas (inclusive no gráfico) com um duplo-clique do mouse.

![screening_grupo](https://user-images.githubusercontent.com/6900313/123527801-e210a400-d6b8-11eb-9a8c-399eb3121d2a.png)

![image](https://user-images.githubusercontent.com/6900313/114629841-ac4e4880-9c8f-11eb-8b5e-3183b887a4a3.png)

Caso se opte pelo "Usar Estratégia de Seleção", basta selecionar a estratégia previamente codificada.
