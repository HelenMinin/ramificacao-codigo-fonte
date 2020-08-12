# Ramificação do código fonte

### Sobre 
Nessa apresentação, eu irei falar sobre a ramificação do código fonte. Por que utilizar e suas principais dificuldades 
<code><img src="https://user-images.githubusercontent.com/42481661/90053604-1d78ce80-dcb1-11ea-9d45-67eb24527f45.jpg" /></code>
### Os temas tradados serão:
<code><img src="https://user-images.githubusercontent.com/42481661/90053796-59139880-dcb1-11ea-87d2-1347b725ec25.jpg" /></code>

### Mainline
<code><img src="https://user-images.githubusercontent.com/42481661/90053869-721c4980-dcb1-11ea-9cfa-66d6ad5f759b.jpg" /></code>
 Se trata da branch principal na qual se encontra o estado atual do projeto, uma nova implementação sempre se iniciará com base nela e ao final, ela será atualizada com as alterações. A mainline pode receber vários nomes variando de acordo com o projeto versionamento utilizado. O mais comum é o nome utilizado por usuários git: "master"

### Ramificação do fonte
<code><img src="https://user-images.githubusercontent.com/42481661/90053918-819b9280-dcb1-11ea-8db3-e4dd99730c35.jpg" /></code>
 Para responder essa pergunta, precisamos entender como seria a vida de uma equipe de desenvolvedores sem a ramificação de código, na qual todas as alterações são feitas na mainline. E ela seria basicamente assim...

<code><img src="https://user-images.githubusercontent.com/42481661/90053925-83fdec80-dcb1-11ea-8324-163d85d24359.jpg" /></code>
 Todo mundo estaria editando o código ao vivo, mudanças pela metade eram compiladas, as pessoas estariam basicamente pisando umas nas outras. 

<code><img src="https://user-images.githubusercontent.com/42481661/90053926-84968300-dcb1-11ea-8be1-542a1bc08bdf.jpg" /></code>
 Devido a esse problema foi criado a ramificação do fonte que mudou a rotina das equipes de desenvolvimento trazendo independência, segurança, confiança e ilusão ao desenvolvedor. Ao ramificar um fonte, temos a ilusão de tempo congelado, como se fossemos os únicos a editar um fonte, trazendo confiança, segurança e independência. Porém uma hora saimos dessa ilusão e percebemos que as implementações na mainline não param e temos uma conta alta para pagar.
bom, e quem paga?
quando paga?
e qual o valor dessa dívida ?

<code><img src="https://user-images.githubusercontent.com/42481661/90053927-84968300-dcb1-11ea-8c42-08bc4073654d.jpg" /></code>
 Jonny LeRoy, em seu twitter, exemplifica bem como funciona a ramificação de um fonte.
A primeira imagem retrata a expectativa de como as pessoas acham que é a linha de desenvolvimento das branch. Essa imagem é muito utilizada para se explicar ramificação, porém não condiz com a realidade apresentada na segunda imagem, onde podemos ver que a cada ramifiação, mais longe da mainline ficamos.
Uma piada antiga diz que se você cair de um prédio alto, a queda não vai machucá-lo, mas o pouso sim. Com o código-fonte é a mesma coisa: ramificação é fácil, a fusão que é difícil.

### Ramificações de recursos
<code><img src="https://user-images.githubusercontent.com/42481661/90053929-852f1980-dcb1-11ea-987b-458bbaa2824d.jpg" /></code>
 Ao utilizar essa features, você garante que a integração com a mainline só será feita quando o recurso estiver completamente implementado e estável. É importante sempre manter a feature atualizada com a master, mas isso ainda não é uma integração, ao final da implementação a feature volta para a master, fazendo assim, a integração

### Frequência de integração

<code><img src="https://user-images.githubusercontent.com/42481661/90053931-85c7b000-dcb1-11ea-96c5-5a5d2197cfd2.jpg" /></code>
 Existem dois tipos principais de integração com a mainline, a de alta frequência e a de baixa frequência. Mas qual a frequência ideal? 

Integração de baixa frequência:
<code><img src="https://user-images.githubusercontent.com/42481661/90053933-85c7b000-dcb1-11ea-92d7-cf1309898155.jpg" /></code>

Integração de baixa frequência:
<code><img src="https://user-images.githubusercontent.com/42481661/90053934-86604680-dcb1-11ea-9ae7-d768b7dcc8fa.jpg" /></code> 

<code><img src="https://user-images.githubusercontent.com/42481661/90053936-86f8dd00-dcb1-11ea-8122-2e9efd31328c.jpg" /></code>
 Perceba que na integração de baixa frequência, existe um ponto de uma grande integração quando violets recebe o bloco de alterações de scarlet. Essa situação não ocorre na integração de baixa frequência , já que a todo momento violet recebe as alterações de scarlett e vice-versa

<code><img src="https://user-images.githubusercontent.com/42481661/90053937-86f8dd00-dcb1-11ea-8d51-c66be7784716.jpg" /></code>
 Outra situação é em casos de conflitos, perceba que na integração de baixa frequência, o conflito que ocorreu no início da implementação persiste em todo o processo, sendo corrigido apenas quando violet recebe as alterações de violett. Já na integração de alta frequência, o conflito é percebido logo no começo e corrigido, não persistindo durante todo o desenvolvimento.

### Release
<code><img src="https://user-images.githubusercontent.com/42481661/90053938-87917380-dcb1-11ea-9cf0-9657081c873f.jpg" /></code>
 É sempre importante manter a mainline estável e sem erros, pois todos que forem iníciar um novo desenvolvimento deve confiar que irá começar em uma versão estável de desenvolvimento. A mainline estável é o principal principio da entrega contínua.

### Contatos:
<code><img src="https://user-images.githubusercontent.com/42481661/90053939-87917380-dcb1-11ea-8092-9e6a7efffba1.jpg" /></code>

### Referencia: 
https://martinfowler.com/articles/branching-patterns.html#collaboration-branch

https://martinfowler.com/articles/branching-patterns.html#path-to-production

https://martinfowler.com/articles/is-quality-worth-cost.html
