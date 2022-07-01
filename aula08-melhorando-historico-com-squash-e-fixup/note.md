##### Melhorando o histórico de commits com squash e fixup 
  * Sempre que a sua branch estiver acima da master
    * Na master, deixar atualizada. 
    * Na branch <funcionalidadeNova> inserir o comando git rebase -i master

    * Não realizar o git push --force, para o git não ignorar tudo que está na sua branch e subir a alteração com seu histórico local para o servidor , pode pode ocorrer de afetar o trabalho de outras branchs
    * Sempre que realizar o rebase e alterar o histórico de commits, ao invés de utilizar o git push --force utilize o git push --force-with-lease
    * o git push --force-with-lease, este comando é mais seguro pois o git emite warnings caso alguém realizar uma nova implementação na sua branch

##### Como deixar os commits úteis no seu histórico? 
  * É possivel tbm usar o git rebase -i master
  * Mostrará os histórico de commits da sua branch
  * Para mudar o arquivo basta apertar a para digitar e esc + :wq para escrever e sair do arquivo
  * O squash junta o commit que está sempre acima mostra a mensagem para renomear o commit
  * O fixup junta o commit que foi selecionado como fixup junta com o commit de cima e não mostra a mensagem para renomear o commit
  * Ambos os comandos quando gerados, geram uma nova hash para o commit
