# Sistema de Gerenciamento de Estoque em Python

Este é um sistema de gerenciamento de estoque simples desenvolvido em Python.
Permitindo o cadastro de produtos e categorias, consulta de produtos, realizar movimentações de entrada e saída de itens, consultar relatórios.
Tudo armazenado em um arquivo JSON.

## Funcionalidades

- **Cadastro de categorias:** Adicione novas categorias de produtos, não sendo possível criar caso a categoria já exista.
- **Cadastro de produtos:** Registre novos produtos com detalhes como nome, categoria, quantidade, preço e localização(em caso de setores).
- **Movimentações:** Registrar entradas e saídas de estoque para produtos existentes.
- **Relatórios:** Sendo possível escolher qual é o valor de estoque baixo ou alto.
  - Produtos com estoque baixo.
  - Produtos com excesso de estoque.
- **Consulta de produtos:** Obtenha informações detalhadas de um produto pelo seu ID ou pelo Nome.
- **Histórico de movimentações:** Veja todas as movimentações realizadas para um produto específico.
- **Deletar:**
  - Remova produtos individualmente.
  - Remova categorias inteiras junto com seus produtos.

## Estruturas Principais

- **Produto:** 
  - ID do produto, nome, categoria, quantidade, preço e localização(setor).
- **Categoria:** 
  - Nome da categoria.
- **Movimentação:** 
  - ID da movimentação, ID do produto, tipo de movimentação (entrada ou saída), quantidade e data.

## Armazenamento de Dados

Os dados são salvos em um arquivo JSON chamado `estoque_data.json`, que é carregado automaticamente ao iniciar o programa. Isso garante que as informações do estoque sejam persistentes entre as execuções.

## Como Executar

Certifique-se de ter o Python instalado em seu sistema.
Clone este repositório ou faça o download do código fonte.
Abra o terminal e navegue até o diretório do projeto.
Execute o programa.

# Fluxo de Operações
Ao executar o programa, você verá um menu com as opções abaixo:

```
1: Cadastrar Categoria
2: Cadastrar Produtos
3: Consultar Produto
4: Registrar Entrada
5: Registrar Saída
6: Relatório de Estoque Baixo
7: Relatório de Excesso de Estoque
8: Consultar o Histórico de Movimentação
9: Deletar Produto
10: Deletar Categoria (e todos os produtos presentes nessa categoria)
11: Sair do Programa
```

Basta escolher a operação desejada e seguir as instruções.

## Exemplo de Uso

**Cadastro de Produto:**

```
Digite o id do produto: 1
Digite o nome do produto: Notebook
Digite a categoria do produto: Eletrônicos
Digite a quantidade de itens: 10
Digite o valor do produto: 3500.00
Digite a localização do produto: A1-B3
Produto 'Notebook' cadastrado com sucesso.
```

**Registrar Entrada:**

```
Digite o id do produto que você deseja registrar a movimentação de entrada: 1
Digite a quantidade do produto que você deseja registrar a movimentação de entrada: 5
Entrada de 5 unidades para o produto 'Notebook' registrada.
```
