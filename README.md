<h1 align="center">
  <img src="assets/reprograma-fundos-claros.png" alt="logo reprograma" width="500">
</h1>

# Tema da Aula

Turma Online 20 - Todas em Tech  | Front-end | Semana 2 | 2022 | Professora Jaqueline de Almeida

Bem-vindas a turma 20 do Bootcamp de Front-end do Todas em Tech!
Hoje  vocês vão navegar pelo mundo do HTML e CSS, conhecendo os principais fundamentos.
Vamos juntas, com tranquilidade e muita diversão em três encontros durante esta semana.


### Instruções
Antes de começar, vamos organizar nosso setup.
* Fork esse repositório 
* Clique no botão code
* Abra o seu GitBash
* Digite o comando:


```
     pwd
```
* Entre no seu desktop:
```
     cd desktop
```
* Clone o fork na sua máquina: basta abrir o seu terminal e digitar:
  
```
     git clone url-do-seu-repositorio-forkado
```
* Digite o comando  ls para encontrar o seu repositório:
  
```
     ls
```
* Copie o nome do repositorio e entre na pasta clonada:
  
```
     cd on20-tet-s2-html-css
```
* Crie uma branch com o seu nome:
  
```
     git checkout -b seu-nome
```
* Digite o comando para abrir o projeto no vscode:
  
```
     code .
```

### Resumo aula sábado!
O que veremos na aula de hoje?
* [HTML](#html)
* [CSS](#css)
* [Inspecionar](#Devtools)
* [Documentação](#css)
* [Intervalos: Vamos comer  😋 e beber café! ☕](#intervalos)

     Vamos ter  dois intervalos : 10:30 e 15:00;

     Vamos almoçar às 12:00;

     Voltamos às 13:00.

## Conteúdo

### HTML
[Tags básicas](#tagbasicas)
  
       div, p, h1, script, link

[HTML semântico](#htmlsemantico)
      
      header, nav, footer, main, sections, header, aside

[Links em âncora](#linkancora)
      
      href="#"

[Formulários](#formularios)
      
   form, input, placeholders, checkbox, radiobuttons, buttons

[Tabelas](#tabelas)
      
   thead, tbody, td, th, tr
   
### CSS 

[Diferentes formas de adcionar estilo à página](#folhadeestilo)

   * Tag Style
   * Link para folha de estilo

[Importando fontes externas (ex: Google Fonts)](#googlefonts)

[Método BEM](#metodobem)

    Como nomear as suas classes.

[Seletor](#seletor)

    .class #id elemento atributo 

[Propriedades de Estilo no CSS](#estilocss)

   * Dimensões de elementos (largura, altura) - (width, height)
   * Margens e espaçamentos (margin, padding, border)
   * Fontes e suas cores, famílias, tamanhos e ênfases
   * Cores de fundo, transparências e gradientes
   * Alinhamento de elementos
   * Propriedades display (none, block, inline, inline-block e flex)
   * Propriedade border-box
   * Medidas usadas no CSS (px e %)
   * Sombra


### HTML 

#### O que é? 

HTML é uma abreviação de **Hyper Text Markup Language** (linguagem de marcação em hipertexto). Não é uma linguagem de programação, pois não tem lógica (algoritmos, processos etc). Ele cria a estrutura de uma página ou aplicação web, determinando a separação de layout e seu conteúdo.
Os sites, nos seus primórdios, eram basicamente feitos de html puro!
Bonito #sqn 🙃.

#### Como ganha vida?

Antes de começar a codar, você precisa criar o arquivo html:
    
   * index.htm

Depois, arquivo criado, você inicia com a estrutura básica:

```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
     
```

Quem lembra da música: "cabeça, ombro, joelho e pé?"
É neste flow que o html se estrutura.


##### Meta Tags

Elas servem para você organizar a sua página, mas sem que o usuário veja.

Lá ficam:

   * lang: linguagem que o navegador vai interpretar;
   * charset: indica a formato de codificação de caracteres
   * viewport: indica que a visualização da página é adequada para responsividade;
   * title: titulo da sua página -  aqui consegue ver.

Aqui você ainda inclui o link para o seu css e para fontes. 

##### Tags

Dentro do body, incluimos as tags (etiquetas) que referenciam o conteúdo incluido no html. Exemplo:

```

<p>conteúdo</p>
     
```

Algumas tags precisam ser abertas e fechadas, para que estejam certas, como no exemplo acima.
Outras  são autocontidas, não precisando de tag de fechamento:

```

<img href="">
     
```

##### Tags Básicas

| Tags HMTL   | O que faz?                                                |
| ----------------- | ---------------------------------------------------------------- |
| html, head, body    | Utilizada para definir a relação entre o documento e algum recurso externo (head) |
| link    | Utilizada para definir a relação entre o documento e algum recurso externo (head) |
| meta      |Utilizada para inserir metadados (informaçõe) a respeito de um documento HTML (head) |
| title      | Define  o titulo do documento (head) |
| main     | Representa o conteúdo de maior relevância dentro de uma página (body) |
| header   | Utilizada para representar o cabeçalho do documento (body) |
| nav   | Utilizada para definir um conjunto de links de navegação (body) |
| section   | Utilizada para criar seções dentro de um documento e geralmente contém um título (body) |
| article   | Utilizada para fazer um artigo dentro de um conteúdo, geralmente se utiliza um título e são idependentes (body) |
| div  | tag de divisão (body) |
| a  | Utilizada para inserir links (body) |
| h1 a h6, p  | Tags para definir textos. H1 a h6: Tags para títulos. p: Tag utilizada para inserir parágrafos (body) |
| img  | Utilizada para insetir imagem|
| aside |Seções muitas vezes representadas como barras laterais, relacionado ao conteúdo do seu entorno, que poderia ser considerado separado do conteúdo |

#### Comentários em HTML:

<!-- Isso é um comentário. Comentários em qualquer linguagem são pedaços de código que são ignorados na renderização (na leitura do computador), mas são úteis para entendimento humano -->


#### HTML semântico
   
Semântica é um estudo a respeito do significado/sentido de palavras, frases ou expressões dentro de um contexto. No programação ela está relacionada ao significado de uma parte do código. **EX: Qual a finalidade/função que esse elemento tem no HTML?** O HTML semântico torna as informações de um site bem explicadas para o computador, facilitando o entendimento de leitores de acessibilidade, e ajudando mecanismos de pesquisa  a captarem palavras-chave importantes que identificam a página com mais facilidade, indexando como preferência nas buscas.

![Bloco BEM](https://miro.medium.com/max/3840/1*NjJoYvshr5Jyj4HMu0aXnA.jpeg)


Algumas tag são mais semãnticas do que outras e é importante ficar atenta a elas.


Leia mais aqui: 
- [HTML Semântico: Conheça os elementos semânticos da HTML5](https://www.devmedia.com.br/html-semantico-conheca-os-elementos-semanticos-da-html5/38065) 

#### Identação

⚠️ Identar o código é deixar ele organizado de uma maneira que facilite a sua leitura e de outros desenvolvedores que leiam os eu código. 
Para indentar, segure a linha de código e aperte **tab**.

### CSS

CSS é abreviação de Cascading Style Sheet (folha de estilos em cascata). É a linguagem que define estilos para o HTML, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração hierarquia dos seletores. É de cima para baixo! 󠁢

Há três formas para incluir o código CSS em um documento HTML: 

*  Interno 

```
<p style="color: blue">Parágrafo com fonte azul.</p>
<p>Esse outro parágrafo não é azul, a não ser que
exista <span style="color: red">CSS em outro lugar</span>.</p>

```
*  Interno
```
<head>
  <style type="text/css">
    seletor { propriedade: valor; }
  </style>
</head>

```

* Link externo

```

<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="css/style.css" />
  </head>
</html>

```

Dentro do arquivo .css, a anatomia é:

```
seletor {
  propriedade: valor;
}
Exemplo:

p {
  color: red;
}

```

#### Comentários em CSS:

```
/* Sou um comentário CSS */
```

### Seletores


Classes e ids são atributos que podem ser inseridos em qualquer tag dentro da tag body. Eles são atributos de nomeação, sendo class muito usada para referência em CSS e id para Javascript, mas o id também pode ser utilizado no CSS quando você quer estilizar um conteúdo de html muito especifico. Uma diferença entre os dois é que podem haver várias classes com o mesmo valor, ao passo que ids devem ser únicos.


* Classes : chamadas com ponto no CSS.
``` 
 <section class="titulo-principal">

```

* Id : chamadas  com  hastag 
``` 
 <section id="imagens-centrais">
 
```

* Elemento : chamando o elemento/tag  direto no CSS.
  
```
<img>
  
```

* Atributo: incluindo a tag +  o atributo entre parênteses : 
  
```
a[href]
  
```

#### Pseudo-classes
   
* Dinâmica: controlam o estado do elemento
```
:hover
  
```

* Estruturais: seleciona um elemento da estrutura do código 
  
```
:firs-child
  
```

#### Principais propriedades

| Propriedades CSS  |                                               |
| ----------------- | ---------------------------------------------------------------- |
| background | background-imagem, backgroun-color |
| text  | text-align, font-family, font-size, text-decoration, font-size, text-transform|
| layout  | width, margin, padding, display(inline-block, lex, block|
| cor | color|
| decoração  | box-shadow, border|

### Método BEM

A sigla BEM significa block, element, modifier, que são os três pilares do método BEM. É uma metodologia de criação de nomes para classes, tornando esse processo mais prático, lógico, e rápido. 
"O BEM ajuda o desenvolvedor a criar pedaços reutilizáveis do códido, tornando o processo de nomeação no HTML e CSS mais prático lógico e rápido." Bruna Gil
Ele facilita o entendimento da hierarquia e ação do código, criando um padrão.

Vamos facilitar a vida, né?

![Bloco BEM](https://miro.medium.com/max/1276/1*xHJeNZlLtdFkjMMIL1z4Ag.jpeg)

#### Esquema de nomenclatura

```
 bloco__elemento_modificado-nome_modificador-valor

```
Nomes em letras latinas minúsculas.

Palavras são separadas por um hífen (-).

```
.titulo-principal

```

O nome do bloco e o nome do elemento são separados por dois underlines (__).

```
.header__logo { } 
.header__imagem { }
.header__pesquisar { }
.header__menu { }

<form class= "search-form">  
    <input class="search-form__input">
  
    <button class="search-form__button">Pesquisar</button> 
</form>

```
O modificador é separado do nome do bloco ou elemento por um único sublinhado (_).

```
.header__navigation { }
  .header__navigation_secondary { }
  .header__navigation_primary { }

```

O valor do modificador é separado do nome do modificador por um único sublinhado (_).


####  Bloco

 * É único e independente
 * Não deve haver dois ou mais blocos com mesmo nome
 * É o primeiro componente a ser idealizado e construído,    carregando consigo os comportamentos e estilos mais genéricos
 * O bloco pode conter elementos ou outros blocos.

![Bloco BEM](https://miro.medium.com/max/1400/1*FJsBKkys_xtJZ2yjA3pt3g.png)

![Bloco BEM](https://miro.medium.com/max/1400/0*yFWW8Q1c6XvZA-ka)

![Bloco BEM](https://miro.medium.com/max/1400/0*lhehYflLEwB0wecm)

#### Elemento

* Está diretamente atrelado a um Bloco.
* Não pode ser utilizado sem um Bloco.
* Depende de outras estruturas no código para “existir”
* Vamos dar uma olhada nesse outro exemplo de código.

![Elemento BEM](https://miro.medium.com/max/1026/1*4Oo7l0npbVwwX49UZwjb1A.png)


Na imagem abaixo, temos um formulário (form) que é um bloco com dois  elementos **input** e **buttton**

![Elemento BEM](https://miro.medium.com/max/960/1*fd5k2iTaHF5wGVC34FO57A.png)

```
<form class= "search-form">  
    <input class="search-form__input">
  
    <button class="search-form__button">Pesquisar</button> 
</form>

```

#### Modificador

* É opcional.
* Pode estar atrelado tanto a um Bloco como a um Elemento.
* Carrega caraterísticas específicas de aparência, estado ou comportamento (“Como esse bloco é? O que esse elemento faz?”)
* Um de seus principais usos é quando temos blocos ou elementos com estruturas iguais, mas com estilos ou estados diferentes.

![Modificador BEM](https://miro.medium.com/max/1400/1*Be8gwK9LectPUvHI0c1z3Q.png)

#### Nomenclaturas alternativas

* Tracinhos (--)
```
nome-do-bloco__nome-do-elemento--modificador
```

* Estilo CamelCase (inicia com a letra minúscula)

```
blockName-elemName_modName_modVal
```

* Estilo React (inicia com a letra maíuscula)
```
BlockName-ElemName_modName_modVal
```

Você pode montar um próprio sistema de nomenclatura, desde que separe a interface em blocos, elementos, modificadores. Ou seja, seguindo a arquitetura do Método BEM.

#### CSS é assim...Respira que vai dá certo

No inicio e no meu do aprendizado de CSS é um pouco como tentativa e erro. Com a prática, vamos acertando para que, ao longo do processo a gente pegue o jeito e seja mais simples e fácil.
Praticar, estudar, pesquisar! Com o tempo você pega o jeito! 

![Modificador BEM](https://media.giphy.com/media/13FrpeVH09Zrb2/giphy.gif)

### Fontes externas

O CSS tem fontes padrões que são utilizadas na construção da página. 
Mas você pode estilizar as fontes através de um link externo adcionado no head do html. 

A ferramenta mais utilizada para esta estilização é  o Google  Fonts:

[Google Fonts](https://fonts.google.com/)


### Dev Tools

Dá um crtl + f12 e vamos embora!
O Devtools é uma ferramenta do navegador que permite a inspeção do código. 
Com ele você consegue verificar o html e css de qualquer página.
Você pode ver as aplicações do código, copiar (sim!, é possivel), mas também ter como inspiração para a sua página.
Ali também você pode fazer alterações para verificar como fica a aplicação na sua página e depois aplicar no seu código.

⚠️O navegador mais recomendado para esta inspeção é o Google Crohme. 

### Documentação

A leitura da documentação é essencial para o aprendizado de HTML e CSS.
A documentação te auxilia a tirar dúvidas, corrigir bugs/erros e trazer novos elementos no seu código.
 
A documentação mais famosa é a da Mozilla. 

[Documentação HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[Documentação CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS)

E ainda tem o W3 Schools que é responsável pelo HTML e CSS.

[W3 Schools](https://www.w3schools.com/)

### Resumo aula de quarta-feira!
O que veremos na aula de hoje?
* [Revisão](#revisao)
* [Formulário](#formulário)
* [Dúvidas](#duvidas)
* [Intervalo: Vamos beber água  🥤e  tomar café! ☕](#intervalo)

  Vamos ter  um intervalo de 10 minutos às 20:30.

#### Formulário 

Um formulário no HTML é representado pela tag form:

```
<form> Esta é uma tag de formulário </form>
```

Esta tag pode receber alguns atributos específicos como o atributo method, que vai definir o método HTTP com que o formulário HTML irá lidar, que pode ser o método Get ou Post. Recebe tbm o atributo action que através de uma URL, vai definir o local para onde serão enviados os dados recolhidos nos formulários.

```
<form method="post" action="/receber_dados.php">
...
</form>

```

|Tags Formulário |                                               |
| ----------------- | ---------------------------------------------------------------- |
| input | Campo de entrada onde o usuário pode inserir dado |
| label  | Tag de rótulo/legenda para um campo do form|
| textarea  | Campo de entrada para texto de várias linhas| 
| fildset | Define um grupo de campos|
| legend  | Título para um conjunto de campos|
| select  | Define uma lista de opções selecionáveis|
| option | Define cada opção dentro do select|


![Formulário](https://user-images.githubusercontent.com/77210732/130660579-6aa98045-fc21-4186-809b-09eaeeb3c8b9.png)

![Formulário](https://user-images.githubusercontent.com/77210732/130661691-72032d9b-81e8-405b-ae17-a550be4ab6dc.png)
***
### Exercícios 

* [Exercicio para casa](https://github.com/reprograma/on20-tet-s2-html-css/tree/main/exercicios/para-casa)
* [Exercicio para sala](https://github.com/reprograma/on20-tet-s2-html-css/tree/main/exercicios/para-sala)


### Material da aula 

### Links Úteis
- [HTML // Dicionário do Programador](https://www.youtube.com/watch?v=4dQtz1PpY9A)
- [CSS (Cascading Style Sheets)// Dicionário do Programador](https://www.youtube.com/watch?v=229xfk3EEM8)
- [Guia HTML para iniciantes](https://www.devmedia.com.br/html-basico-codigos-html/16596)
- [Do Zero a iniciante CSS](https://www.ninjadevspace.com.br/post/do-zero-a-iniciante-css-properties)
- [Dicas de CSS para iniciantes](https://eufacoprogramas.com/dicas-de-css-para-iniciantes/)
- [Organizando seu código: O que é Método BEM e como utilizá-lo?](https://medium.com/reprogramabr/organizando-seu-c%C3%B3digo-o-que-%C3%A9-m%C3%A9todo-bem-e-como-utiliz%C3%A1-lo-89f1664af295)
- [HTML Semântico](https://www.devmedia.com.br/html-semantico-conheca-os-elementos-semanticos-da-html5/38065/)
- [Tutorial Formulário HTML](https://tutorialehtml.com/pt/html-tutorial-criacao-formularios/)
- [Seletores CSS](https://www.devmedia.com.br/css-seletores/40729)
- [Box Sizing e Box Model](https://www.alura.com.br/artigos/entendendo-como-funciona-box-model-e-o-box-sizing)
- [Flexbox Guia Completo](https://origamid.com/projetos/flexbox-guia-completo/)
- [Flexbox CSS Guia Completo](https://www.alura.com.br/artigos/css-guia-do-flexbox)

#### Já que é para estudar...

- [Seletores do CSS Pseudo Classes](https://imasters.com.br/css/seletores-do-css-pseudo-classes)
- [Os principais atributos CSS](https://eufacoprogramas.com/os-principais-atributos-css/)


#### Material Complementar - em Vídeo 
- [Aulas CSS - Marco Bruno](https://www.youtube.com/watch?v=kU8oIbe5hLs&list=PLirko8T4cEmx5eBb1-9j6T6Gl4aBtZ_5x&index=10)
- [Aula FlexBox - Rafaela Ballerini](https://www.youtube.com/watch?v=KbjLtEgmZ_E)
- [Representando Cores em Css](https://www.youtube.com/watch?v=uKjKnztS3cY)
- [Aprenda CSS Position em 10 minutos](https://www.youtube.com/watch?v=zPlt84S1L0U)



<p align="center">
Desenvolvido com :purple_heart: 
</p>

