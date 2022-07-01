#### Atualizando o reposiório remoto com o local 

  * Como sincronizar uma branch com o repo remoto? 

  (Com o git pull): o que acontece?
    - Por de baixo dos panos o git pull realiza um git fetch + git merge 
      * O que é o git fetch? 
        - Sua ação é baixar todo o conteúdo do repositório de origem para o repo local, lembrando que baixa somente os conteúdos que o repo local não possui.
      * O git pull salva suas alterações em uma branch origin/master, como se fosse uma duplicata da sua branch local e da branch remota, atualizando a branch remota
      a branch local atualiza em função da remota.

  * Da pra fazer rebase ?
    - git pull --rebase, por de baixo dos panos esse comando realiza um git fetch e um git rebase a partir da branch de origem para a local

  * o git pull origin master  pega todos os conflitos para resolver de uma só vez.
  * o git pull origin master --rebase
  * git rebase --abort || git merge --abort cancela o processo.

  * Quando usar cada um? 
  Merge: quando faz sentido mergear a branch local com a master. Fica declarado no histórico do git onde teve a junção das branchs, se quiser realizar um git revert fica mais 
  fácil do que fosse com rebase.
  Rebase: Mantém um histórico linear, bom para feature branches (Resolve individualmente)
    - As vezes se cair na mesma resolução de conflito com o rebase, utilize a função git rerere que armazena na memória do git os conflitos que já foram resolvidos anteriormente
    caso apareca.
