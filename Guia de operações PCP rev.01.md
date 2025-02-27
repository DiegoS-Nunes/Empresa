**Guia de operações PCP**

Abaixo está uma estrutura de como é a sequência do fluxo de trabalho do PCP:

![image](./Midia/workFlow.png?raw=true)

![alt text](./Midia/fluxograma.png?raw=true)

![alt text](./Midia/sequenceDiagram.png?raw=true)

# 1. ADM

Sistema que usamos para controlar as requisições.

Clique no ícone ![alt text](./Midia/admBarra.png?raw=true) na barra de tarefas ou ![alt text](./Midia/admDesktop.png?raw=true) no desktop.

> Duplo clique em ***`ADM`*** e insira seu login e senha
>
>![alt text](./Midia/abrirADM.png?raw=true)

>Digite o Nº `1` - aquamec.
>
>![alt text](./Midia/selecionarEmpresa.png?raw=true)

>Insira a senha novamente na tela seguinte.
>
>![alt text](./Midia/segundaSenha.png?raw=true)

>No módulo de requisição, selecione consulta
>
>![alt text](./Midia/requisicaoADM.png?raw=true)

>Aqui é possível ver todas as requisições feitas no sistema
>
>![alt text](./Midia/requisiçoesADM.png?raw=true)

>Navegue até a requisição com seu nome e tecle `ENTER`. Você poderá ver informações que identificam essa requisição. 
>
>![alt text](./Midia/detalhesRequisicaoADM.png?raw=true)
>
>Mais um `ENTER` e você poderá ver os itens da requisição.
>
>![alt text](./Midia/itensRequisicaoADM.png?raw=true)

>No módulo e compras é possível ver todos os pedidos de compra efetuados.
>
>![alt text](./Midia/comprasADM.png?raw=true)

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Em consulta é possível ver todos os detalhes de um pedido. Mas para uma consulta é recomendável utilizar `Consulta Origem(s)`, onde é possível ver todos os itens com pedidos por período ou por pedido.

![alt text](./Midia/origensADM.png?raw=true)

É possível selecionar por PV, por um período entre duas datas, ou os dois.

![alt text](./Midia/filtroOrigesADM.png?raw=true)
</div>

# 2. Egis
![alt text](./Midia/IconEGIS.png?raw=true)

Nosso sistema para construção das árvores dos pedido e emissão de requisições.

>**Usuário:** Guilherme
>**Senha:** #gro0924

## 2.1 Vendas

---

Assim que o comercial encaminha um pedido por e-mail, deve ser cadastrado no módulo de ***`Vendas internas`*** no EGIS para dar continuidade às operações.

## 2.1.1 Tipos de pedido

---

Existem 3 tipos de pedidos. Para saber diferenciar entre eles é necessário ter um pouco de experiência para saber o que é um equipamento e o que não é.

* **Pedidos de fabricação:**

![alt text](./Midia/pedidoFabricação.png?raw=true)

* **Pedidos de sobressalentes:**
Pedidos que contém peças de itens que compõe os equipamentos.

![alt text](./Midia/Pedido.png?raw=true)

* **Pedidos de reforma:**
Um de seus itens é um serviço de mão de obra.

![alt text](./Midia/pedidoReforma.png?raw=true)

## 2.1.3 Consultar pedido no EGIS

---

Os Nº de pedido são gerados automaticamente em sequência, não é possível escolher eles. Se você estiver precisando cadastrar um pedido com um Nº que não é o maior imediato ao último cadastrado, será necessário cadastrar pedidos com cliente e produto genérico para preencher o gap.

Exemplo: O último PV cadastrado é o PV0001 e você quer cadastrar o PV0005, você terá que cadastrar antes todos os PVs até chegar no PV0005. Pode cadastrar como cliente aQuamec com os itens em branco e depois alterar o cliente e os itens.

Por isso, deve ser consultados os pedidos em aberto para saber se o Nº do pedido já está em uso.

>Acesse o módulo de vendas
>
>![alt text](./Midia/iconVendas.png?raw=true)

>No menu esquerdo, selecione o menu `Consulta` e `Consulta de Pedidos`.
>
>![alt text](./Midia/iconConsultaPV.png?raw=true)

>Na tela que se abrir, selecione em `Data Inicial` selecione uma data mais antiga.
>
>Em `Data Final` a data de hoje.
>
>Clique em `Pesquisar`.
>
>Clique no nome da coluna `PV` para ordenar por ordem decrescente.
>
>![alt text](./Midia/ordenarColunaPV.png?raw=true)
>
>Os PVs com a descrição igual à `Obsoleto` não são PVs reais, são PVs aberto genericamente para preencher os que faltavam até atingir a numeração do PV mais recente.

## 2.1.3 Inserir pedido no EGIS

---

>Acesse o módulo de vendas
>
>![alt text](./Midia/iconVendas.png?raw=true)

>Selecione a operação desejada no menu lateral:
>
>![alt text](./Midia/iconPedidos.png?raw=true)

>Assim que abrir o menu de pedidos clique em ***`Cliente`*** para inserir um novo pedido. 
>
>![alt text](./Midia/iconCliente.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

As vezes o EGIS pula um número de pedido. É uma falha sistêmica, quando isso acontecer não tem nada que possamos fazer. Continue cadastrando a partir do número que pulou.
</div>

>Na próxima tela clique em CNPJ para procurar o cliente e selecione o que mais parecer com o cliente do pedido.
>
>![alt text](./Midia/insertCliente.png?raw=true)

>Se não tiver o cliente cadastrado clique em ***`inserir`*** no canto inferior esquerdo e preencha os dados do cliente no próximo formulário. Os campos mais importantes são os destacados em vermelho.
>
>![alt text](./Midia/insertButton.png?raw=true)
>
>![alt text](./Midia/insertDadosCliente.png?raw=true)

>Feito isso, um novo Nº de PV será gerado e você poderá inserir os itens do pedido.
>
>![alt text](./Midia/insertItensPedido.png?raw=true)

>No final clique em gravar e saia do módulo!
>
>![alt text](./Midia/savePedido.png?raw=true)

## 2.1.3 Alterando um pedido

---

>Para alterar os itens de um pedido é só acessá-lo através de menu de pesquisa e alterar seus dados.
>
>![alt text](./Midia/searchPedido.png?raw=true)

>Para alterar o cliente de um pedido será necessário acessar um menu diferente. Feche o módulo ***`Pedido de vendas`*** permanecendo apenas no módulo de ***`Vendas Internas`*** e selecione o módulo de alteração de cliente no menu esquerdo.
>
>![alt text](./Midia/iconAlterarCliente.png?raw=true)

>Na próxima tela selecione o tipo ***`Pedido de Venda`*** insira o número do pedido e em ***`Cliente`*** clique nos 3 pontos para selecionar o cliente e siga os passos de inserir clientes explicado anteriormente no item ***2.1.2***
>
>![alt text](./Midia/searchCliente.png?raw=true)

## 2.2 Engenharia

---

Todos os pedidos precisam ser engenheirados (ter desenho e lista de materiais) exceto itens padrões da lamor, tais como os abaixo:

![alt text](./Midia/tableItensLamor.png?raw=true)

Mas, **engenheirados ou não**, todos os itens precisam ter uma árvore no EGIS onde será feito requisição interna para retirá-los do estoque, ou de compra. Essa árvore deve ser aberta no módulo de engenharia após ter recebido os documentos da engenharia e cadastrado o pedido no módulo de vendas.

>Quando é um equipamento completo os documentos da engenharia, tais como as listas e desenhos, ficam salvos na rede ***Desenhos*** dentro da pasta ***PV_BOMBAS_E_VALVULAS*** ou dentro das pastas com o Nº do ano para os itens que são ***AQUAMEC***
>
>![alt text](./Midia/diretorio.png?raw=true)

>**Exemplo de lista da engenharia:**
>
>![alt text](./Midia/listaEngenharia.png?raw=true)

>**Exemplo de desenho de montagem:** 
>
>São aqueles que possuem no uma lista na descrição
>
>![alt text](./Midia/desenhoCJgeral.png?raw=true)

## 2.2.1 Explicando a interface

---

>**Acessar módulo de engenharia:**
>
>![alt text](./Midia/iconEngenharia.png?raw=true) 
>
>![alt text](./Midia/iconControlProjeto.png?raw=true)

![alt text](./Midia/interfaceEngenharia.png?raw=true)


## 2.2.2 A-Colunas

---

Ao arrastar as colunas para cima ou para baixo você pode remover elas, ao clicar no botão ![alt text](./Midia/iconColunas.png?raw=true) no menu inferior um menu lateral é aberto para você poder selecionar quais colunas quer ver.

![alt text](./Midia/optionColunas.png?raw=true)

## 2.2.3 A-Projetos

---

Na aba de projetos é possível ver itens dos pedidos que o comercial nos envia.

<div style="border-left: 4px solid #3498db; padding-left: 10px; background-color: rgba(52, 152, 219, 0.1);">

<p style="color: darkblue"><img src="./Midia/Note.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>NOTE</b></p>

Item do pedido = Projeto

Cada item do pedido deve ser cadastrado como um projeto diferente, com o mesmo PV. Conforme visto na imagem do tópico [2.2.1-Explicando a interface](##2.2.1-Explicando-a-interface)

</div>

Para cadastrar um pedido você deve iniciar um projeto.

### 2.2.3.1 C-Cadastrar Projeto

---

Para cadastrar um projeto, você deve cadastrá-lo utilizando o menu ![alt text](./Midia/iconProjetos.png?raw=true). Os campos necessários para cadastrá-lo e o formato padrão para cadastro é:

![alt text](./Midia/interfaceProjetos.png?raw=true)

>Assim que o inserir o ***`item`*** do ***`pedido de venda`*** e pressionar *tab* os dados do cliente e o ***`Nome do produto do cliente`*** serão preenchidos automaticamente com as informações cadastradas no módulo de vendas,conforme visto no tópico [2.1.2-Inserindo um pedido](##2.1.2-Inserindo-um-pedido). 

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Quando um Nº do pedido é pulado pelo sistema módulo de vendas no EGIS, não será possível preencher os dados automaticamente. Nesse caso preencha esse cadastro sem o Nº do ***`Item`***, para que não tente puxar os dados de maneira automática e insira o restante dos dados de forma manual conforme pedido enviado pelo comercial. E lembre-se de inserir a ***`Quantidade`***.
</div>

>Copie o ***`Nome do produto do cliente`*** e cole no ***`Nome interno`*** e no desenho insira o desenho do item, se não tiver também pode ser o nome do produto.

>Em ***`Projetista responsável`*** e ***`liberação`*** a única mudança que haverá em relação à da imagem é o nome do projetista que deverá ser *Josafá* para os itens da *Lamor* e *Rafael* para os demais.

>O ***`Centro de Custo`*** no rodapé também deve ser ***`14 - (193) Produção Glass`*** para itens de bombas, válvulas e suas partes. ***`1 - Aquamec Equipamentos`*** para itens da aquamec e ***`27 - LAMOR AMBIENTAL`*** para os itens da lamor.

## 2.2.4 B-Composições

---

Na aba de composições são subgrupos do projeto, geralmente divididos conforme os *desenhos* ou *listas* da engenharia.

![alt text](./Midia/interfaceComposição.png?raw=true)

### 2.2.4.1 C-Cadastrar Composição

---

Existem 2 formas de cadastrar uma composição, manualmente e por **Listas Standard**, manualmente será utilizado **somente** para itens que não forem de fabricação, mas sim de peças sobressalente, reformas, etc.

### 2.2.4.1.1 Manualmente

---

Forma de cadastro de composição utilizada **somente** para pedidos de sobressalentes

Para cadastrar uma composição, você deve estar dentro do projeto, para isso de 2 cliques na linha do projeto, ou selecionar o projeto e clique na aba ***`Composições`*** no campo **B**.

Os campos necessários de preenchimento são:

![alt text](./Midia/insertComposição.png?raw=true)

Onde ***`Item do Projeto`*** e ***`Tipo do Projeto`*** sempre deverão ser 1

O desenho deve ser sempre o Nº da lista da engenharia, que pode ser encontrado na capa da OP ou na própria lista:


### 2.2.4.1.1.1 Materiais

---

>Na interface de materiais é onde são cadastrados, de fato, todos os itens do projeto.
>
>![alt text](./Midia/interfaceMateriais.png?raw=true)

Para cadastrá-los, primeiro você deve estar dentro de uma composição. Para isso dê 2 cliques em uma composição, ou clique 1 vez e clique na aba de ***`Materiais`*** no campo **B**.

>Após isso clique no ícone de ***`Material`*** no campo **C** e um formulário se abrirá para você pesquisar o item do pedido. Clique no botão de inserir um novo pedido e logo após nos 3 pontos ao lado de **Fantasia Produto**
>
>![alt text](./Midia/insertMaterial.png?raw=true)

>Após isso um buscador se abrirá para você pesquisar o material. Pesquise pelo código ou pelo nome até achar o item desejado. Clique duas vezes sobre ele no botão ***Confirmar*** para adicioná-lo à lista de materiais do projeto.
>
>![alt text](./Midia/pesquisaMaterial.png?raw=true)

Existem duas colunas de quantidade, onde numa é possível ver a quantidade inserida na lista e noutra é possível ver a quantidade total do projeto. 

<div style="border-left: 4px solid #3498db; padding-left: 10px; background-color: rgba(52, 152, 219, 0.1);">

<p style="color: darkblue"><img src="./Midia/Note.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>NOTE</b></p>

Essa quantidade total é calculada multiplicando a quantidade que você inseriu durante essa fase de cadastro de materiais, a quantidade da composição e a quantidade do projeto, inseridos durante a inserção de seus respectivos cadastros.
</div>

Após concluir o preenchimento da lista de materiais clique no botão de salvar no canto inferior direito.

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Para pesquisar os itens utilize os caracteres **"%"**, por exemplo:

`%bomba`*** trará os resultados que terminem com *bomba*.

`bomba%`*** trará os resultados que comecem com *bomba*.

`%bomba%`*** trará os resultados que contenham *bomba*.

`%bomba%centrífuga%`*** trará os resultados que contenham *bomba* seguido de *centrífuga* com qualquer palavra no começo, no final e entre eles 
</div>

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

As vezes você encontrará itens com descrições semelhantes ou em duplicidade. Para saber qual o mais correto a se usar organize a coluna ***`disponibilidade`*** do maior para o menor, o qua tiver maior número de movimentações é o mais correto.
</div>

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Se não encontrar o produto específico deve ser solicitado o cadastro ao responsável por essa atividade.
</div>

### 2.2.4.1.2 Composição Standard

---

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>


~~**DESATUALIZADO: Atualmente estamos cadastrando as composições standard no projeto `STANDARD`**~~

![alt text](./Midia/standardProject.png?raw=true)

~~**Basta cadastrar e copiar para a o projeto que desejar.**~~

![alt text](./Midia/copyProject.png?raw=true)

![alt text](./Midia/copyComposição.png?raw=true)

</div>

---

Outra forma de cadastrar uma composição é pelas listas Standard quando receber a lista, ou desenho da engenharia. 

Os desenhos de usinagem (exceto bases de bomba e protetores do acoplamento de bombas) e fundição não precisam ser cadastrados, porém os desenhos de montagem, também chamados de desenho de conjunto geral, precisam.

### 2.2.4.1.3 Cadastrando Listas Standards

---

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

~~**DESATUALIZADO: Atualmente estamos cadastrando as composições standard no projeto `STANDARD`**~~

![alt text](./Midia/standardProject.png?raw=true)

~~**Basta cadastrar e copiar para a o projeto que desejar.**~~

![alt text](./Midia/copyProject.png?raw=true)

![alt text](./Midia/copyComposição.png?raw=true)
</div>

---

>Acesse ***`listas standard`*** dentro do campo **C**
>
>![alt text](./Midia/iconStandard.png?raw=true)

>No menu ***`Dados`*** clique em ***`Inserir`*** para adicionar uma nova composição
>
>![alt text](./Midia/insertStandard.png?raw=true)

Na composição standard insira um código, pode ser qualquer um já que terá que mudar o descrição para o aquela que mais te servir.

>Cadastrar a composição no item assim como foi explicado na seção *2.2.4.1.1* 
>![alt text](./Midia/createComposiçãoStandard.png?raw=true)

>Em seguida clique na aba ***`Material`*** para inserir os itens da composição. Essa aba contém duas abas de ***`dados`*** e ***`cadastro`***. Onde ***`cadastro`*** é o lugar que o item deve ser inserido e ***`dados`*** é onde são visualizados.
>
>![alt text](./Midia/insertMaterialStandard.png?raw=true)

>Na aba de ***`cadastro`*** os campos necessários de preenchimento são os destacados na imagem abaixo. Sendo o tipo de produto e matéria prima os únicos constantes
>
>![alt text](./Midia/insertItensStandard.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Se não for inserido o Tipo ***`Produto`*** e a ***`Matéria Prima`*** dará um erro.

Terminado de criar a composição, feche a janela. Escolha um projeto e dentro da aba  ***`Composições`*** no campo **B** clique em ***`Composição`*** no campo **C**.

![alt text](./Midia/insertComposicaoStandard.png?raw=true)

Selecione composição Standard no roda pé e na janela que abrir selecione todas as composições desejadas, conforme nº do ***`desenho`*** (que também pode ser a lista da engenharia) e clique em ok

![alt text](./Midia/iconComposiçãoStandard.png?raw=true)

![alt text](./Midia/selectComposiçãoStandard.png?raw=true)
</div>

<div style="border-left: 4px solid #3498db; padding-left: 10px; background-color: rgba(52, 152, 219, 0.1);">

<p style="color: darkblue"><img src="./Midia/Note.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>NOTE</b></p>

Vamos revisar. No campo **B**:
>Existe a aba de ***`projetos`***. Que são abertos conforme PV.
>>Dentro do projeto existem ***`composições`***. Que são abertas conforme os desenhos, ou listas
>>>Dentro das composições existem os ***`materiais`***. Que são abertos conforme os materiais dentro dos desenhos, ou listas.
</div>

## 2.2.5 Lista (Campo B)

---

Nessa aba é possível ver todos os itens que vão no pedido, mesmo que estejam em projetos diferentes, de forma resumida, ou seja, agrupados: Se tiver dois itens iguais dentro do mesmo projeto o item é mostrado apenas uma vez e a quantidade base(quantidade sem multiplicação) e somado, se tiver em projetos diferentes é mostrado uma vez para cada projeto.

E as quantidades não são multiplicadas.

![alt text](./Midia/sampleLista.png?raw=true)

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

**<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>**

Se quiser ver o mesmo resumo, mas contendo uma coluna separando por composições. Acesse o menu de produtos explicado no tópico *2.2.8.*

Se quiser copiar os dados, exporte para excel ou siga para a próximo tópico *2.2.6 Acompanhamento*

![alt text](./Midia/iconExportLista.png?raw=true)
</div>

## 2.2.6 Produtos (Campo B)

---

Faz a mesma função da lista, porém separa os itens de **1 projeto** por composição e não de vários projetos. E mesmo se tiver mais de 1 item idêntico na composição, não é agrupado.

Nessa aba é possível dar 2 cliques para selecionar e copiar os valores de dentro das células.

![alt text](./Midia/sampleProduto.png?raw=true)

## 2.2.7 Verificação de estoque.

---

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Se for um item da Lamor, a consulta de estoque deve ser feita pessoalmente com os coordenadores da Lamor, (atualmente o Sr. Clodiomiro e o Sr. José Nilton). Imprima uma cópia do PV e leve até eles para separar e liberar. Após isso siga para as etapas de requisição e liberação par coleta.
</div>

Após ter inserido o projeto, as composições e os itens das composições, o próximo passo é enviar para o almoxarifado verificar e separar o estoque.

>Para isso, monte um email conforme imagem abaixo. Encaminhando junto os documentos enviados pela engenharia.
>
>![alt text](./Midia/emailVerificação.png?raw=true)

>O almoxarifado responderá com a seguinte lista. Indicando o que tem e o que não tem em estoque:
>
>![alt text](./Midia/respostaALmoxarifado.png?raw=true)

Para os itens que foram marcados que temos disponível, faça uma requisição interna. (Continue a partir do passo 10-Plano de corte)

Para os itens que não temos disponível existem duas rotas a se tomar:

* Para o itens comerciais e fundidos faça uma requisição de compra.

* Para os itens usinados, imprima o desenho de usinagem, leve até o responsável pelo setor de usinagem (Atualmente é o Sr. Cristiano Sebastião), ele lhe dirá o que ele conseguirá fazer internamente e o que será necessário fazer uma requisição de compra do serviço de usinagem.

    Se ele for fazer internamente, faça uma requisição interna da usinagem. Se for externo existem duas rotas:

    * Verifique se o item é usinado a partir de fundido ou matéria prima. Na lista da engenharia está indicando isso.

    >![alt text](./Midia/fundidosEusinados.png?raw=true)
    >
    >Os itens acima são usinados a partir de fundidos. Os códigos dos desenhos dos fundidos começam com o número 1 e 2 para os usinados. Além disso, na descrição é possível observar que esses desenhos estão ligados com apenas um item.

    >![alt text](./Midia/usinadosDeMP.png?raw=true)
    >
    >Os itens acima são usinados a partir de matéria prima. Na descrição é possível observar que existem mais de um item e abaixo está descrito a matéria prima que será usinada para virar o item acima.

    * Para os itens usinados a partir de fundidos: Faça uma requisição de compra normalmente. Se já tivermos os fundidos em estoque, solicite a separação e a *liberação da Nota Fiscal de envio de remessa para industrialização*. Se não tiver em estoque, requisite a compra e aguarde o recebimento deles para depois solicitar.

    * Para os itens usinados a partir de matéria prima: Verifique se ele é comprado já com a matéria prima. Se for, é necessário fazer apenas a solicitação de compra. Se não for, faça um ***`Plano de Corte`*** e entregue ao responsável pelo setor de caldeiraria/fabricação (atualmente o Sr. Wellington Pereira).

## 2.2.8 Liberação (Campo C)

---

Após as árvores terem sido feitas. Tire um print do projeto e envie para o almoxarifado verificar os itens que temos disponíveis em estoque.

![alt text](./Midia/emailVerificação.png?raw=true)

Alguns códigos, naturalmente, estarão errados e o almoxarifado corrigirá. Corrija esses códigos dentro das listas standard e nos itens dentro de cada composição.

![alt text](./Midia/verificaçãoAlmoxarifado.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Para fazer requisições é necessário que os projetos estejam liberados. Certifique de fazer uma liberação a cada mudança dentro das árvores, se não as requisições não sairão conforme a última alteração.
</div>

Selecione o ícone de liberação no menu **C** ![alt text](./Midia/iconLiberação.png?raw=true). Existem duas forma de fazer a liberação

![alt text](./Midia/liberação.png?raw=true)

* **Liberar Projeto:** Você não precisa selecionar quais itens quer liberar, pois ela libera tudo que está dentro do projeto de uma vez só. Porém, é mais restritiva, pois ela só libera **1 projeto por vez**. 

    Se o **pedido** tiver vários itens e, por consequência, a árvore tiver vários **projetos**, você terá que sair da tela de liberação após liberar um projeto, entrar em outro projeto, acessar essa tela de liberação e liberar projeto.

    Portanto é melhor usá-la quando o pedido tiver apenas 1 item.

* **Liberar Seleção:** Você consegue liberar todos os projetos e seus itens de uma vez. Porém só funciona uma vez. Se todos os projetos do pedido já tiverem liberados, não será possível utilizar essa função, apenas a liberação de projeto.

    Portanto só a utilize **após** o almoxarifado ter respondido e todas as alterações terem sido feitas nos itens das composições dos projetos.

## 2.2.9 Requisição (Campo C)

---

Tendo corrigido e liberado a árvore do pedido e alinhado com os coordenadores o que será feito internamente e externamente, é hora de fazer as requisições e OPs (`Ordem de Produção`, no Hailer, conforme seção [### 3.1.5.1-Ordens de produção interna](###3.1.5.1-Ordens_de_produção_interna) abaixo)

>No campo **C** clique em geração de requisição
>
>![alt text](./Midia/gerarRequisição.png?raw=true)

>Na próxima janela que se abrirá, siga a rota abaixo:
>
>![alt text](./Midia/selecionarRequisição.png?raw=true)
>
>**1.** Clique em pesquisar para buscar os itens do da árvore do pedido. Aqui ele busca os itens de todos os projetos que contenham o título (que inicia com "PV...") semelhante.
>
>**2.** Selecione todos os itens que deseja requisitar.
>
>**3.** Clique para adicionar os itens selecionados na requisição
>
>**4.** E por fim gere a requisição desejada.

Ao clicar em ***`Gerar RC`*** abrirá uma janela de confirmação. 

>Certifique de ter selecionado o ***`centro de custo`*** *`(1-AQUAMEC, 14-GLASS, 27-LAMOR)`* correspondente ao pedido , conforme visto no tópico [1.2.3.1-Cadastrar Projeto (Campo C)](##1.2.3.1-C-Cadastrar-Projeto) e o ***`plano de compras`*** sempre será ***`01.15`***.
>
>![alt text](./Midia/requisiçãoCompra.png?raw=true)
>
>Você poderá verificar o sucesso da geração da requisição na coluna marcada abaixo:
>
>![alt text](./Midia/sucessoRequisicao.png?raw=true)

### 2.2.9.1 Alterar requisição

---

>Para editar as informações da requisição, acesso a página inicia do EGIS e clique em `Cadastro` e em `Requisição de compra`
>
>![alt text](./Midia/requisicaoCompraEgis.png?raw=true)

>Na janela que abrir:
>
>1. Selecione o período de tempo para filtrar.
>
>2. Clique em pesquisar, se quiser, insira o Nº da requisição. O sistema trará todas as requisições feitas no período. Clique na requisição desejada.
>
>![alt text](./Midia/todasRequisicaoCompraEgis.png?raw=true)
>
> Na aba itens, em`Fantasia` altere o código para o produto desejado. Altere a quantidade e é **importante** insirir o PV e o item (pode ser todos os itens como 1).
>
>![alt text](./Midia/editarRequisicaoCompraEgis.png?raw=true)

### 2.2.9.2 Exportar requisição

---

Após geradas as requisições é hora de exportar para o sistema ADM.

>Selecione a consulta de requisições
>
>![alt text](./Midia/consultaRequisições.png?raw=true)

>Escolha a data que foi emitida a requisição que deseja consultar
>
>Pesquise pelo Nº da requisição
>
>Exporte para Excel no caminho ***`req:\bkp\[crie uma pasta com seu nome]`***
>
>![alt text](./Midia/exportarRequisições.png?raw=true) 

>Salve com o Nº da requisição para ficar mais fácil a identificação
>
>![alt text](./Midia/arquivoReq.png?raw=true)

<div style="border-left: 4px solid #e74c3c; padding-left: 10px; background-color: rgba(231, 76, 60, 0.1);">

<p style="color: darkred"><img src="./Midia/Caution.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>CAUTION</b></p>

Para que a importação funcione corretamente é necessário que no primeiro espaço do nome do arquivo esteja preenchido com `_`. Como imagem acima
</div>

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Também é possível salvar todas as requisições em um único arquivo para exportar todas juntas.
</div>

>Certifique-se de que a coluna `Usuário` contenha seu nome e `Pedido de Venda` e `Projeto` tenham o PV referente ao item.
>
>![alt text](./Midia/colunasRequisição.png?raw=true)

>Salve no formato 97-2003
>
>![alt text](./Midia/salvarRequisição.png?raw=true)

>Copie os arquivos e cole na rede req. Automaticamente os arquivos serão importados para o sistema ADM.
>
>![alt text](./Midia/redeReq.png?raw=true)

Após a requisição estar no ADM e as OPs feitas no Hailer conforme seção [### 2.1.5.1-Ordens de produção interna](###2.1.5.1-Ordens_de_produção_interna) abaixo, envie no e-mail na seguinte estrutura:

>email para as requisições internas e OP (anexando as ops )
>
>![alt text](./Midia/emailRI.png?raw=true)

>Email para as requisições de compra:
>
>![alt text](./Midia/emailRC.png?raw=true)

# 3. Hailer
Nosso software para gerenciar os processos dos pedidos.

>**Login:** seu email
>
>**Senha:** mesma senha que usa para entrar no computador

## 3.1 Módulos

## 3.1.1 PCP em carga

---

Onde fica todos os PV's desde a abertura até expedição. Nos ajuda a ver em qual fase (Área) do processo o pedido está e qual ação está aguardando.

![alt text](./Midia/accessPPCPmodule.png?raw=true)

### 3.1.1.1 Inserindo dados no Hailer: 

---

Existem duas formas de inserir dados no Hailer:

### 3.1.1.1.1 Manualmente:

---

Clique em ![alt text](./Midia/iconAddButton.png?raw=true) e abrirá um menu lateral para você inserir os dados
![alt text](./Midia/insertPedidoHailer.png?raw=true)

A ***Data Cronograma*** será preenchida posteriormente somente pelo supervisor do PCP após ter elaborado o cronograma do pedido.

Na ***Área responsável e Ação*** são inseridos qual etapa do processo se encontra o pedido. Se for um pedido de bombas e válvulas, **sempre** precisará de desenho da engenharia para poder dar continuidade, então a Área responsável será preenchida com *ENGENHARIA* e a ação com *AGUARDANDO DESENHOS*

![alt text](./Midia/insertPedidoField1Hailer.png?raw=true)

Para pedidos padrões da Lamor cujo não é necessária a etapa de engenharia, conforme imagem vista no tópico [1.2 Engenharia](1.2-Engenharia), será aberto já como *ALMOXARIFADO* e *VERIFICANDO ESTOQUE*.

![alt text](./Midia/insertPedidoField2Hailer.png?raw=true)

Nas ***Observações*** deverá ser inserido o tipo de frete para o pedido e a transportadora. Essas informações são encontradas no pedido. Se o frete for *FOB* e não tiver transportadora insira como *FRETE: FOB - CLIENTE IRÁ DEFINIR*, caso seja *CIF* e não tiver a transportadora apenas insira *FRETE: CIF*, caso contrário, insira o tipo de frete e o nome da transportadora.

![alt text](./Midia/fieldsPedido.png?raw=true)

***Coordenadores***

 Os coordenadores do módulo PPCP e dos outros são diferentes vide tabela abaixo

|Setores|PPCP|Outros|
|:-|:-|:-|
|Aquamec|Lucas Azevedo|Se ÁREA = montagem, então é Jean;</br>Se ÁREA = Fabricação, então é Wellington|
|Bombas/Válvulas|Lucas Azevedo|Cristiano Sebastião|
|Lamor|Hilton Júnior|Jean Leme|

### 3.1.1.1.2 Importação:

---

Muito útil para pedidos grandes.
Selecione os seguintes botões
![alt text](./Midia/Ebutton.png?raw=true)

![alt text](./Midia/iconGenerate.png?raw=true)

Uma planilha, contendo em seu nome a palavra "template", será gerada. Ali você deve preencher com os dados que quer inserir no módulo do Hailer, aqui está um modelo.

![alt text](./Midia/interfaceTemplate.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Por se tratar de um sistema holandês, nos campos de **data** o único formato aceito pelo Hailer é **"AAAA.MM.DD"**.
E todos os campos, exceto *valor com impostos* deve ser do tipo texto. Por isso insira o código do pedido com uma aspas simples no início, se não o excel converterá o código em número.
</div>

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Não é necessário ter todos os campos preenchidos para poder fazer o upload no hailer e nem todos os campos serão upados mesmo se preenchidos, por exemplo: se existir mais de um cliente cadastrado com o mesmo nome (duplicidade), ou se estiver com o nome errado, o sistema irá upar o campo como vazio. Posteriormente ao upload esses dados poderão ser inseridos em conjunto conforme mostrado abaixo
</div>

---

<div style="border-left: 4px solid #e74c3c; padding-left: 10px; background-color: rgba(231, 76, 60, 0.1);">

<p style="color: darkred"><img src="./Midia/Caution.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>CAUTION</b></p>

~~**(DESATUALIZADO, os pedidos já vem com o IPI incluso no valor total do item)**~~

~~Quando haver um pedido com mais de um item, é importante adicionar o valor do IPI em cima do preço total de cada item para o valor final bater com o valor total do pedido. Para esse processo fica mais fácil importar os dados através do excel.~~

![alt text](./Midia/calculoValorPedido.png?raw=true)

![alt text](./Midia/dadosTemplate.png?raw=true)
</div>

### 3.1.1.2 Alterando dados no Hailer

---

Basta clicar na linha que deseja alterar os dados e no menu lateral que abrir à direita, clique no campo que deseja alterar e mude o valor. 

Para alterar várias linhas de uma só vez, marque a caixa de seleção à esquerda das linhas que deseja alterar ou na caixa de seleção da coluna para selecionar todos e em seguida no botão ***`edit x activities`***.

![alt text](./Midia/editAll.png?raw=true)

## 3.1.2 PCP concluído

---

Onde fica todos os PV's que já foram atendidos (expedidos). Muito útil na hora de procurar referências

![alt text](./Midia/interfaceAtendidosHailer.png?raw=true)

Toda vez que um PV for finalizado, deve-se imprimir a nota de venda que a contabilidade envia e por junto com os documentos físicos do PV que o comercial nos envia.

## 3.1.3 Follow Up pendentes

---

Onde fica os itens que controlamos e está pendente de recebimento.

![alt text](./Midia/interfacePendentesHailer.png?raw=true)

As informações contidas nesse módulo vem do sistema ADM.


### 3.1.3.1 Importando pedidos do ADM para o Hailer

---



>Ordene a coluna de requisição do menor para o maior ou ao contrário, conforme sua preferência, para ajudar na visualização dos dados
>![alt text](./Midia/fiterSC.png?raw=true)

No módulo de Follow Up Itens Pendentes, gere um template de importação para aquele módulo, conforme visto no passo [3.1.1.1. Inserindo dados no Hailer: Importação](3.1.1.1.-Inserindo-dados-no-Hailer:-Importação). 

Clique no nome da coluna de requisição para filtrar as requisições de compra do maior para o menor, ou ao contrário, conforme sua preferência, para ajudar na visualização dos dados.

Veja qual é o maior número de requisição que existe no Hailer e apague todas aquelas que são iguais ou menores na planilha exportada do ADM, pois já foram importadas para o HAILER.

Faça um filtro dos itens que o PCP não controla: Tudo que contém um número de PV, deve ser importado para o HAILER. Para os Itens que são para a fábrica, faça um filtro eliminando os que não são comercializados (ou seja, para consumo interno), tais como: Folha sulfite, marmitas, lanches, aparelhos eletrônicos, equipamentos de medição, madeira, etc.

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Lembrando que o Hailer só aceita datas no formato **AAAA.MM.DD** e os valores numéricos devem ser sem o ponto separador de milhar, contendo apenas a vírgula separadora dos decimais.
</div>

### 3.1.3.2 Preenchendo dados Follow Up

---

Após importar os dados do ADM para o Hailer, é importante que tenha preenchido o ***`NºPC`***, ***`Fornecedor`***, ***`Valor total`***. Nem sempre os dados que serão importados do ADM terão essas colunas preenchidas, o pessoal do suprimentos irá fechando cotações e inserindo os dados regularmente, por isso é importante verificar a consulta dinâmica (compras) todos os dias e preencher os dados que faltam no Hailer.

Também é importante que tenha os dados de ***`Data Solicitação NF`***, ***`NºNF`*** e ***`Data NF`*** (NF de remessa para Industrialização). Esses dados não ficam no ADM, a solicitação da NF é pedida no e-mail e a nota fiscal é envia por lá também, assim que for enviado o e-mail deve ser preenchido esses campos. Também seria interessante de anexar a NF nos itens do Hailer.

## 3.1.4 Follow Up recebidos

---

Onde fica o histórico de todos os itens que já recebemos.

![alt text](./Midia/interfaceRecebidosHailer.png?raw=true)

### 3.1.4.1 Dando baixa nos itens recebidos

---

Sempre que recebemos itens na fábrica o setor de recebimento envia as notas fiscais no grupo de recebimento no grupo do chat (ou outra ferramenta de mensagem que estiver usando no momento):

![alt text](./Midia/chatRecebimento.png?raw=true)

Essas notas ficam salvas para consulta em dois lugares. Na pasta da logística na rede: ***`LOGISTICA:\RECEBIMENTO\`*** e também no site: [TRIBUTUM](https://app.tributum.com.br/albriggs/nfes) (clique para acessar). Peça para o Helpdesk criar um acesso para você.

>![alt text](./Midia/tributumRoutes.png?raw=true)
>
>No passo 5 é possível salvar templates, ou seja, quais colunas quer ver e carregar sempre que vc acessar o site.
>
>No passo 6 clique com o botão direito do mouse sobre a nota que quer visualizar.

Após acessar a nota confira os seguintes dados:

>![alt text](./Midia/NF.png?raw=true)
>
>1. Nº da nota;
>
>2. Valor da nota;
>
>3. Descrição dos itens;
>
>4. **As vezes**, na descrição, vem o código do item, o número do pedido e o peso do item;
>
>5. A quantidade que recebemos;
>
>6. Nº Pedido de compra (geralmente na descrição ou rodapé);

Às vezes, o fornecedor envia uma quantidade diferente de material do que solicitamos. Às vezes eles põe outra peça no meio que também não está no pedido. Quando isso acontece, precisamos corrigir o pedido no Hailer.

Caso o item foi pedido para um PV, a quantidade não pode ser alterada nessa mesma linha, pois não vamos entregar material a mais ou a menos  do que o cliente solicitou. Nesse caso, duplique a linha, enderece o excedente para a fábrica e corrija o valor conforme o valor unitário na consulta dinâmica.

## 3.1.5 Ordem de produção em carga

---

Onde ficam todos os pedidos que estão em produção atualmente.
![alt text](./Midia/hailerProducao.png?raw=true)

>Esse módulo é onde são inseridos as datas dos cronogramas que o supervisor do PCP manda regularmente. Sobre essas datas, devem ser alinhado o andamento de seus respectivos itens regularmente com os líderes da produção, de preferência 1 ou 2 dias antes de vencer.
>
>![alt text](./Midia/hailerProducaoAtividades.png?raw=true)
>
>![alt text](./Midia/cronograma.png?raw=true)

Toda segunda-feira é feita uma reunião com todos os líderes para alinhar o andamento desses itens, discutir prazos e próximas etapas.

Assim que finalizado a reunião e o supervisor atualizar o cronograma, deve ser impresso um documento com os dados dos itens que serão finalizados na mesma semana e entregue aos líderes para o acompanhamento dos mesmos.

### 3.1.5.1 Ordens de produção interna

---

Também existem as ordens de produção nomeadas como OP. Essas OPs são itens qe nós produziremos internamente e que o almoxarifado dará entrada em estoque, tanto das que possuem ESTOQUE no nome, tanto das que possuem PV.

Essas OPs são registradas no Hailer da mesma maneira que os demais itens, porém com a nomenclatura `-OP.` a mais e o número sequencial daquela OP.

![alt text](./Midia/OPs.png?raw=true)

Essas OPs devem ser impressas, carimbadas e entregue ao seu supervisor de produção correspondente. Uma vez que estão finalizadas, eles entregarão ao gerente da produção junto com a quantidade de horas gasta na produção daquele equipamento, para que o mesmo possa dar baixa para o módulo de custo e também carimbar a OP. Então a OP será entregue fisicamente para o almoxarifado poder dar entrada do saldo dos itens em estoque.

Para imprimir uma cópia dessas OPs siga os passos abaixo:

> 1. Selecione a atividade que quer imprimir
>
> 2. Clique para editar todas as atividades
>
> 3. Clique em imprimir e um arquivo PDF com todas as atividades selecionadas será gerado para impressão
>
>![alt text](./Midia/imprimirOPs.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

* Todas as numerações de OP deve seguir uma sequência linear, não pode ter OP com numeração duplicada.
</div>

## 3.1.6 Ordem de produção finalizado

---

Onde ficam todos os pedidos que estavam em produção e foram finalizados.
![alt text](./Midia/interfaceEmCargaHailer.png?raw=true)


# 4. Plano de corte

Tendo terminado de:

1. Abrir o PV no EGIS - [1.1.2](1.1.2)

2. Realizar a árvore do projeto para o PV. [1.2.3.1](1.2.3.1)

3. Verificado o estoque. [1.2.7](1.2.7)

4. Corrigido o código dos itens nas composições do projeto e standard conforme informado pelo almoxarifado

5. Alinhado o que usinaremos / fabricaremos internamente ou não com os coordenadores

6. Feito as requisições [1.2.9](1.2.9)

Agora, se tiver itens que necessita de cortar matéria prima para enviar para o fornecedor industrializar, é necessário fazer um plano de corte para que a produção tome ação.

O plano de corte é relativamente simples, ele é composto por um cabeçalho onde ficam as informações do pedido relacionado e o corpo onde fica qual matéria prima deve ser cortada, em qual tamanho e para fazer oque.

![alt text](./Midia/planoDeCorte.png?raw=true)

Todas as informações podem ser obtidas em:

* **Desenho:** Lista da engenharia e desenho
* **Pos.(posição):** Desenho (geralmente 1)
* **Qt.(Quantidade):** Lista da engenharia e desenho
* **Qualidade:** Lista da engenharia e desenho
* **Dimensão Primária:** Lista da engenharia e desenho
* **Dimensão Secundária:** Lista da engenharia e desenho, mas é sempre bom se guiar pelo desenho, sempre ponha 5mm  mais de sobre-metal no comprimento dos perfis redondos.
* **Req. (Requisição de compra):** ADM, e-mail ou relatório ()
* **Peso:** Utilize a planilha show, disponível na rede: [PCP:/Diversos/Planilha Show](PCP:/Diversos/Planilha_Show), para descobrir o peso específico da matéria prima e calcule conforme sua necessidade:
    * Fórmula peso de MP:
        * **perfil redondo:** c(mm)/1000*pe
        * **perfil quadrado:** c(mm)/1000*pe
        * **perfil chato:** c(mm)/1000*pe
        * **chapa:** c(mm)/1000*L(mm)/1000*pe

            *pe = peso específico*
            
            *C= comprimento*

            *L= largura*

* **Fornecedor:** ADM, relatório (), ou Hailer se já tiverem inseridos
* **Descrição:** Árvore EGIS
* **Nº PC:** ADM, relatório (), ou Hailer se já tiverem inseridos
* **Código:** Árvore EGIS
* **Lote:** Sempre 1
* **Código MP:** Árvore EGIS
* **Código Estruturado:** Na planilha `Cadastro Itens SADI` disponível em `PCP:\Diversos`. Basta procurar pelo código que tem e na coluna ao lado estará o código estruturado. 

    ![alt text](./Midia/codigoEstruturado.png?raw=true)

    Caso o código estruturado esteja indefinido, peça para o responsável cadastrar.

* **Estoque:** Caso tenha acabado de fazer o plano de corte, ponha sempre verificando, caso a produção já tenha te retornado, altere para ***`Comprando`*** se a produção informar que não temos a matéria prima, ou ***`Ok`*** caso tenha.

O plano de corte também deve ser inserido no Hailer no módulo de produção em carga, com prazo curto, pois é uma verificação interna e também para ser mencionado na reunião do bom dia toda semana para relembrar, caso não tenha sido finalizado ainda.

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Sempre entregue o plano de corte com os respectivos desenhos para a produção poder analisar melhor.
</div>

---

# 5. Lista de Aprovisionamento


# 6. Solicitação Costumar (Dona Maria)

A dona maria nos fornece serviços de costura, geralmente para a Lamor, fazendo costura de zíperes para as sacolas de barreira, fabricar almofadas P2, etc.

A dona Maria, é uma fornecedora especial nossa, pois, diferente dos demais fornecedores, ela não possui um CNPJ e não emite notas, portanto as solicitações de trasporte e NF deve ser emitidas por nós. Toda conversa com ela é feita através de um grupo do whatsApp

>1. Pergunte à dona Maria sobre sua disponibilidade para poder enviar os materiais.

>2. Utilize o romaneio pré pronto ajustando o custo do material, peso e volume e mande para a Aline emitir nota. Para ajustar o preço basta entrar no SADI, ver o custo unitário da última compra do material, e acrescentar os impostos em cima. A fórmula ficaria assim:
>
>       ***`custo unitário*(1-(0,12+0,0165+0,076))`***
>
>       Peso e volume deve ser alinhado com o pessoal da lamor após cortar e separar o material.
>
>       ![alt text](./Midia/romaneioCostumar.png?raw=true)

>2. Crie uma solicitação do Hailer
>
>    ![alt text](./Midia/solicitaçãoTransporte.png?raw=true)

>3. Mova a solicitação para movimentação de materiais
>
>    ![alt text](./Midia/movimentaçãoMateriais.png?raw=true)

>4. Será solicitado o preenchimento dos dados da carga. Que devem ser levantados anteriormente com os funcionários da Lamor. Preencha apenas os seguintes campos, fazendo as alterações necessárias, mantenha os dados de origem e destino conforme abaixo:
>
>   ![alt text](./Midia/hailerCostumar.png?raw=true)

>5. Na devolução preencha a origem como destino e vice versa. Quando o material chegar, solicite ao sr.Adriano Assimões os recibos para pagamento.
>
>![alt text](./Midia/emailReciboCostumar.png?raw=true)

>6. Quando ele enviar, repasse para o sr. Alex e sr. Roberto efetuarem o pagamento.
>
>![alt text](./Midia/emailPagamentoCostumar.png?raw=true)

# 7. Planilha de Análise Hailer

Para facilitar a análise do Hailer, eu desenvolvi um arquivo de excel que contém várias planilhas que analisam os dados do Hailer, formata e cria planilhas automaticamente.

Para utilizá-la, basta exportar os dados das abas de ***`PPCP em carga`***, ***`PPCP finalizado`***, ***`Follow Up Pendentes`***, ***`Ordem de produção em carga`***, `Relatório de compras do ADM` e `Relatório de Requisições do ADM`.

## 7.1. Extraindo relatório do Hailer

---

>Selecione o botão de exportação no canto superior direito
>
>![alt text](./Midia/buttonExportHailer.png?raw=true)
>
>Selecione para extrair:
>
>![alt text](./Midia/ExportHailer.png?raw=true)

## 7.2. Extraindo relatório do ADM

---

>1. Dentro do módulo de requisição, selecione `Rastreamento (CSV)`
>
>![alt text](./Midia/admRQRelatExtract.png?raw=true)
>
>2. Em `Somente com Referência`, insira `N` para que traga todos os itens.
>
>3. Em `Dados Ordenado` selecione 1.
>
>4. Em `Separador Decimal` digite `,`.
>
>5. Digite `S` na última caixa para salvar o arquivo.
>
>![alt text](./Midia/admRQRelatForm.png?raw=true)


>1. Selecione `Relatório` dentro do módulo de compras.
>
>![alt text](./Midia/admPCRelatExtract.png?raw=true)
>
>2. Em `Somente em Aberto`, insira `N` para que traga todos os itens.
>
>3. Em `Ordem de Impressão` selecione 1.
>
>4. Em `Impressão` digite `I`.
>
>5. Em `Separador Decimal` digite `,`.
>
>6. Na última etapa abrirá um pop up, selecione `Disco` para gravar o arquivo no PC.
>
>![alt text](./Midia/admPCRelatForm.png?raw=true)

>Os arquivos ficarão salvos no caminho: `relcmp\relat`
>
>![alt text](./Midia/caminhoRelatorios.png?raw=true)

## 7.3. Gerar Relatórios

---

Renomeie os arquivos do Hailer, removendo o sufixo `_AAAA-MM-DD` (ano-mês-dia) e do ADM deixe apenas a primeira palavra.

>Mova e substitua os arquivos para a pasta `PCP:\Indicadores\Consultas\Dados`
>
>![alt text](./Midia/diretorioDados.png?raw=true)</br>

>Abra cada uma das exportações e transforme os dados em tabela.
>
>![alt text](./Midia/formatarTabela.png?raw=true)

<div style="border-left: 4px solid #e74c3c; padding-left: 10px; background-color: rgba(231, 76, 60, 0.1);">

<p style="color: darkred"><img src="./Midia/Caution.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>CAUTION</b></p>

**É importante que a tabela de todas as planilhas estejam nomeadas como _"Tabela1"_.**

![alt text](./Midia/tableName.png?raw=true)
</div>

>Para o arquivo `req` existem duas colunas de descrição, sendo uma a continuação da outra, pois no adm tem um limite de caracteres para a descrição.
>
>![alt text](./Midia/reqColunasDescricao.png?raw=true)
>
>Acontece que as vezes o texto é dividido logo antes do hífen `-`, fazendo com que a segunda coluna inicie com esse caractere. Porém, para o Excel, isso é entendido como uma fórmula e ele acaba realizando uma operação calculada.
>
>![alt text](./Midia/reqDescricaoCalculo.png?raw=true)
>
>Em alguns casos pode resultar em erro também.
>
>![alt text](./Midia/reqDescricaoErro.png?raw=true)
>
>Para evitar isso, é melhor substituir todos os valores `=-` por `'-` (pondo um apóstrofo no início, o Excel entende que é um texto e não uma fórmula ou número)
>
>![alt text](./Midia/substituirDescReq.png?raw=true)

Acesse o arquivo ***`Análises H_CD`*** no caminho: `PCP:\Diego\Procedimento PPCP\Consultas` ![alt text](./Midia/H_CD.png?raw=true).

>Na aba dados clique em atualizar tudo 
>
>![alt text](./Midia/atualizarTudo.png?raw=true)

>Se aparecer o erro `[Expression.Error]` é porque o arquivo não está formatado em tabela. Formate e tente novamente.
>
>![alt text](./Midia/Expression.Error.png?raw=true)

>Se aparecer o erro abaixo é porque o arquivo não está na pasta correta, ou está nomeado errado.
>
>![alt text](./Midia/localizarArquivoErro.png?raw=true)

Renomeie os arquivos como mostrado  o arquivo para a pasta correta, como mostrado na imagem no início dessa seção.

Verifique se o caminho da pasta está correto:

>Na aba *Dados* clique em ***`Mostrar Consultas`***
>
>![alt text](./Midia/mostrarConsultas.png?raw=true)

>Na aba lateral que aparecer clique com o direito em qualquer consulta e em *Editar*.
>
>![alt text](./Midia/editarConsulta.png?raw=true)


>No lado esquerdo clique na seta para expandir as consultas
>
>![alt text](./Midia/expandirConsulta.png?raw=true)

>Na aba que abrir, clique no parâmetro ***`LocalDosArquivos`*** e troque a letra inicial pela letra que indica a unidade do PCP na rede, pode ser diferente em cada computador.
>
>![alt text](./Midia/editarParametro.png?raw=true)
>
>![alt text](./Midia/redePCP.png?raw=true)

>Feito isso clique no botão para fechar o power query e carregar as consultas.
>
>![alt text](./Midia/fecharEcarregar.png?raw=true)

>Fazendo isso todas as planilhas serão atualizadas, conforme observado no rodapé da planilha. Pode demorar alguns segundos.
>
>![alt text](./Midia/statusAtualizacao.png?raw=true)

## 7.4. Alterar formatação condicional

---

>Você perceberá que em partes das tabelas está com a formatação bagunçada. Isso é comum de acontecer quando a planilha é atualizada.
>
>![alt text](./Midia/fomatacaoErrada.png?raw=true)

>Para corrigir isso, acesse as configurações da formatação condicional.
>
>![alt text](./Midia/fomatacaoCondicional.png?raw=true)

>Na janela que abrir selecione todas as formatações da planilha, arraste a barra lateral até encontrar as formatações cuja a fórmula se inicia nas primeiras linhas. Exclua todas as outras formatações exceto elas.
>
>![alt text](./Midia/excluirFormatacao.png?raw=true)

>Corrija o local de aplicação para coincidir com a ultima coluna e a última linha da planilha.
>
>![alt text](./Midia/aplicacaoFormatacao.png?raw=true)

## 7.5. Req

---

Planilha que trata os dados do módulo de requisições do ADM.

![alt text](./Midia/reqBar.png?raw=true)

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacaoReq.png?raw=true)

## 7.6. PC

---

Planilha que trata os dados do módulo de compras do ADM.

![alt text](./Midia/pcBar.png?raw=true)

<div style="border-left: 4px solid #3498db; padding-left: 10px; background-color: rgba(52, 152, 219, 0.1);">

<p style="color: darkblue"><img src="./Midia/Note.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>NOTE</b></p>

Essa planilha não precisa de correção na formatação condicional.
</div>

>Todo dia de manhã, depois de atualizar a planilha, copie ela inteira apertando `Ctrl+Espaço` 2 vezes.
>
>![alt text](./Midia/selectPC.png?raw=true)

>Abra um novo arquivo Excel e cole a tabela mantendo a formatação original.
>
>![alt text](./Midia/planilhaPC.png?raw=true)

>Selecione a planilha inteira novamente, altere o tamanho da fonte para 9 e na aba exibir, desmarque a opção de mostrar as linhas de grade
>
>![alt text](./Midia/tirarGrade.png?raw=true)

>Salve renomeando o arquivo para `PC dd mm aaaa` (dia mês ano) e mande no e-mail da seguinte maneira:
>
>![alt text](./Midia/emailCD.png?raw=true)

## 7.7. CD

---

Planilha que mescla a planilha de RQ com a PC, se o item da requisição já não estiver na planilha PC.

![alt text](./Midia/cdBar.png?raw=true)

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacaoCdBar.png?raw=true)
>
>![alt text](./Midia/formulaFormatacaoCdBar.png?raw=true)

Copie os dados para uma nova planilha assim como na seção anterior e envie no chat do supervisor do PCP.

## 7.8. SC sem RC

---

![alt text](./Midia/SCsemRC.png?raw=true)

Essa planilha contém uma tabela, que mostra todos os PVs do módulo ***`Follow Up Pendentes`*** que não possuem Nº SC EGIS, ou Nº SC ADM, ou Nº PC.

>Utilize a planilha PC ou CD, conforme seções anteriores, para filtrar essas SC e se tiver um Nº PC, insira no item correspondente em ***`Follow Up Pendentes`*** junto com o *Data PC*, *Fornecedor* e *Valor Total*.
>
>![alt text](./Midia/preencherFollowUp.png?raw=true)

## 7.9. 100% Recebido

---

Planilha que mostra os **PVs** (não itens) que tem no módulo `Ordem de Produção - Em carga` e não tem no módulo `Follow-up - Pendentes`.

Todos os itens dessa planilha deve estar com todas as linhas da coluna `Observações` escrito `MP OK`. 

Se não estiver, quer dizer que ainda não recebemos o item, ou que ainda não está inserido no módulo de `Follow-up - Pendentes`. Para verificar isso, basta acessar o módulo de `Follow-up - Recebidos` e procurar pelo PV e pelo item. Se já tivermos recebido então pode alterar a observação para `MP OK` no módulo `Ordem de Produção - Em carga` no Hailer.

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacao100.png?raw=true)
>
>![alt text](./Midia/formulaFormatacao100.png?raw=true)

## 7.10. !=100% recebido

---

![alt text](./Midia/barNaoRecedibos.png?raw=true)

Assim como a planilha de **100% recebido**, esta planilha verifica se existe alguma linha no módulo `Follow-up - Pendentes` que tenha o mesmo PV contido em `Ordem de Produção - Em carga` e que contenha a `AÇÃO`=`MONTAGEM` ou `EMBALAGEM` (últimas fases dos processos). Indicando que o PV ainda tem itens pendentes de recebimento.

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacaoNaoRecedibos.png?raw=true)
>
>![alt text](./Midia/formulaFormatacao100.png?raw=true)

>Após aplicar a formatação padrão, para ficar mais fácil de ver, verifique a coluna `Observações`. Cada PV deve ter pelo menos 1 item `AGUARDANDO MP`, se todos estiverem escrito `MP OK` e ainda estiver nessa planilha, quer dizer que a coluna `Observações` está errada no Hailer, verifique os itens pendente de recebimento e altere a observação daqueles que ainda não chegaram para `AGUARDANDO MP`.
>
>![alt text](./Midia/telaNaoRecebidos.png?raw=true)

## 7.11. Cronog. Pendentes

---

![alt text](./Midia/barCronPendentes.png?raw=true)

Planilha onde fica a tabela contendo os **PVs** que tem no módulo `PPCP em carga` mas não tem em `Ordem de Produção em carga`.

<div style="border-left: 4px solid #e74c3c; padding-left: 10px; background-color: rgba(231, 76, 60, 0.1);">

<p style="color: darkred"><img src="./Midia/Caution.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>CAUTION</b></p>

Em casos especiais, pode ter item que está no módulo do `PPCP em carga` e nao tem atividade no módulo de `Ordem de Produção`, pois não tem ação interna. Avalie cada caso.
</div>

## 7.12. Controle Produção

---

![alt text](./Midia/barControleProducao.png?raw=true)

Planilha que busca todos os dados do módulo `Ordem de Produção em carga` e trás todas as atividades previstas para serem finalizados na semana. Organizando por Coordenador, data de término, PV.

Essa planilha serve para auxiliar você quando tiver que descer no chão de fábrica e ir cobrar os coordenadores dos itens pendentes para serem finalizados na semana.

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacaoControleProducao.png?raw=true)

>**Fórmula linha tracejada:**
>
>![alt text](./Midia/formulaLinhaTracejada.png?raw=true)

>**Fórmula linha cinza:**
>
>![alt text](./Midia/formulaLinhaCinza.png?raw=true)

## 7.13. Expedição

---

![alt text](./Midia/barExpedicao.png?raw=true)

Planilha onde fica todos os itens do módulo `PPCP em carga` que estão na fase `AGUARDANDO COLETA`, essa é uma planilha `importante` que deve ser impressa diariamente e entregue ao responsável pelas embalagens. (Atualmente o Sr. Edson Guimarães). Para que não ocorra de a transportadora vir coletar um item que ele foi informado para fazer a embalagem.

Essa coluna possui um vínculo com a próxima planilha **`Data S.Coleta`** 

Após realizar os procedimentos do próximo passo em 
`Data S.Coleta`, volte a essa planilha.

>A coluna `Solicitação` altere qualquer uma das linhas pra o Nº Máximo de linhas da planilha `Data S.Coleta`
>
>![alt text](./Midia/alterarFormulaExpedicao.png?raw=true)

Aplique a formatação padrão e imprima. 

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacaoExpedicao.png?raw=true)

<div style="border-left: 4px solid #e74c3c; padding-left: 10px; background-color: rgba(231, 76, 60, 0.1);">

<p style="color: darkred"><img src="./Midia/Caution.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>CAUTION</b></p>

Lembre-se de deixar apenas o frete e transportadora na observação e a descrição complementar do item se houver. Apague os dados de valor de frete e outras informações sensíveis e não importantes.

![alt text](./Midia/observacaoExpedicao.png?raw=true)
</div>

## 7.14. Data S.Coleta

---

![alt text](./Midia/barDataSolicColeta.png?raw=true)

Planilha onde ficam as datas que foi solicitado coleta do PV. Serve para inserir as datas automaticamente na planilha anterior, `Expedição`.

>Na planilha de `Expedição` copie todos os PVs que não tenham uma data de solicitação.
>
>![alt text](./Midia/expedicaoSemData.png?raw=true)


>Na planilha Data S.Coleta cole na parte inferior:
>
>![alt text](./Midia/completarPVDataSemColeta.png?raw=true)


>Mantenha um registro único e sem hífen.
>
>
>![alt text](./Midia/arrumarPVDataSemColeta.png?raw=true)

>Você perceberá que irá aparecer um número na primeira coluna. Esse número vai aparecer caso haja um registro correspondente ao PV na planilha de `Expedição`. Caso esse célula fiqu em branco, pode excluir a linha, pois o item já foi coletado, ou já foi emitido nota para ele.
>
>![alt text](./Midia/formulaPVDataSemColeta.png?raw=true)

>No e-mail pesquise pelo primeiro e-mail de solicitação de coleta ou de liberação de faturamento do PV e insira a data na coluna `Scoleta`.
>
>![alt text](./Midia/emailAgendarColeta.png?raw=true)
>
>![alt text](./Midia/dataAgendarColeta.png?raw=true)

## 7.15. Clientes

---

![alt text](./Midia/barClientes.png?raw=true)

Planilha onde os ficam os clientes de cada PV e o nome simplificado desse cliente. Essa planilha é um banco de dados de nomes simplificados que são utilizados em outras planilhas. Como `Controle Produção`, `Expedição` e `FORM-AQU-403 - Ordem de Produção`, este último veremos na próxima seção, é uma arquivo excel externo e também é por esse motivo que essa planilha de clientes não pode ficar oculta, porque arquivos externos não conseguem ver planilhas ocultas.

# 8. FORM-AQU-403 - Ordem de Produção

---

Funciona igual a planilha de `Controle produção` da seção [7.12. Controle produção](712-Controle-Produção). Mostrando tudo pendente de finalizar na semana. Essa planilha deve ser impressa toda segunda-feira após a reunião do bom dia, onde são acertados as entregas da semana e entregues à cada coordenador.

>Abra o gerenciador de arquivos e navegue até `PCP:\Forms`, existe um arquivo chamado `FORM-AQU-403 - Ordem de Produção`
>
>![alt text](./Midia/caminhoForm403.png?raw=true)

Atualize tudo como mostrado na seção [## 7.3. Gerar Relatórios](*)

>**Formatação Padrão:**
>
>![alt text](./Midia/formatacaoForm403.png?raw=true)
>
>![alt text](./Midia/formulaLinhaForm403.png?raw=true)
>
>![alt text](./Midia/formulaCorForm403.png?raw=true)

>Copie o nome do coordenador que vai imprimir na célula indicada na imagem abaixo. Automaticamente o cabeçalho vai mudar para o nome daquele coordenador.
>
>![alt text](./Midia/processoImpressaoForm403.png?raw=true)

Após formatar a planilha, faça um filtro e imprima uma para cada coordenador.

# 9. Horas funcionários
## 9.1. Folhas de Horas

---

>Abra o gerenciador de arquivo e navegue até a pasta `PCP:\Indicadores\Horas_funcionarios\Modelo apontamento de horas`. Lá você encontrará as planilhas de apontamento de horas:
>
>![alt text](./Midia/arquivosHoras.png?raw=true)

* **`Apontamento de horas modelo:`** Essa planilha deve ser impressa periodicamente, contendo os próximos dias de trabalho **(incluindo Sábado)** e entregue para cada funcionário do **chão de fábrica** preencher.

    ![alt text](./Midia/planilhaApontamentoHoras.png?raw=true)

* **`Apontamento [coordenador]:`** Essa planilha é separada por dia, contendo o nome de todos os funcionários de um coordenador. Após coletar a folha de horas `Apontamento de horas modelo`, passe os dados digitalmente para esses arquivos.

    ![alt text](./Midia/folhaApontamentoHoras.png?raw=true)

Após preenchido e conferido a folha `Apontamento [coordenador]` de cada dia, leve até o gerente da produção para ser carimbado.

Após ser carimbado, lance as horas no EGIS.

## 9.2. Cadastrar funcionários no EGIS

---

Quando entrar um funcionário novo, é necessário lançar em dois lugares no EGIS para cadastrar.

## 9.2.1. Cadastro Geral

---

Abra o EGIS clique no ícone de `Cadastramento Geral`
![alt text](./Midia/iconCadastroGeralEgis.png?raw=true).

>No menu Empresa, navegue para baixo até achar o menu de cadastro de funcionário. 
>
>![alt text](./Midia/iconFuncionarioEgis.png?raw=true)

Clique no botão para inserir um novo registro>
![alt text](./Midia/buttonInsert.png?raw=true)

>Na tela que abrir, preencha os campos:
>
>* **`Empresa:`** AQUAMEC
>* **`Nome Fantasia:`** Nome do funcionário
>* **`Chapa:`** Pergunte ao coordenador responsável, ao RH, veja no cartão ponto do funcionário, ou pergunte ao próprio funcionário.
>* **`Funcionário:`** Nome do funcionário
>* **`CPF:`** Pergunte ao coordenador responsável, ao RH, ou ao próprio funcionário.
>
>![alt text](./Midia/preencherFuncionário.png?raw=true)

## 9.2.2. Módulo de PCP

---

Na tela inicial do EGIS entre no módulo de PCP
![alt text](./Midia/iconPCPEGIS.png?raw=true)

>Em `operador`, selecione `operador`
>
>![alt text](./Midia/buttonOperador.png?raw=true)

Clique no botão para inserir um novo registro
![alt text](./Midia/buttonInsert.png?raw=true)

>Na tela que se abrir preencha os seguintes campos:
>
>* **Nome:** Nome do funcionário
>* **Chapa:** Pergunte ao coordenador responsável, ao RH, veja no cartão ponto do funcionário, ou pergunte ao próprio funcionário.
>* **Turno:** Sempre Diurno
>* **Status:** Sempre ativo
>* **Setor:** Podem ser apenas os setores abaixo. Confirme o setor de operação com o Coordenador do funcionário:
>   * Caldeiraria
>   * Montagem AQUAMEC
>   * Montagem Bombas e Válvulas
>   * Montagem LAMOR
>   * Solda
>   * Traçagem Corte e Preparação
>   * Usinagem
>
>* **Apontamento produção:** Sempre sim.
>
>![alt text](./Midia/preencherOperador.png?raw=true)

## 9.3. Lançando as Horas

---

Após as folhas de apontamento terem sido carimbadas pelo gerente conforme instruído na seção [9.1. Folhas de Horas](#), é hora de lançar elas no sistema.

Na tela inicial do EGIS entre no módulo de PCP
![alt text](./Midia/iconPCPEGIS.png?raw=true).

>No menu lateral esquerdo, role tudo pra baixo e acesse `Movimento Apontamento Produção`.
>
>![alt text](./Midia/movimentoApontamentoProdução.png?raw=true)

Na tela que se abrir, no menu inferior, clique no ícone ![alt text](./Midia/ocultarMovimentoApontamentoProdução.png?raw=true) para fechar o menu lateral.

>Na parte superior, selecione o intervalo de datas que deseja trabalhar.
>
>![alt text](./Midia/selecionarDataMovimento.png?raw=true)

>Clique no botão executar. Se não tiver dados naquele período, não aparecerá nada, se tiver aparecerá uma tabela.
>
>![alt text](./Midia/telaApontamento.png?raw=true)

Clique **duas vezes** no botão para inserir um novo registro
![alt text](./Midia/buttonInsert.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

É importante clicar mais de uma vez nesse botão, já que clicar apenas uma vez, o sistema pode não entender que é um novo registro, assim, ao inserir um novo dado, o último que lançou será sobrescrito.
</div>

>Preencha os campos do formulário que abrir.
>
>![alt text](./Midia/formularioApontamento.png?raw=true)
>
>* **Em vermelho:** Preenchimento obrigatório.
>   * **Identificação:** Preencher com `PV`, ou `OP` e o número, ou `PVXXXX-OPXXXX`. 
>   * **Improdutiva:** O código é `7.XX` mas preencha esse campo com apenas o número `XX` (após o ponto).
>   * **Produção / Hora extra:** Pode preencher apenas um dos dois, ou os dois caso pertençam ao mesmo PV
>* **Em verde:** Preenchimento obrigatório, tem que ser o último campo preenchido, para que o sistema consiga calcular automaticamente.
>* **Em azul:** Campo calculado automaticamente. **O total de horas de produção não podem ultrapassar 8:48.**
>

> Se **``Identificação``** tem algum dado, então **``Improdutiva``** deve estar vazia, a não ser que **``Identificação``** seja uma OP para estoque, ou retrabalho. Nesse caso deve ter
>
>![alt text](./Midia/regraIdentificacaoProdutiva.png?raw=true)

No final, clique em gravar ![alt text](./Midia/buttonGravar.png?raw=true) para salvar os dados.

## 9.4. Consistência dos dados

---

Após ter lançado todos os dados, verifique por inconsistências que podem surgir depois.

## 9.4.1. Horas produtivas e improdutivas

---

>Clique em executar 
>
>![alt text](./Midia/buttonExecutar.png?raw=true)

>Filtre as horas improdutivas pelas células **não** vazias.
>
>![alt text](./Midia/filtroHorasImprodutivas.png?raw=true) 

>Organize a coluna de identificação por ordem crescente ou decrescente 
>
>![alt text](./Midia/fintroIdentificacao.png?raw=true)

>Verifique se os lançamento que tem a coluna `Hora improdutiva` preenchida, estão com a coluna `Identificação` vazia. Só podem ter as duas preenchidas caso seja uma **OP** para estoque, ou **retrabalho**.
>
>![alt text](./Midia/corrigirIdentificacaoImprodutiva.png?raw=true)

>Para remover o filtro, remova ele na parte inferior da tela
>
>![alt text](./Midia/removerFiltroInferior.png?raw=true)
>
>Se quiser remover apenas um filtro específico, selecione `All` na coluna filtrada.
>
>![alt text](./Midia/removerFiltroSuperior.png?raw=true)

## 9.4.2. Intervalo

---

>Organize a coluna `Intervalo` por ordem crescente ou decrescente.
>
>![alt text](./Midia/filtroIntervalo.png?raw=true)

>Corrija os dados lançados incompletos ou errados.
>
>![alt text](./Midia/erroIntervalo.png?raw=true)

## 9.4.3. Quantidade Total de Horas

>Organize a coluna `Quantidade Total de Horas` por ordem crescente ou decrescente.
>
>![alt text](./Midia/filtroQtdTotalHoras.png?raw=true)

>Corrija as horas negativas, ou que são superiores à 8:48
>
>![alt text](./Midia/erroQtdTotalHoras.png?raw=true)

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Verifique se isso não pode ser um erro de ordem de inserção dos dados. Como mostrado na seção [9.3. Lançando as Horas]()
</div>

## 9.4.4. Intervalo Extra

---

>Organize a coluna `Qtd. Total Extra` por ordem crescente ou decrescente. 
>
>![alt text](./Midia/filtroQtdTotalExtra.png?raw=true)

>Corrija as horas negativas, ou superiores.
>
>![alt text](./Midia/erroQtdTotalExtra.png?raw=true)

<div style="border-left: 4px solid #3498db; padding-left: 10px; background-color: rgba(52, 152, 219, 0.1);">

<p style="color: darkblue"><img src="./Midia/Note.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>NOTE</b></p>

O intervalo na hora extra funciona igual para as horas normais, deu 12:00 tem pausa para almoço.
</div>

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Verifique se isso não pode ser um erro de ordem de inserção dos dados. Como mostrado na seção [9.3. Lançando as Horas]()
</div>

## 9.5. Exportar Horas Funcionários

---

>Após ter lançado e corrigido as horas dos funcionários. Extraia a tabela para o excel no menu superior. E salve no caminho `PCP:\Indicadores\Horas_funcionarios\Movimento Apontamento Produção` no formato excel 97-2003
>
>![alt text](./Midia/extrairHorasExcel.png?raw=true)

>Após isso, abra esse mesmo arquivo. Transforme os dados em tabela e exclua a última linha de totais.
>
>![alt text](./Midia/excluirLinhaHoras.png?raw=true)
>
>Ao fechar o arquivo, será pedido que salve em outro formato mais atualizado, pode salvar e sobrescrever o arquivo de mesmo nome.
>
>![alt text](./Midia/arquivoHorasAtualizado.png?raw=true)

## 9.6. Planilha de Análise Horas Funcionários

---

Feito o passo anterior, é hora de fazer as análises de horas dos funcionários e corrigir inconsistências.

>Para isso, volte uma pasta e abra o arquivo `Movimento Apontamento Produção Cálculos`:
>
>![alt text](./Midia/movimentoApontamentoProduçãoCálculos.png?raw=true)

>Na aba dados clique em atualizar tudo 
>
>![alt text](./Midia/atualizarTudo.png?raw=true)

Existem 3 planilhas dentro dessa pasta do Excel:

## 9.6.1. Apontamento Produção Dados

---

>Essa planilha é simples:
>* Calcula o total de horas extras trabalhadas. 
>* Se o motivo da hora improdutiva for `Férias`, o total de horas é alterado para 0.
>
>![alt text](./Midia/apontamentoProducaoDados.png?raw=true)

Em resumo, é um espelho do EGIS.

## 9.6.2. Apontamento Produção Cálculos

![alt text](./Midia/apontamentoProducaoCalculos.png?raw=true)

>Na primeira parte dessa planilha tem a contagem de funcionários por célula e por Coordenador.
>
>![alt text](./Midia/contagemFuncionarios.png?raw=true)

>Logo abaixo tem uma tabela dinâmica que serve para auxiliar na conferência da integridade dos dados do EGIS que estão na planilha da seção anterior `Apontamento Produção Cálculos.`
>
>![alt text](./Midia/dinamicaApontamento.png?raw=true)

>A tabela funciona da seguinte maneira. Ela traz um resumo por setor, do total de horas que um funcionário trabalhou em um dia. 
>* **Esse total de horas não pode ser maior nem menor que `8,8` horas.** Caso esteja assim, a célula ao lado irá ficar vermelha e a coluna `Horas Erradas` irá notificar.
>
>* A coluna `Contagem Funcionários` irá contar quantos valores tem na coluna `Operador` e irá comparar com o total de funcionários daquele setor, que está na parte superior da planilha, conforme imagem acima. Se tiver um valor diferente, irá ficar vermelho
>
>* A Coluna `Contagem de Trabalhadores` irá contar a quantos valores tem na coluna `Soma de Total Horas Trabalhadas`. Essa coluna é importante para uma outra planilha que veremos a seguir.
>
>![alt text](./Midia/dinamicaApontamentoExpandida.png?raw=true)

Se algum dado estiver errado. Procure o erro no lançamento que foi feito no EGIS na seção [9.2.3. Módulo de PCP](). 

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Se der uma hora a mais ou a menos, pode ser o bug de ter lançado o intervalo por último.
</div>

## 9.6.3. Disponibilidade de Fábrica

Essa planilha serve para conferirmos se tanto o DashBoard, quanto a planilha de `Movimento Apontamento Produção Dados` está correto.

Crie uma pasta dentro dessa planilha para cada dia Mês do ano. Nas linhas, exclua os dias que são feriados, ou finais de semana, incluindo sábado.

>Na planilha de `Movimento Apontamento Produção Cálculos` existem 3 setores de montagem. Porém na planilha de `Disponibilidade de fábrica` existe apenas 1. Nesse caso, na planilha de `Apontamento Produção Dados`, renomeie todos os setores `Montagem [setor]` para `Montagem` apenas. 
>
>![alt text](./Midia/renomearSetores.png?raw=true)
>
>Clique com o botão direito na tabela dinâmica na planilha `Apontamento Produção Cálculos` e atualize. 
>
>![alt text](./Midia/atualizarDinamica.png?raw=true)

<div style="border-left: 4px solid #2ECC71; padding-left: 10px; background-color: rgba(46, 204, 113, 0.1)">

<p style="color: #27AE60"><img src="./Midia/Tip.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>TIP</b></p>

Ao clicar em atualizar tudo no menu superior, a planilha `Apontamento Produção Dados` irá retornar aos valores originais, separando cada setor de montagem novamente. 
</div>

>Na planilha `Movimento Apontamento Produção Dados` copie a coluna `Contagem de Trabalhadores` de cada célula e preencha na coluna `Homens` dessa planilha.
>
>![alt text](./Midia/disponibilidadeDeFábrica.png?raw=true)



>O total tem que estar igual o total de horas de horas nas duas planilhas.
>
>![alt text](./Midia/compararTotalDeHoras.png?raw=true)

## 9.6.4. Dashboard

---

Tendo corrigido todas as ocorrências do EGIS, é hora de migrar os dados para o DashBoard.

>Dentro da planilha `Movimento Apontamento Produção Cálculos`, acesse a pasta `DashBoard Cálculos`
>
>![alt text](./Midia/dashBoardCalculos.png?raw=true)

Essa planilha faz o seguinte:
* Adiciona uma coluna chamada `Hora 2`, que identifica se na primeira coluna `Identificação` tem `PV, OP, Férias` ou `Estoque` e traz o valor `Hora Produtiva`, se não traz o valor `Hora Improdutiva`.
* Nas células que estão em branco na coluna `Horas` insere o valor `Hora Produtiva`
* Nas células que estão em branco na coluna `Identificação` insere o valor da coluna `Hora`.

>Clique em cima do Nº 2 da segunda linha da tabela e no teclado tecle `Ctrl+Shift+Seta para baixo` pra selecionar todas as linhas da tabela e copie.
>
>![alt text](./Midia/selecionarTabela.png?raw=true)

>No caminho `N:\Indicadores` abra o arquivo `Dashboard_Produção-[Mês]-[Ano]`
>
>![alt text](./Midia/dashProducao.png?raw=true)

>Na última linha da planilha, clique com o botão esquerdo do mouse, depois clique com o direito para abrir o menu de opções e então selecione `Inserir células copiadas` para inserir as células no **meio** da tabela.
>
>![alt text](./Midia/inserirCelulas.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/Warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

As células **devem** ser inseridas no **meio** da tabela, não no final, se não os dados não serão entendidos como parte da tabela e não serão calculados.
</div>

>Ao fazer isso a planilha será inserida porém fora de formatação
>
>![alt text](./Midia/formatacaoDash.png?raw=true)
>
>Para corrigir isso:
>1. Clique no Nº de alguma linha acima
>2. Tecle `Ctrl+Shift+Seta para baixo`
>
>![alt text](./Midia/corrigirFormatacaoDash.png?raw=true)

>Na aba dados clique em atualizar tudo 
>
>![alt text](./Midia/atualizarTudo.png?raw=true)

>1. Selecione o mês desejado.
>2. Selecione cada setor no dash.
>3. Verifique se a soma do percentual das horas é igual à 100% e se a soma das `Horas Produtiva` e `Horas Improdutiva` é igual as `Horas Totais`
>
>![alt text](./Midia/verificarDash.png?raw=true)

>Copie o valor de `Horas Produtiva` e `Horas Improdutiva` e cole na planilha de `Disponibilidade de Fábrica` conforme cada setor
>
>![alt text](./Midia/totalHorasDash.png?raw=true)
>
>![alt text](./Midia/igualdadeHorasDash.png?raw=true)

## 9.6.5. Apresentação de Horas

>Após o dash ter sido feito, entre na pasta `PCP:\Indicadores\Horas_funcionarios` a abra o power point `Apresentação de Horas`
>
>![alt text](./Midia/apresentaçãoHoras.png?raw=true)

>substitua as imagens da apresentação por novas extraídas do dashboard.
>
>![alt text](./Midia/imageApresentaçãoHoras.png?raw=true)

<div style="border-left: 4px solid #f1c40f; padding-left: 10px; background-color: rgba(241, 196, 15, 0.1);">

<p style="color: #B8860B"><img src="./Midia/warning.png?raw=true" alt="alt text" style="vertical-align: middle; height: 18px; margin-right: 5px;"><b>WARNING</b></p>

Imprima em folha colorida e pendure no quadro em frente a sala da qualidade.
</div>

# 10.Rotinas

1. Fazer o relatório de CD e PC (Consulta dinâmica). Enviar o CD no grupo do PCP e o PC por email. Conforme: [7.7. CD](#).
2. Abrir PVs no EGIS e PCP em carga. Se for lamor, verificar com os responsáveis pela Lamor.
3. Atualizar pedidos de compra no Hailer [7.8. SC sem RC
](#).
4. Verificar se recebemos itens fundidos para enviar para usinagem.
5. Corrigir a observação dos itens com MP OK ou não no módulo de produção em carga, conforme [7.9 100% Recebido](#79-100-recebido) e [7.10 !=100% Recebido](#710-100-recebido).
6. Fazer planilha de itens aguardando coleta para o responsável pela embalagem.
7. Nas segundas feiras, após a reunião do bom dia, fazer as folhas de acompanhamento para os coordenares da produção.