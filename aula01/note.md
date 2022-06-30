https://www.youtube.com/watch?v=BAmvmaKQklQ

##### git add 
  * Use o git add para trackear os arquivos. 
  * O git add redireciona os arquivos para o "staging area" 
    - Analogia: Coloca todas alterações dentro de um pacote. (Esse pacote é o commit)
  * git add . adiciona todos os arquivos modificados || git add <nomedoarquivo>

### Commit
  * git commit -m ""
  * É o pacote com as suas alterações. 
    - Analogia: Lacra o pacote com os arquivos alterados. "Estamos fechando um pacote de alterações"

##### git status 
  * Mostra as alterações que foram realizadas nos arquivos. 

##### tree 
  tree .git mostra a árvore da pasta .git

##### checkout 
  * O git checkout -b <nomedaetiqueta/feature> cria uma nova ramificação/branch e migra tal. 

##### gitk
  * O gitk --all mostra em gráfico as ramificações

##### HEAD
  * Faz referência a branch corrente/utilizada.

##### git restore
  * Utilize o git restore --staged <arquivo> para reverter o git add
