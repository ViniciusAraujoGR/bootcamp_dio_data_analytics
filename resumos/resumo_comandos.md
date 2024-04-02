
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

## 🛜 COMANDOS REPO LOCAL & REPO REMOTO 

| COMANDOS  | UTILIDADE |
|-----------|-----------|
| __git remote add origin__ url | Conecta o repo remoto com o repo local
| __git push -u origin main__ | Atualiza o repo remoto com as infromaçãoes do repo local
|__git pull__ | Atualiza as alterações feitas remotamente no repositório local 
| __git checkout -b__ teste | Cria uma nova branch com base no último commit da branch atual/main |
|__git checkout main__ |  Retorna á branch main apartir da branch teste
|__git branch -v__ | Mostra em que commit esta cada branch|
| __git merge teste__ | Mescla a branch teste(onde foi feita alguma alteração) na branch main
|__git branch__ | Visualiza a branhc que estamos e todas as branchs |
|__git branch -d__ teste | Uma vez feita as alterações nas branch teste 
|__git clone url --branch__ teste __--single-branch__ | Clona apenas a branch teste de um repositorio remoto |
|__git stash__| Pesquisar mais sobre
|__git fetch__| Pesquisar mais sobre


Observações: 
- Sepre dar o git pull para atualizar os arquivos locais quando tiv er alteração nos arquivos remotamente
- É possivel codar no Github remotamente, alterando tanto códigos quanto arquivos txt, sempre comitando as mudanças. Parecido com o VSCode.
- Sempre se certificar em qual branch está se trabalhando, chamar as branchs "teste" de feature.
- 





