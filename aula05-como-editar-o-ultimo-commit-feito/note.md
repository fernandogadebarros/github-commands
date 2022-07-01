##### amend 
  * git commit --amend ajuda a reescrever a ultima mensagem do commit que foi realizado. 

##### Para mexer em algum código (git reset)
  * o ideal é desfazer o commit anterior com o git reset --hard <hashDoCommit>
  * git reset ajuda a voltar no histórico de commit
  * Exemplo: git reset --hard 4bac331 || git reset --hard HEAD@{1} || git reset HEAD~1

* As alterações de amend e reset somente fazer na branch em que está trabalhando.