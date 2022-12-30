# Mobile First

# Para entender o que é Mobile First, basta traduzir?

O tema Mobile First tem sido mencionado em diversos lugares em que estou presente, principalmente em entrevistas, e minha resposta sempre foi a mesma: "Mobile First é começar programando para celular HEHE..." essa resposta não está incorreta, porém, está incompleta. Então resolvi estudar o que é Mobile First de fato, e descobri que trata-se de uma filosofia de desenvolvimento. 

Geralmente desenvolvemos um site em sua versão principal para desktop e adaptamos para celular, seguindo a filosofia Mobile First nós desenvolvemos pensando nos usuários mobile, tendo em mente que um celular geralmente tem menos recursos de processamento e rede comparado a um computador. Além da experiência do usuário final, Mobile First traz diversos benefícios para o site, e é sobre isso que iremos conversar nesta publicação.

## Um pouco de teoria

Luke Wroblewski publicou um artigo chamado [Mobile First](http://www.lukew.com/ff/entry.asp?933), onde ele apresenta a ideia que consiste em desenvolver pensando no mobile e adaptar para desktop, não o contrário. O artigo foi publicado em 2009, e a filosofia de desenvolvimento Mobile First foi adotada por diversas empresas como Google, Twitter, Facebook e muitas outras. 

Quando entramos em algum site e nos deparamos com uma montanha de informações e um layout que não se adapta bem no celular, nós facilmente desistimos de continuar navegando neste site, esse é o ponto que Luke queria trazer, nós devemos levar em consideração que o usuário pode estar acessando o site no 3G com 1 pontinho de sinal, com certeza colocar um video 1080p não é uma boa ideia.

Um ponto que o próprio Luke confirmou é que os mecanismos de pesquisa priorizam sites performáticos para mobile e penalizam sites que não são, então se você quer que seu site seja encontrado, você deve desenvolver pensando no mobile.

## OK, entendemos que devemos desenvolver pensando o mobile bonito e performático, mas como podemos fazer isto?

### Utilizando subdomínios

- Muitas empresas estão adotando subdomínios para separar o site mobile do desktop, por exemplo: [m.site.com.br](http://m.site.com.br/), [site.com.br](http://site.com.br/), desta forma você consegue desenvolver o site mobile e desktop separadamente sem precisar se preocupar com o layout do desktop no mobile e vice-versa.

### Utilizando media query

- É interessante utilizar media query para aplicar a filosofia de mobile first. Independente da linguagem que está utilizando, se você consegue implementar css você consegue utilizar media query.

```
  @media (max-width: 600px)
  {
    .facet_sidebar
    {
      display: none;
    }
  }
```

### Utilizando Javascript

- Podemos utilizar javascript para incluir verificações que mostram ou não um componente na versão mobile, ou até mesmo controlar versões de componente, um pensado exclusivamente para mobile e outro para desktop.

## O que ganhamos aplicando essa filosofia?

- Foco em entregar uma ótima experiência para o usuário mobile: Não é novidade para ninguém que a popularidade dos celulares e tablets aumenta a cada ano, garantir para essa galera uma experiência fácíl e ágil com certeza vai fazer ela voltar ou até mesmo compartilhar com alguém.
- Mais simplicidade no projeto: Claro que isso é relativo, porém defendo esse ponto pelo fato de que é muito mais simples adaptar um site mobile para desktop, temos mais recursos de hardware, uma dimensão muito maior, logo isso pode economizar algumas sprints.
- Melhor ranqueamento: Um site acessível para mobile ganha alguns pontos com os mecanismos de pesquisas, dica que o próprio Luke Wroblewski Product Director da Google confirmou em uma talk.

## Conclusão

Mobile fisrt é uma filosofia interessante, claro que não é garantia de um bom desenvolvimento e não é a única opção para o desenvolvimento de um site. Existem alguns fatores a serem considerados para decidir adotar essa filosofia, mas com certeza estudar sobre esse tema nos faz relembrar da importância de se colocar no lugar de todos os tipos de usuários, os que tem uma RTX 3090 32 ram ,ou seja, não irão sofrer quando for perciso carregar um site pesado, porém precisamos pensar naqueles que estão no celular com uma internet extremamente instável.

Os exemplos de implementação que dei estão extramente objetivos, com a intenção de apresentar uma proposta de solução, mas caso queiram discutir mais sobre, fazer uma POC ou até mesmo uma parte 2 deste artigo se aprofundando na prática entre em contato comigo, bora bater uma papo!

Se curtiu o conteúdo ou tem algum feedback deixe aqui embaixo, obrigado e até a próxima 👋🏽.