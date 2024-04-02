
##  ✍️ COMANDOS PARA ALTERAÇÕES E INICALIZAÇÃO

| COMANDOS  | UTILIDADE |
|----------|-----------|
| __git init__ | Primeiro passo para iniciar o repositório git |
| __mkdir__ pasta_exemplo   | Cria uma pasta chamada pasta_exemplo|
| __touch__ arquivo.md | Cria um arquivo .md | 
| __mv__ pasta_exemplo pasta1 | Renomeia pasta_exemplo para pasta1
| __git status__ | Checa se alguma alteração precisa ser feita 
| __git add__ | Adiciona o arquivo ao repositorio git
|  __git commit -m__"commit_exemplo" | Comita as alterações feitas no repositório
| __git log__ | Log de commits realizados no repositório
|__echo__ pasta1/ __> .gitignore__ | Adiciona a pasta1 ao arquivo gitignore onde os arquivos selecionados não serão contabilizados

## 🗑️ COMANDOS PARA DESFAZER ALTERAÇÕES
| COMANDOS  | UTILIDADE |
|-----------|-----------|
| __rm -rf .git__ | Remove recursivamente de forma forçada o respositorio git iniciado |
| __git restore__ arquivo.md | Descarta __todas__ as alterações feitas naquele arquivo, retornando ele á origem |
| __git commit --amend__ | Edita no Vim a descrição do último commit feito |
| __git reset  --soft__ hash_commit | As alterações feitas após o commit de destino ainda estarão no índice e no diretório de trabalho, prontas para serem reconfirmadas (re-staged) e recommitidas.
|__git reset --mixed__ hash_commit | As alterações no diretório de trabalho que não são adicionadas ao índice (ou seja, não estão "staged") permanecem no diretório de trabalho como modificações não rastreadas.
|__git reset --hard__ hash_commit | As alterações no diretório de trabalho que não são adicionadas ao índice serão descartadas permanentemente, ou seja, o diretório de trabalho será revertido para o estado do commit especificado.

Observações: 
- Para editar o commit no Vim, primeiro é preciso apertar insert, depois disso editar o nome do commit em cima e para salvar e sair apertar ESC e digitar :wq 
- Desfazer as alterações nos commits devem ser feitas apenas localmente antes do envio para o repositório remoto para evitar conflitos.

## 🛜 COMANDOS REPO LOCAL - REPO REMOTO 

| COMANDOS  | UTILIDADE |
|-----------|-----------|
|