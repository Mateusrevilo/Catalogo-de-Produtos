# Sistema de Gestão de Produtos

Aplicação web para gerenciar uma lista de produtos, desenvolvida em React com Vite e Tailwind CSS.

## Visão Geral

O sistema permite visualizar, adicionar e excluir produtos. Os itens são exibidos em cards com nome, preço e descrição.

## Tecnologias

- **React 19** — biblioteca para construção da interface
- **Vite 7** — build tool e servidor de desenvolvimento
- **Tailwind CSS 4** — estilização com classes utilitárias

## Estrutura do Projeto

```
src/
├── App.jsx              # Componente raiz
├── main.jsx             # Ponto de entrada da aplicação
├── page/
│   └── Home.jsx         # Página principal (lista e formulário)
└── components/
    └── ProdutoCard.jsx  # Card de exibição de cada produto
```

## Funcionalidades

### Lista de Produtos

- Lista inicial carregada após 1,2 segundos (simulando requisição assíncrona)
- Produtos padrão: Camisa, Calça e Bermuda
- Cada produto exibe: nome, preço e descrição

### Adicionar Produto

- Formulário com campos: Nome, Preço e Descrição
- Novos produtos recebem ID único baseado no timestamp
- São incluídos imediatamente na lista

### Excluir Produto

- Botão "Excluir" em cada card remove o produto da lista

## Modelo de Dados

Cada produto possui:

| Campo    | Tipo   | Descrição                      |
|----------|--------|--------------------------------|
| `id`     | number | Identificador único            |
| `nome`   | string | Nome do produto                |
| `preco`  | number | Preço em reais                 |
| `descricao` | string | Descrição do produto        |

## Como Executar

### Instalação

```bash
npm install
```

### Desenvolvimento

```bash
npm run dev
```

Acesse [http://localhost:5173](http://localhost:5173) no navegador.

### Build para Produção

```bash
npm run build
```

### Preview do Build

```bash
npm run preview
```

## Scripts Disponíveis

| Script   | Descrição                                      |
|----------|------------------------------------------------|
| `npm run dev`    | Inicia servidor de desenvolvimento com HMR     |
| `npm run build`  | Gera build otimizado para produção             |
| `npm run preview`| Servidor local para testar o build             |
| `npm run lint`   | Executa o ESLint no código                     |
