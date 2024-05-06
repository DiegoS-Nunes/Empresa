# Guia de operações PCP
---
># 1. Egis
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/d54cd7a0-a9b8-47de-8ba2-cd6eb55b5a30)
>
>Nosso sistema para construção das árvores dos pedido e emissão de requisições.
>
>**Usuário:** Guilherme
>**Senha:** gro0924

## 1.1 Vendas

### 1.1.1 Inserindo um pedido
Assim que o comercial encaminha um pedido por e-mail, deve ser cadastrado no módulo de *Vendas internas* no EGIS para dar continuidade às operações:

>Exemplo de pedido:
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/701b035b-da76-434c-bee2-ed98d0c5afa6)
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/700c0ba8-aab3-403d-970a-e62acb063def)

>Selecione a operação desejada no menu lateral:
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/a846f268-0b7f-4865-b9f8-c3d9a5899620)

>Assim que abrir o menu de pedidos clique em *Cliente* para inserir um novo pedido. 
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/9f5da375-411a-4c67-abca-2d5cbb8bac72)

>[!NOTE]
>Os Nº de pedido são gerados automaticamente em sequência, não é possível escolher eles. Se você estiver precisando cadastrar um pedido com um Nº que não é o maior imediato ao último cadastrado será necessário cadastrar pedidos com cliente e produto genérico para preencher o gap.
> As vezes o EGIS pula um número de pedido. É uma falha sistêmica, quando isso acontecer não tem nada que possamos fazer. Continue cadastrando a partir do número que pulou.

>Na próxima tela clique em CNPJ para procurar o cliente e selecione o que mais parecer com o cliente do pedido.
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/7db16336-dcfc-4cbc-a5eb-32f03bdc9390)

>Se não tiver o cliente cadastrado clique em *inserir* no canto inferior esquerdo e preencha os dados do cliente no próximo formulário. Os campos mais importantes são os destacados em vermelho.
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/de50dc9b-ba34-4487-8203-a9c475c814e1) 
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/5f5494f8-bded-4694-abb8-e730b135e40b)

>Feito isso, um novo Nº de PV será gerado e voce poderá inserir os itens do pedido.
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/cb036c33-3221-4a51-a834-49ce58eeeca7)

>No final clique me gravar e saia do módulo!
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/09ac8047-1c4e-4d3c-a05b-f5492cce1817)

### 1.1.2 Alterando um pedido
>Para alterar um pedido é só acessá-lo através de menu de pesquisa e alterar seus dados.
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/b94d7c7a-f87b-4856-84de-919abb290fad)

>Para alterar o cliente de um pedido será necessário acessar um menu diferente. Feche o módulo *Pedido de vendas* permanecendo apenas no módulo de *Vendas Internas* e selecione o módulo de alteração de cliente no menu esquerdo.
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/305dc57d-5fce-4fe0-877f-2e266a1e13f8)

>Na próxima tela selecione o tipo *Pedido de Venda* insira o número e em *Cliente* clique nos 3 pontos para selecionar o cliente e siga os passos de cadastro de cliente explicados anteriormente no item 1.1.1
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/46f27708-85c6-4d70-bca9-b2f9cf741995)

## 1.2 Engenharia

Todos os pedidos precisam ser engenheirados (ter desenho e lista de materiais) exceto itens padrões da lamor, tais como os abaixo:

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/e70efb5e-32f6-4b3e-8df2-317521f88a9f)

Mas, **engenheirados ou não**, todos os itens precisam ter uma árvore no EGIS onde será feito requisição interna para retirá-los do estoque, ou de compra. Essa árvore deve ser aberta no módulo de engenharia após ter recebido os documentos da engeharia.

>Módulo de engenharia:
>
>![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/0b79f8a3-4eb6-4ba3-9212-eafcb76668d6) ![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/7a76f0c5-38df-4592-bf91-1921f3b598ad)

### 1.2.1 Explicando a interface

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/f97d09cb-3ca9-488f-af14-de1098be88cd)

### 1.2.2 Colunas
Ao arrastar as colunas para cima ou para baixo você pode remover elas, ao clicar no botão ![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/378114f2-81d0-4ffa-8f95-f1e7faedbcde) no menu inferior um menu lateral é aberto para você poder selecionar quais colunas quer ver.

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/053973fa-c950-44bb-9ce1-eb77fd64065f)

### 1.2.3 Projetos
Na aba de projetos é possível ver os pedidos. Para cadastrar um pedido você deve inicar um projeto conforme o tópico G.

#### 1.2.3.1 Cadastrar Projeto
Para cadastrar um projeto, você deve cadastrá-lo utilizando o menu ![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/ce26bfd7-10b9-420d-aac9-644eb8e38bac). Os campos necessários para cadastrá-lo e o formato padrão para cadastro é:

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/b296cd35-82d1-45ff-8c78-d786c3aa1746)

>Assim que o inserir o item do pedido e pressionar *tab* os dados do cliente e o ***Nome do produto do cliente*** serão preenchidos automaticamente com as informações cadastradas no módulo de vendas. Conforme visto no tópico [### 1.1.1 Inserindo um pedido]. Copie o ***Nome do produto do cliente*** e cole no ***Nome interno*** e no desenho insira o código do item, também pode ser o nome do produto.

>Em ***Projetista responsável*** e ***liberação*** a única mudança que haverá da imagem é o nome do projetista que deverá ser *Josafá* para os itens da *Lamor* e *Rafael* para os demais.

>O ***Centro de Custo*** no rodapé também deve ser *14 - (193) Produção Glass* para itens de bombas, válvulase suas partes. *1 - Aquamec Equipamentos* para itens da aquamec e *27 - LAMOR AMBIENTAL* para os itens da lamor.

### C. Composições
Na aba de composições são subgrupos do projeto, geralmente divididos conforme os *desenhos* ou *listas* da engenharia. Para cadastrar uma composição, você deve estar dentro do ti

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/e094aec2-a0ba-4134-b233-00068dc9bc3a)

### D. Materiais
Na interface de materiais é onde são cadastrados, de fato, todos os itens do projeto.

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/bcf823a3-fab9-4273-8c60-b4314ff07dc5)


### E. Lista
### F. Acompanhamento
### G. Projeto
### H. Composição
### I. Material
### J. Standart
### K. Requisição
### L. Liberação

---
# 2. Sadi

---
# 3.Hailer
Nosso software para gerenciar processos dos pedidos.

# 3.1Módulos
# 3.1.1 PCP em carga
Onde fica todos os PV's desde a abertura até expedição. Nos ajuda a ver em qual fase (Área) do processo o pedido está e qual ação está aguardando.
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/98feefea-576a-4c12-b156-39c4461c6c17)

# 3.2 Como inserir dados no Hailer
Existem duas formas de inserir dados no Hailer:
# 3.2.1 Manual
Clique em ![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/8a1f0626-8f6a-4c5a-b00c-df981d962f9f) e abrirá um menu lateral para você inserir os dados
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/8e942e31-b100-4a3b-a090-c5c890bcc1a5)

A ***Data Cronograma*** será preenchida posteriormente somente pelo supervisor do PCP após ter elaborado o cronograma do pedido.

Na ***Área responsável e Ação*** são inseridos qual etapa do processo se encontra o pedido. Se for um pedido de bombas e válvulas, **sempre** precisará de desenho da engenharia para poder dar continuidade, então a Área responsável será preenchida com *ENGENHARIA* e a ação com *AGUARDANDO DESENHOS*

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/99196de5-f0a9-4ae7-97c0-00b062fd8189)

Para pedidos padrões da Lamor cujo não é necessária a etapa de engenharia, conforme imagem vista no tópico 1.2, será aberto já como *ALMOXARIFADO* e *VERIFICANDO ESTOUE*.

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/358244e6-090d-456e-8187-1445cfac7ae2)

Nas ***Observações*** deverá ser inserido o tipo de frete para o pedido e a transportadora. Essas informações são encontradas no pedido. Se o frete for *FOB* e não tiver transportadora insira como *FRETE: FOB - CLIENTE IRÁ DEFINIR*, caso seja *CIF* e não tiver a transportadora apenas insira *FRETE: CIF*, caso contrário, insira o tipo de frete e o nome da transportadora.

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/e9a120c7-716b-4998-b90e-e59decb7eff6)

***Coordenadores***
> Os coordenadores do módulo PPCP e dos outros são diferentes vide tabela abaixo

|Setores|PPCP|Outros|
|:-------|:----|:------|
|Aquamec|Lucas Azevedo|Se ÁREA = montagem, então é Jean, se ÁREA = Fabricação, então é Wellington|
|Bombas/Válvulas|Lucas Azevedo|Cristiano Sebastião|
|Lamor|Hilton Júnior|Jean Leme|

# 3.2.2 Importando dados
Muito útil para pedidos grandes.
Selecione os seguintes botões
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/978c16b2-8215-470e-aad5-87e3e767af61)

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/42367e0e-7809-4457-a561-43cdd507518a)

Uma planilha, contendo em seu nome a palavra "template", será gerada. Ali você deve preencher com os dados que quer inserir no módulo do Hailer, aqui está um modelo.

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/30c66ead-0128-42c3-8c35-62a355913336)

>[!WARNING]
>Por se tratar de um sistema holandês, nos campos de **data** o único formato aceito pelo Hailer é **"AAAA.MM.DD"**.
>E todos os campos, exceto *valor com impostos* deve ser do tipo texto. Por isso insira o código do pedido com uma aspas simples, se não o excel converterá o código em número.

> [!IMPORTANT]
> Quando haver um pedido grande (com várias linhas) é importante adicionar o valor do IPI em cima do preço total de cada item, para o valor final bater com o valor total do pedido. Para esse processo fica mais fácil importar os dados através do excel.

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/2086857d-a85d-40dd-9896-0b5aa516cd9f)

![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/635dea8e-87f3-4389-95d4-eb1227a7d494)

>[!Tip]
>Não é necessário ter todos os campos preenchidos para poder fazer o upload no hailer e nem todos os campos serão upados mesmo se preenchidos, por exemplo: se existir mais de um cliente cadastrado com o mesmo nome (duplicidade), ou se estiver com o nome errado, o sistema irá upar o campo como vazio. Posteriormente ao upload esses dados poderão ser inseridos em conjunto conforme mostrado na seção 3.2.

### 3.1.2 PCP concluído
Onde fica todos os PV's que já foram atendidos (expedidos)
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/5f6b0f29-d7b5-4e83-bd97-5054c719579e)
### 3.1.3 Follow Up pendentes
Onde fica os itens que controlamos e está pendente de recebimento.
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/8168c8e6-2e42-4a8f-b128-9462e7155d4c)

As informações contidas nesse módulo vem do sistema Sadi (compras)

### 3.1.4 Follow Up recebidos
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/936ae493-01ed-43e9-806a-891caf5ba43c)

### 3.1.5 Ordem de produção em carga
Onde ficam todos os pedidos que estão em produção atualmente.
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/e05b53fc-9df5-42b0-a0d2-ae40aa784a38)

### 3.1.6 Ordem de produção finalizado
Onde ficam todos os pedidos que estavam em produção e foram finalizados.
![image](https://github.com/DiegoS-Nunes/Empresa/assets/161138399/3627373b-a796-4670-af7f-3e89859a768d)

---
# 3.2 Como editar dados no Hailer

---

## Planilha de Análise Hailer
## Rotinas
## Solicitação Costumar (Dona Maria)
## Horas funcionários
### Planilha de Análise Horas Funcionários
## Plano de corte
## Solicitação NF de remessa para industrialização
