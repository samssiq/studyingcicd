# Jenkins - O que é, o que faz e como usar.

 Aqui eu vou documentar todo o meu processo de estudo com o Jenkins (esse é meu primeiro contato com a ferramenta).

### Criando um Job

O passo inicial é criar um job. Isso é feito lá no dashboard, na aba "new item/nova tarefa" -> nomeá-lo -> depois selecionar "freestyle".

Depois é só ir nas configurações, colocar algum trigger (se quiser) e depois colcoar os passo nas execução. Eu coloquei um ```echo "Hello world from Jenkins"```, apliquei, salvei e executei. Tudo certo se o botãozinho ao lado do job estiver verde ;)

#### Jobs parametrizados:

Como o nome diz, são Jobs com parâmetros. Esses parâmteros são acessados através de escolhas e toda a sua manipulação é feita com scripts e seguindo a sintaxe deles.

### Criando uma pipeline

* Diferença entre job e pipeline:


O processo de criação de uma pipeline é bem semelhante ao de um job: Nova tarefa -> nomear oq vai ser feito -> pipeline..

A pipeline é escrita de forma declarativa e tem uma sintaxe própria. O jeito mais fácil de usar uma é com um simples script (o próprio Jenkins fornece um de "Hello World"). 

As pipelines são *statefull*, ou seja: elas guardam o estado do que foi rodado. Isso significa que, caso você rode um código pela primeira vez, tudo o que foi baixado para ele rodar será armazenado e, na segunda vez, a execução dele será bem mais rápida.

#### Scripted pipelines x declarative pipelines
