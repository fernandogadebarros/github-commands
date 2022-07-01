### Dica para reverter um commit que gerou um bug na master
  * Faça o comando git log --decorate --oneline --graph --all
  * Selecione a hash do commit que está em produção 
  * E utilize o comando git revert <hashDoCommitNaMaster>, 
  * Este comando gera um novo commit sem as alterações do hash e não polui o histórico de commits