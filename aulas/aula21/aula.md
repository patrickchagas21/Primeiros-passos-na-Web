# Github e hospedagem gratuita Github Pages

Vamos colocar nossa primeira página online, e para isso vamos usar o Github e seu serviço Github Pages como nossa ferramenta. Mas antes, precisamos compreender o que ele é e como funciona.

## Git

Antes de tudo, precisamos versionar nossos arquivos com o Git. Um sistema de controle de versão e gerenciamento de código fonte. Foi desenvolvido por Linus Torvalds, criado inicialmente para o desenvolvimento do Kernel Linux, e é ainda hoje muito usado em diferentes projetos digitais no mundo inteiro.

## Github

Depois precisamos armazenar nosso projeto no Github. Uma plataforma social através da qual milhares de pessoas constroem códigos, entre outras coisas, de forma colaborativa, aberta e gratuita. O Github oferece um espaço para armazenar pastas e arquivos com seu conteúdo versionado através do Git.

>"O Github, é na verdade uma rede social ou uma fábrica social de software, que desenvolve e promove milhares de códigos fontes pré armazenados, para as mais diversas finalidades." Wikipedia

## Github Pages

Então já podemos usar o Github Pages para colocar nossa página online. Ele é um serviço oferecido pelo Github, que permite a criação de páginas na web a partir de projetos que foram armazenados nele.

## Primeiros comandos

Vimos anteriormente que nossos arquivos podem ser versionados com o Git, depois guardados no Github, e então hospedados no Github Pages para ter nossas páginas online.

Agora que já conhecemos o Git e o Github, vamos aprender na prática como eles funcionam!

### Versionando nossos arquivos

Para o sistema do Git, os dados dos nossos arquivos são como conjuntos de fotografias, como se seu sistema estivesse fotografando as alterações que acontecem dentro da nossa pasta, para criar versões de nossos arquivos. Mas como ele faz isso? Bom...

Usamos o comando `git init` para pedir ao git que comece a versionar nossa pasta. Agora, ainda pensando no git como um fotógrafo de nossas alterações, precisamos dizer a ele quais fotografias queremos que ele nos lembre. E pedimos que ele coloque um post-it em um um conjunto de mudanças para que possamos ler depois. Usamos o comando `git add` para que ele saiba que as alteraçõoes que fizemos importam para esse conjunto de dados. Ou seja, pedimos que ele fotografe, depois, que ele dê um nome a essa fotografia atual dos nossos arquivos - chamamos isso de commit. Para essa tarefa, usamos o comando git commit -m "oi! eu sou um comentário e vim te lembrar que você mudou esses arquivos aqui"

### Subindo nossos arquivos para o Github

Agora que já conhecemos os comandos mais básicos no Git, queremos que nossos arquivos sejam armazenados não somente no nosso computador, mas também no Github!

Nossa pasta já existe no computador, mas dentro do Github ainda não. Então, vamos abrir o site e criar um repositório vazio dentro dele. Ainda usando o git, precisamos dizer ao Github que nossa pasta e seus commits existem na nossa máquina e queremos que ela vá também para ele. Usamos o comando `git remote add origin https://github.com/seunome/suapasta.git` para dizer que é essa pasta que vai receber a pasta do nosso computador, ou seja a pasta do github vai estar sincronizada à pasta do seu computador. Depois usamos o comando `git push` para enviar nossos arquivos.

### Criando páginas no Github

Agora nossa pasta já existe no Github e queremos criar uma página dela usando o serviço do Github Pages. Como essa será nossa primeira página, podemos criá-la apenas dando a nossa pasta o nome de seunome.github.io

### Ramificando páginas

O Git tem um recurso maravilhoso chamado Branch, ramo em português. Vamos voltar a pensar no Git como um fotógrafo de alterações! Imagine, agora, que nossas fotografias são frutos de uma árvore e que podem crescer por vários ramos diferentes. Podemos escolher quais ramos queremos que cresçam e podemos dar nomes a eles.

Vamos criar um ramo chamado gh-pages onde crescerão nossos frutinhos, ops! nossas páginas. Usamos o comando `git checkout -b gh-pages` para criar um ramo e mudar para ele ao mesmo tempo, então criamos ou mudamos nossos arquivos como queremos, damos commit, depois damos push para subir ele ao Github.

Agora podemos acessar no navegador seunome.github.io/suapasta e tchanrann! nossa página já está online!
