# PROMPTS.md — Lições Aprendidas

## Pesquisa OLX — Play 5 / PS5

Data: 2026-10-16
Site: https://www.olx.com.br/
Estado filtrado: São Paulo (SP)

### O que foi feito
- Acessado https://www.olx.com.br/ via Playwright MCP.
- Navegado para a categoria PlayStation 5 em São Paulo.
- Tentado buscar por "Play 5" e "PS5".

### Problemas encontrados
- Nenhum CAPTCHA explícito foi exibido, mas o site apresentou 176+ erros de console (falhas de rede, recursos bloqueados, erros 422) e comportamento instável.
- A página de resultados carregou parcialmente, mas a navegação e a extração de dados foram prejudicadas pela quantidade de erros.
- Não foi possível extrair de forma confiável os 5 primeiros anúncios com título, preço, localização e URL devido à instabilidade.

### Lição aprendida
- Sites de classificados como OLX frequentemente bloqueiam ou limitam scraping automatizado.
- Se houver CAPTCHA ou bloqueio, não tentar contorná-lo; registrar o bloqueio e a limitação.
- Sempre verificar a estabilidade da página (erros de console, carregamento) antes de extrair dados.
- Se a página estiver instável, registrar a tentativa e os problemas observados, sem inventar dados.

### Resultado
- Nenhum arquivo de relatório de produtos foi criado (não inventar dados).
- Nenhum arquivo extra foi gerado além deste registro de lição.
