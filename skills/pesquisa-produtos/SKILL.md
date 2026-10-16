# Skill: Pesquisar Livros no Books to Scrape com Playwright MCP

## Objetivo
Pesquisar livros específicos no site https://books.toscrape.com/ usando Playwright MCP, seguindo uma estratégia obrigatória de busca por título, categoria e paginação.

## Pré-requisitos
- Playwright MCP configurado no VS Code
- Acesso ao site https://books.toscrape.com/

## Passos

### 1. Verificar campo de busca
- Inspecionar a página atual.
- Se existir um campo de busca utilizável, inserir o título exato do livro e submeter.
- Se o livro for encontrado, registrar os dados e parar.
- Se não houver campo de busca, prosseguir para o passo 2.

### 2. Navegar para a categoria mais relevante
- Inspecionar as categorias disponíveis no site.
- Selecionar a categoria mais relevante para o livro (ex.: `Fantasy` para livros de fantasia).
- Abrir a categoria e inspecionar os produtos.
- Se o livro for encontrado, registrar os dados e parar.
- Se não for encontrado, prosseguir para o passo 3.

### 3. Correspondência por similaridade
- Comparar os títulos exibidos com o título solicitado.
- Aceitar correspondências exatas, fortes (mesmas palavras-chave com pequenas diferenças) ou possíveis.
- Se houver uma correspondência forte, abrir a página do produto para verificar.

### 4. Limite de paginação
- Inspecionar até 5 páginas distintas da categoria relevante por livro.
- Se o livro não for encontrado após 5 páginas, registrar como "não encontrado" e listar as páginas inspecionadas.
- Não inspecionar uma sexta página da mesma categoria para o mesmo título.

## Registro de resultados
- Salvar os resultados em um arquivo Markdown (`relatorio-pesquisa.md`).
- Incluir: título, URL, descrição, preço, disponibilidade, avaliações, categoria e páginas inspecionadas.
- Se o livro não for encontrado, registrar claramente como "não encontrado".

## Observações
- Não inventar produtos, preços, descrições ou URLs.
- Não simular navegação; todas as ações devem ser realizadas via Playwright MCP.
- Reutilizar a sessão do navegador existente quando possível.
