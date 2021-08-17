

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ***configuração***                                           |                                                              |
| git config --global --list                                   | lista as configurações                                       |
| git config --global user.name "x"                            | configura o nome de usuário                                  |
| git config --global user.email "x"                           | configura o email                                            |
| git config –global core.editor “code --wait”                 | altera o editor para o nomeado entre aspas                   |
| git config --global  --unset core.editor “vim”               | reseta para o editor padrão                                  |
|                                                              |                                                              |
|                                                              |                                                              |
| ***comandos(repositório)***                                  |                                                              |
| git init                                                     | inicia o repositório local                                   |
| git clone x                                                  | clona para o repositório local(colar o link no x)            |
| git commit -m "x'                                            | cria o nome do seu commit(nome no lugar do x)                |
| git push origin x                                            | empurra o projeto(x é o branch atual)                        |
|                                                              |                                                              |
|                                                              |                                                              |
| ***checkout(cria ou alterna branch) verificar o comando stash antes*** |                                                              |
| git checkout x                                               | alterna para o branch x                                      |
| git checkout -b x                                            | cria um novo branch e o torna o atual(x= nome de exemplo)    |
|                                                              |                                                              |
|                                                              |                                                              |
| ***stash(abre, salva, exclui uma lista de arquivos temporários)*** |                                                              |
| git stash                                                    | salva com nome aleatório                                     |
| git stash save "arquivo-salvo"                               | salva os arquivos em uma lista temporária(usar antes do checkout) |
| git stash list                                               | mostra a lista salva                                         |
| git stash pop 1                                              | abre a lista temporária(1 seria a posição da lista)          |
| git stash clear                                              | limpa a lista                                                |
|                                                              |                                                              |
|                                                              |                                                              |
| ***status(mostra ou muda status)***                          |                                                              |
| git status                                                   | mostra os arquivos não salvos                                |
| git status .                                                 | muda o status                                                |
|                                                              |                                                              |
|                                                              |                                                              |
| ***branch(lista, altera, deleta branch)***                   |                                                              |
| branch                                                       | lista todas as branch(branch com * é a atual)                |
| git branch -m x                                              | altera o nome da branch atual para x                         |
| git branch -m antigo novo                                    | altera o nome de outra branch para novo                      |
| git branch -d novo                                           | Deleta uma branch passando o nome dela entre aspas e não estando nela |
|                                                              |                                                              |
|                                                              |                                                              |
| ***merge(junta as branch)***                                 |                                                              |
| git merge x                                                  | une as branch (x é a head)                                   |
|                                                              |                                                              |
|                                                              |                                                              |
| ***log(abre, gera, resume o histórico)***                    |                                                              |
| git log                                                      | gera um relatório de todas as postagens dentro do projeto    |
| git log -oneline                                             | resume o histórico de cada modificação                       |
| git log -graph                                               | mostra ilustrado graficamente                                |
| gitk                                                         | abre a ferramenta gráfica para melhor visualização           |
|                                                              |                                                              |
|                                                              |                                                              |
| ***reset(deleta, retorna commit)***                          |                                                              |
| git reset x                                                  | torna o commit x como principal, e deleta os commits após ele |
| git reset HEAD~1                                             | olhe onde a git head está e se mova uma vez para trás        |
| git reset --soft~1                                           | retorna ao estágio anterior ao commit                        |
| git reset --mixed HEAD~1                                     | deleta o commit atual e Volta para o estado anterior a ele   |
| git reset –hard HEAD~1                                       | deleta o commit atual                                        |
|                                                              |                                                              |
|                                                              |                                                              |
| vim                                                          | abre o editor padrão                                         |
| :q!                                                          | sai do editor                                                |
| git remote -v                                                | lista os repositórios remotos                                |
| git help                                                     | manual de ajuda                                              |
| ctrl+l ou clear                                              | limpa o terminal                                             |
