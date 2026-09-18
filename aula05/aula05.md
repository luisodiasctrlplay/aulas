## Introdução

Bem-vindo à primeira aula de CSS do Ctrl+Young! Agora suas páginas irão ficar mais bonitas e “cheias de estilo”.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/3445de55-6e00-4121-9424-d48205af9ebf-image9.png)

Imagem 01 - Logotipo da linguagem CSS 3.

## Objetivo

- Aprender noções básicas para personalização do design de uma página _web_.

1 Comentário

---

Lucas Faustino

18/04/2024 às 14:27

**Diferença entre os atributos Id e Class.**

**id**: É um atributo único usado para identificar um único elemento na página da web. Cada id deve ser único e uma página não deve ter dois elementos com o mesmo id. É comumente usado com JavaScript para manipular ou obter dados desse elemento específico.

**class**: Este atributo é usado para identificar vários elementos que compartilham a mesma classe. Uma classe pode ser reutilizada várias vezes na mesma página. É comumente usado com CSS para aplicar estilos a todos os elementos que possuem essa classe específica.

## O que é CSS?

CSS é um conjunto de códigos utilizados para declarar “folhas” de estilos que configuram a formatação e a apresentação dos elementos de uma página HTML.

Com ele é possível definir cores de para textos, fundos, bordas, tamanhos e tipos de fontes, espaçamentos, posicionar blocos, até fazer animações, entre outros.

## Por que usar CSS?

As principais vantagens de usar CSS são:

- O controle e facilidade de manutenção visual do site através de um arquivo externo;
- Aumento da performance e velocidade das páginas. Suas páginas vão abrir mais rápido no navegador, uma vez que os códigos HTML vão ser menores e mais otimizados;
- Possibilidade de elaborar layouts para atender diferentes tipos de dispositivos. Por exemplo, você pode configurar com CSS uma aparência do seu site para celular e outra para computadores.

O nome CSS vem da abreviação de _Cascading Style Sheets_, que em português significa “Folhas de estilo em cascata”, uma vez que as definições de estilo podem ser feitas umas sobre as outras, parecido com uma cascata.

## Escrevendo CSS

A declaração de código CSS pode ser feita dentro de _tags_ e em arquivos HTML, mas é melhor separar os elementos HTML e a formatação do CSS em arquivos diferentes.

Geralmente, um código CSS consiste de uma série de propriedades associadas a um valor cada uma e terminada com ponto e vírgulas (separadores). Essas propriedades são especificadas dentro do bloco de algum seletor. O seletor é uma referência a um ou vários elementos, onde a formatação será aplicada.

Veja na Imagem 02, o formato básico de uma configuração CSS. Cada configuração definida em um código CSS é chamado de “estilo”, por isso, após essa aula, pode-se afirmar que suas páginas ficarão mais estilosas.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/731a94e2-2c1d-4f30-adea-e646603d68e5-image11.jpg)

Imagem 02 - Formato de uma declaração CSS.

Que tal adicionar um pouco de CSS nos seus códigos HTML? No Replit, ao criar um projeto de HTML já são criados os scripts de CSS e JS, inclusive com um _template_ de programação que os conecta entre si, como você viu na sua primeira aula de HTML.

Para referenciar o arquivo CSS no script HTML, é necessário adicionar ao escopo da _tag_ `<head>` a seguinte linha de código:

```
<link href="style.css" rel="stylesheet" type="text/css" />
```

**Obs**: O parâmetro “href” referencia o nome e o local do script de CSS, sendo que caso ambos os arquivos estejam na mesma pasta, basta referenciá-lo apenas pelo nome.

A partir daí, em qualquer _tag_ que você utilizar o atributo id igual ao seletor que você definiu (no caso “textoExemplo”) o escopo dessa _tag_ vai ficar com o formato igual ao definido no arquivo CSS. Veja um exemplo de código HTML (na tag `<p>`) utilizando o estilo definido anteriormente.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/1c740ded-f029-4299-bf74-1969e40223bc-image1.png)

Imagem 03 - Exemplo de código HTML com CSS.

## Formatando elementos HTML

Primeiramente, você precisa definir o seletor do seu estilo. Você pode utilizar um tipo, uma classe de elementos ou um elemento HTML específico, através de identificadores, como um seletor CSS. Nas seções a seguir, você pode ver um exemplo de cada um desses seletores. Depois ficará mais fácil decidir qual será mais útil no seu código.

## Tipo do elemento

Com CSS é possível formatar textos de um tipo de elemento específico (_tags_), como por exemplo a _tag_ `<h1>`. Além disso, é permitido declarar várias _tags_ ao mesmo tempo no seletor, basta separá-las com vírgulas. Na Imagem 04, foi definido que todo texto no escopo das _tags_ `<h1>`, `<h2>` e `<h3>` seria da fonte “Comic Sans MS”, utilizando o atributo _font-family_.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/564d5a8d-04ad-4e02-8502-db9693747826-image5.jpg)

Imagem 04 - O texto nas _tags_ `<h1>`,`<h2>` e `<h3>` estarão na fonte “Comic Sans MS”

## Classe

Se você quiser configurar toda uma classe de elementos HTML, você terá que definir no arquivo HTML e inserir o atributo _class_ na _tag_ que você quer formatar. No arquivo CSS, o nome da classe deve ter um ponto “.” no início do nome no seletor. Na Imagem 05, toda tag com a classe “italicoLinha” vai ter apresentação de fonte em itálico e com uma linha sólida inferior. Já na Imagem 06, uma tag cujo atributo class é igual a “italicoLinha”.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/57d7b69e-f4d4-4978-814b-fb745e6f7fa2-image7.jpg)

Imagem 05 - Classe definida em CSS.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/bc0101c5-cb6e-4e85-b527-e5efda86c68e-image8.jpg)

Imagem 06 - _Tag_ de HTML com a classe definida.

## Identificadores

Para criar uma formatação para um elemento específico (_tag_), você precisa vincular o seletor CSS a um identificador de uma tag HTML, que é declarado usando o atributo id. No arquivo CSS, o identificador deve ser iniciado com um _hashtag_ (#), veja um exemplo na Imagem 07 e o seu uso na Imagem 08.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/8a9f6480-51d0-4910-83d8-0dae59ea67e6-image10.jpg)

Imagem 07 - Configurando um identificador no CSS.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/afbc3024-2ce8-42c1-bb6b-5b5c27614991-image3.jpg)

Imagem 08 - Utilizando o identificador “destaque” em um parágrafo.

**Atenção**: Não é permitida repetição de uma id. Ela deve ser especialmente única para cada elemento. Assim, se você quiser usar a configuração do “destaque” em outros parágrafos no seu texto, você terá que criar um novo seletor para cada um deles (destaque2, destaque3...).

## A tag <div>

Na maioria das vezes, você vai querer colocar estilos em trechos delimitados do seu código HTML. Para definir trechos faça divisões no seu código utilizando a _tag_ `<div>`.

Com essa _tag_, você só vai precisar digitar o id ou a _class_ que você deseja para formatar a divisão feita. Na Imagem 09 e 10 são demonstrados três identificadores sendo utilizados em três divisões diferentes.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/bb26e932-acec-4c0c-b0a6-8a680c5cb48a-image2.jpg)

Imagem 09 - Quatro identificadores no CSS.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/c311a046-3c1a-4a75-bbc4-f645bc18dae9-image6.jpg)

Imagem 10 - Utilizando quatro estilos diferentes na mesma página.

Agora que você já sabe criar estilos e utilizá-los em suas páginas, você vai aprender o formato dos valores utilizados em propriedades do CSS.

## Valores e propriedades no CSS

Existem vários tipos de valores, alguns específicos para certas propriedades. Porém, alguns são de uso comum para muitas propriedades e provavelmente você irá usar em seus projetos. Veja uma lista a seguir:

## Pixels (px)

Muita usada em dimensões de blocos e fontes. Exemplo:

- _**width**_: 100px;
- _**font-size**_: 13px;
- _**height**_: 50px;

## Em

Utilizada para tamanhos de fontes. Seus valores são calculados comparando com a fonte padrão. Assim um elemento com tamanho de fonte de 2em (_font-size_:2em) tem duas vezes o tamanho padrão. Caso o tamanho padrão seja 16 pixels, uma fonte de 2em equivalerá a 32 pixels. Exemplos:

- _**font-size**_: 1.5em;
- _**font-size**_: 3.25em;

## Porcentagens (%)

Ela é relativa ao escopo onde o elemento está contido. Se um escopo tem 100 pixels e for atribuído a outro escopo contido nele uma largura de 50%, equivalerá a 50 pixels.

- _**width**_: 70%;
- _**font-size**_: 120%;

## Hexadecimal

É um sistema de numeração usado no CSS para atribuir valores para propriedades de cor de fontes (_color_), cor de fundo (_background-color_), cor de borda (_border-color_) entre outras. Exemplo:

- _**background-color**_: #cccccc;
- _**color**_: #ffa500;

Neste caso, existe a cor laranja para textos. Lembre-se de sempre iniciar o valor em hexadecimal no CSS com o símbolo “#”.

O valor hexadecimal é formado por três pares de caracteres. A ordem dos pares, da esquerda para direita, representa o sistema de cores RGB (_Red_, _Green_, _Blue_) reproduzindo cores através da variação de cada saturação das cores Vermelha, Verde e Azul.

Algumas vezes é mais fácil utilizar cores através dos nomes delas em inglês, ou utilizando o sistema RGB com número de 0 a 255. Por exemplo:

`_color_:_orange_` equivale a `_color_:#FFA500` ou `_color_: rgb(255,165,0)`.

Tudo pronto! Com o conhecimento adquirido até aqui, você só precisa escolher as propriedades corretas para criar códigos CSS, e assim elaborar sites com aparência mais sofisticadas.

## Principais Propriedades

Existem mais de 200 propriedades em CSS para diferentes situações, tantas que não caberiam nessa aula. Aqui você vai aprender as propriedades mais utilizadas na maioria dos projetos. Desta vez a tabela com os significados está no formato “Nome-Função”.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/8a77dc36-da76-4ce3-90d4-b8ec0bffcc3f-image4.png)

Tabela 01 - Propriedades de CSS: Parte I.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmptxglggpg.upload/compressed_images/b2faf7ae-785b-414b-8ba8-22046272e82c-image12.png)

Tabela 02 - Propriedades de CSS: Parte II.

Lembre-se de salvar os códigos que você desenvolveu hoje. Caso tenha um repositório no Git e essa ferramenta instalada no seu computador, salve o desenvolvimento da aula de hoje através do prompt de comando do computador usando o código abaixo, fornecendo seu usuário e seu diretório como parâmetros.

```
git remote add origin https://github.com/USUÁRIO/DIRETÓRIO.git
git push -u origin master
```

Você também pode usar o GitHub Desktop, caso prefira usar essa interface. Em caso de dúvidas, busque ajuda do seu professor.

Faça todos os exercícios e o desafio, tentando utilizar ao máximo os seletores, propriedades e valores aprendidos. Pois como diria o ditado: a prática leva a perfeição.

Até a próxima!!

O que é o CSS? Conjunto de regras que define o estilo e a aparência de um documento HTML.

A formatação de estilos é aplicada diretamente: As tags da página HTML

A tag <div> é usada para dividir trechos no código para delimitar estilização: Verdadeiro

Para estilizar uma página HTML, você pode usar o CSS para definir estilos para elementos específicos.

```css
body {
  background-color: #f0f0f0;
}
```
