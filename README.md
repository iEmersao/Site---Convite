# Site - Convite (Churrascão da Rafa)

Este repositório contém a página de convite para o Churrascão da Rafa. O arquivo principal é `index.html`.

Observações importantes:
- Se quiser música de fundo, adicione um arquivo chamado `samba.mp3` na raiz do repositório ou altere o `src` do elemento `<audio>` no `index.html` para uma URL pública.
- A confirmação de presença é salva localmente (localStorage) no navegador — não há backend.

Como publicar o site (passo a passo):

1) Preparar os arquivos localmente
- Salve `index.html` e `README.md` na pasta do repositório local.

2) Criar/usar a branch gh-pages (opção recomendada para GitHub Pages)
- git checkout -b gh-pages
- git add index.html README.md samba.mp3   # inclua samba.mp3 só se existir
- git commit -m "Publica site: index.html e README"
- git push -u origin gh-pages

3) Ativar GitHub Pages (se necessário)
- No GitHub: vá em Settings → Pages → Source e escolha a branch "gh-pages" (root). Salve.
- Aguarde alguns minutos. O site ficará disponível em:
  https://<seu-usuario>.github.io/<nome-do-repo>/

Alternativa: publicar a partir da branch main
- Se preferir não usar gh-pages, faça commit em `main` e, em Settings → Pages, selecione branch `main` e a pasta `/ (root)` ou `/docs`.

Ferramentas úteis (opcional):
- gh (GitHub CLI): `gh pages` facilita algumas operações se você estiver acostumado com CLI.

Testar localmente:
- Na pasta com `index.html`: `python3 -m http.server 8000`
- Abra: http://localhost:8000

Quer que eu:
- Gere os comandos prontos (em um bloco copiável) para execução local? (já incluídos acima), ou
- Faça o push direto dos arquivos para a branch `gh-pages` do repositório para publicar? Se quiser que eu faça o push, confirme e informe se devo incluir também um arquivo de áudio `samba.mp3` (se estiver disponível) ou usar apenas a index.html.
