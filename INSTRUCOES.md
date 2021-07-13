# Índice

[Importação de estratégias no Profit](#Importação-de-estratégias-no-Profit)

[Usando estratégias](#Usando-estratégias)

[Regra de coloração](#Regra-de-coloração)

[Regra de seleção (SCREENING)](#Regra-de-seleção-(SCREENING))

[Backtests](#Backtests)



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

Caso se opte pelo "Usar Estratégia de Seleção", basta selecionar a estratégia previamente codificada.

![image](https://user-images.githubusercontent.com/6900313/114629841-ac4e4880-9c8f-11eb-8b5e-3183b887a4a3.png)

Para aplicar a estratégia, selecione a periodicidade, a lista de ações sobre as quais deseja aplicar a seleção ("COMPLETO" no exemplo) e então clique em "APLICAR".

![screening_uso](https://user-images.githubusercontent.com/6900313/123527846-429fe100-d6b9-11eb-8eb9-1598767d28d8.png)

DICA: colocar a janela do SCREENING no mesmo grupo das outras janelas permite que a ação seja alterada de acordo nas outras janelas (inclusive no gráfico) com um duplo-clique do mouse.

![screening_grupo](https://user-images.githubusercontent.com/6900313/123527801-e210a400-d6b8-11eb-9a8c-399eb3121d2a.png)

# *Backtests*

O Profit possui uma ferramenta integrada bem interessante para a execução de *backtests*, que nada mais são do que a aplicação da estratégia codificada em dados do passado para que se possa ter uma ideia sobre como ela teria se comportado caso tivesse sido aplicada.

Lembrando do mantra "rendimentos passados não são garantia de rendimentos futuros", é necessário ter em mente que não necessariamente uma estratégia que se comportou bem no passado vai continuar se comportando bem no futuro. Há que se levar diversos fatores em conta.

Por exemplo, se a estratégia é focada exclusivamente em operaçòes *LONG* (na ponta da compra), ela terá um desempenho aceitável somente em ações que estejam em processo de valorização. Caso esta estratégia seja aplicada em ações em queda ou sem tendência, a performance certamente não será positiva.

Para se fazer *backtests* siga este roteiro:

1. No menu "Estratégias", clique em "Editor de Estratégias":

![image](https://user-images.githubusercontent.com/6900313/125375437-6a50a380-e35f-11eb-99f4-a08b64a35c8b.png)

2. No Editor de Estratégias, clique no ícone do disquete com a seta verde e selecione a estratégia desejada na lista (certifique-se de que a estratégia está com o *flag* "Execução" como "Sim":

![image](https://user-images.githubusercontent.com/6900313/125375722-ef3bbd00-e35f-11eb-87a6-aad453902d86.png)

3. No Editor de Estratégias, com o código da estratégia carregado, clique na aba "Misto", e no gráfico que está no lado direito da tela, digite o código do ativo sobre o qual deseja aplicar a estratégia:

![image](https://user-images.githubusercontent.com/6900313/125376047-8739a680-e360-11eb-8dff-fff70eb83c9d.png)

Certifique-se de escolher o tempo gráfico adequado para a sua estratégia neste gráfico: diário, semanal, 15 minutos etc.

4. Com o ativo selecionado, clique no botão *play* (seta verde para a direita) para executar a estratégia, ou tecle **F12**:

![image](https://user-images.githubusercontent.com/6900313/125376187-df70a880-e360-11eb-9f88-b697c01ea432.png)

5. Em seguida, clique na aba "Estatísticas", e veja o resultado da execução da estratégia:

![image](https://user-images.githubusercontent.com/6900313/125376376-370f1400-e361-11eb-8f5b-c3030e0d6655.png)

5.1 Resumo

![image](https://user-images.githubusercontent.com/6900313/125376436-5dcd4a80-e361-11eb-9833-b37c126235cc.png)

> Repare no capital inicial, percentual de operações vencedoras/perdedoras, fator de lucro, retorno do capital incial etc.

5.2 Lista de operações

![image](https://user-images.githubusercontent.com/6900313/125376545-9bca6e80-e361-11eb-83fd-b6f2d4cfce38.png)

5.3 Gráfico de operações

![image](https://user-images.githubusercontent.com/6900313/125376586-b4d31f80-e361-11eb-98b9-4dd20a37970d.png)

5.4 Evolução do capital

![image](https://user-images.githubusercontent.com/6900313/125376618-cd433a00-e361-11eb-8c30-7734797dc070.png)




