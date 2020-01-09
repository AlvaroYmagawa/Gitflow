# Gitflow
O Gitflow é um design de fluxo de trabalho, que define funções específicas para branches, diz quando essas elas devem interagir entre si e cria versões para seu projeto. Ele é dividido em 2 branches principais, a *master* e a *develop* , e divide operações em branches de recursos que sendo elas *feature*, *release*, *hotfix* e *support*.
* * * 


## Branches principais
As branches principais são fixas no projeto, não devem ser apagadas e servem de histórico do projeto em modo de produção e desenvolvimento.

### master
A branch *master* é seu ambiente de produção, ela deve conter todo código estável de seu projeto.

### develop
A branch *develop* é o ambiente de desenvolvimento de sua equipe, ela sempre será a última versão do seu produto.
* * * 

## Branches de recursos
As branches de recursos são criadas dentro de *develop* e são branches temporárias, onde seu principal objetivo é isolar o desenvolvimento de tarefas específicas, e uma vez que o desenvolvimento da tarefa for concluído essas branches serão mescladas a *develop* e depois apagadas.

### feature
Branches do tipo *feature* são designadas para aprimoramentos/ melhorias do projeto. Após sua finalização ela é mesclada a branch de desenvolvimento(develop).

### realese
Branches do tipo *release* são designadas apenas quando se decide gerar uma nova versão do produto que irá para produção. Ela é responsavél por verificar os códigos vindos da *develop*, mescla-la com a *master* e gerar uma nova versão do seu projeto. 
  
### hotfix
Branches do tipo *hotfix* são designadas para tratar bugs que foram para produção(master). Após sua finalização ela é mesclada a branch de produção(master). ***Obs Essa é a única branch que interagi diretamente com a master, pois ela trata de erros que devem ser corrigidos com maior urgência**``.

### support
Branches do tipo support são designadas para tratar mudanças em versões antigas do seu projeto.
*Obs: Essa funcionalidade ainda está instável, é recomendado não utiliza-la para produção.
* * * 

## Como funciona na prática
  * Instalação
  * Branches de recursos
    * [feature](https://bitbucket.org/yazo-app/gitflow/src/master/Branches%20de%20recursos/Feature/)
    * [release](https://bitbucket.org/yazo-app/gitflow/src/master/Branches%20de%20recursos/Release/)
    * [hotfix](https://bitbucket.org/yazo-app/gitflow/src/master/Branches%20de%20recursos/Hotfix/)