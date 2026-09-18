# Introdução

Olá, tripulante! Você gostou da primeira aula de CSS? Hoje, você vai aprender a construir configurações especiais e tirar maior proveito de CSS para construir sites cada vez mais bonitos.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/680c816f-7432-4fc9-aa7d-ab406a512379-image18.png)

Imagem 01 - Logotipo da linguagem CSS.

## Objetivo

- Aprender conceitos avançados para formatação de estilos em CSS.

Antes de partir para códigos cada vez mais avançados, é necessário entender que em códigos CSS, essa linguagem é muito poderosa. Com CSS é possível personalizar cada detalhe do seu site!

## Combinadores

Um combinador é um artifício que explica a relação entre dois ou mais seletores simples. Um seletor simples é aquele que se refere a apenas um elemento HTML. Um seletor de CSS pode conter mais de um seletor simples.

Entre os seletores simples, você pode incluir um combinador. Existem quatro combinadores diferentes em CSS: seletor descendente, seletor filho, seletor de irmãos adjacentes, seletor irmão geral.

## Descendentes (espaço)

Em CSS, descendentes são todos os elementos que pertencem ao escopo de um outro elemento. Por exemplo, uma _tag_ `<h2>` declarada dentro do escopo de uma `<table>` é considerada uma descendente dela. Com esse conceito em mente, você pode definir configurações específicas apenas para as _tags_ `<h2>` descendentes de `<table>`, colocando como seletor “table h2”. Veja um exemplo na Imagem 02.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/e21d0d62-dd6f-41ca-a432-da082e8852c8-image1.jpg)

Imagem 02 - `<h2>` é descendente de `<table>`.

Na Imagem 03, você pode ver o código-fonte de uma página que utiliza o estilo definido na Imagem 02. Nela, somente o cabeçalho da tabela está com a letra na cor laranja, pois foi utilizado a _tag_ `<h2>` que é descendente da _tag_ `<table>`, de acordo com o código CSS da Imagem 02.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/1362b233-2cbc-4bb8-a5d6-48f906fe90d6-image8.jpg)

Imagem 03 - Apenas a palavra “Eletrônicos” vai aparecer laranja.

## Filho (>)

O seletor filho seleciona todos os elementos que são os filhos imediatos de um elemento especificado. Se você quiser definir um seletor simples como sendo filho de um outro, utilize o sinal “>”. Na imagem a seguir, são formatados todos as _tags_ `<p>` que são filhos imediatos de uma _tag_ `<div>`:

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/6e9ad02f-3545-4c10-9c68-569d691749c5-image7.jpg)

Imagem 04 - Definindo o seletor “p” como filho do seletor “div”.

Experimente criar uma página com várias _tags_ `<p>` dentro do escopo de uma _tag_ `<div>`. Agora, coloque outras _tags_ `<p>` fora do escopo, como demonstrado na Imagem 05. O que aconteceu? Apenas os parágrafos “filhos” do `<div>` mudaram de cor.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/dfba557d-653f-4cb0-932b-94376f03e51f-image11.jpg)

Imagem 05 - Exemplo de código-fonte HTML utilizando seletores filhos.

Observe que o terceiro parágrafo não é formatado, pois ele não é “filho direto” de `<div>`, na verdade ele é filho de `<center>` e apenas descendente de `<div>`.

## Irmão Adjacente (+)

Adjacente é o elemento que aparece logo em seguida após um elemento usado de referência. Para definir um elemento adjacente a outro, você deve utilizar o sinal “+”. Veja um exemplo de declaração de um elemento adjacente na imagem a seguir e na Imagem 07 um exemplo de uso.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/2c8f4ebd-e2f4-4e6e-b214-b05e50c62fa2-image13.jpg)

Imagem 06 - Definindo a tag <p> como adjacente ao elemento com id=PróximoParágrafo.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/2a44aa69-be66-4948-a1b3-45b86390a686-image10.jpg)

Imagem 07 - Apenas o “Texto 2” será configurado.

## Irmão geral (~)

O seletor irmão geral seleciona todos os elementos que são irmãos de um elemento especificado. São formatados apenas os elementos que forem codificados após o elemento especificado. O exemplo a seguir, seleciona todos as _tags_ `<p>` que são irmãos de `<div>`.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/e9b64c72-eb61-471c-a09a-d1f30e2aa6ab-image2.jpg)

Imagem 08 - Todos as _tags_ `<p>` irmãs de `<div>` terão a cor de fundo verde.

Execute o código da Imagem 09 e veja que só são formatadas as _tags_ `<p>` que ocorrem após o `<div>`.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/e7cbce14-361b-41ce-8c42-b3668b294660-image12.jpg)

Imagem 09 - Apenas os parágrafos 3 e 4 estarão com a cor de fundo verde.

## Pseudo-Classes e Pseudo-Elementos

Outra função interessante que pode deixar o estilo do seu site ainda mais legal é o uso de Pseudo-classes e Pseudo-elementos.

Uma pseudo-classe é usada para definir um estado especial de um elemento. Por exemplo, pode ser usado para:

- Estilizar um elemento quando um usuário passar o mouse sobre ele;
- Colorir links visitados e links não visitados de forma diferente;
- Modificar um elemento quando ele recebe foco.

Já um pseudo-elemento é usado para estilizar partes especificadas de um elemento. Por exemplo, pode ser usado para:

- Mudar a primeira letra ou linha de um elemento;
- Inserir conteúdo antes ou depois do conteúdo de um elemento.

Nessa aula, você vai aprender um exemplo de pseudo-classe e um exemplo de pseudo-elemento. Mas não se preocupe, no final da aula você vai encontrar uma tabela com mais informações para aprender as outras pseudo-classes e pseudo-elementos.

## Pseudo-classe - Hover

Essa formatação vai deixar o seu site com um efeito dinâmico. Ele é aplicado quando o mouse está por cima de um elemento. Experimente adicionar o estilo “_hover_” a um elemento do seu site, por exemplo uma imagem pode ficar preto a branco quando o mouse estiver em cima e ficar colorida novamente quando o mouse sair. Para isso, copie o código da Imagem 10 em um arquivo CSS e depois adicione uma imagem em um código HTML.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/d6dfb239-54e2-4c76-b6c8-26c956c3b1ad-image15.jpg)

Imagem 10 - A imagem vai ficar em preto e branco quando o mouse “passar” por cima.

## Pseudo-elemento - First-letter

Você já deve ter visto em alguns livros, a primeira letra de um parágrafo muito maior que as demais. Para isso, você precisaria formatar apenas a primeira letra de um texto e repetir isso a cada nova página. Para evitar esse trabalho repetitivo, escreva o código da Imagem 11 no seu arquivo CSS.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/59431ca9-2061-4725-9fc6-f014120176dd-image9.jpg)

Imagem 11 - A primeira letra de todo parágrafo será 4 vezes maior que o restante do texto.

Alguns pseudo-elementos são aplicáveis apenas aos elementos do tipo bloco, tais como `<div>`, `<p>` e `<h1>`.

Essa aula vai chegando ao fim, mas antes tente criar em uma página web, utilizando apenas HTML, a tabela da Imagem 12:

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/526f147b-97a5-4790-bd08-ae76d4dae8df-image14.jpg)

Imagem 12 - Tabela zebrada.

## Tabela Zebrada

Tabelas zebradas são muito utilizadas na internet para facilitar a leitura. São tabelas com duas cores de fundo que se alternam de uma linha para outra. Para escrever o código CSS dessa tabela, primeiro imagine que cada linha da tabela tem uma numeração, que começa com o valor 1.

Com isso em mente, utilizando o seletor `nth-child()` aplicado ao seletor tr você pode referenciar uma linha da tabela. Esse seletor é genérico, isto é, para selecionar uma linha específica, basta indicar um número (Imagem 13). Com a palavra “even” você seleciona as linhas pares e com a palavra “odd” as ímpares, veja um exemplo na Imagem 14.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/7edbd1db-5bb3-4bee-a6c9-7a78761bb7c2-image4.jpg)

Imagem 13 - Colorindo uma linha específica (3) em uma tabela.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/6169f051-5cc8-42b5-9cd6-31b8422e3a42-image5.jpg)

Imagem 14 - Colorindo as linhas ímpares (_odd_) e pares (_even_).

**Obs**: Se você não quiser “colorir” a primeira linha da sua tabela, utilize o marcador `<th>` para caracterizá-la como um cabeçalho.

Esse mesmo seletor pode ser utilizado em outros elementos HTML, como em listas (Imagem 15).

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/80e94085-6f91-4153-ab6b-0007ed321ddf-image6.jpg)

Imagem 15 - Em todas as listas, o segundo item vai ser vermelho e todos os itens ímpares serão verdes.

Como você pode ter notado, alguns desses comandos que você acabou de ver são utilizados para formatar elementos específicos. Porém, existem muitos outros seletores para formatações específicas, veja os principais nas tabelas a seguir:

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/1944adc1-ec24-4be0-97d4-2a52c77e1e5b-image16.png)

Tabela 01 - Comandos para formatação: Parte 1

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/3843a36e-7978-4313-ab61-a41d26b1178e-image3.png)

Tabela 02 - Comandos para formatação: Parte 2

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmp6kfnd0t1.upload/compressed_images/f58b4acc-af42-4f78-b37e-cdca24ff3ac5-image17.png)

Tabela 03 - Comandos para formatação: Parte 3

Lembre-se de salvar os códigos que você desenvolveu hoje. Caso tenha um repositório no Git e essa ferramenta instalada no seu computador, salve o desenvolvimento da aula de hoje através do prompt de comando do computador usando o código abaixo, fornecendo seu usuário e seu diretório como parâmetros.

```
git remote add origin https://github.com/USUÁRIO/DIRETÓRIO.git
git push -u origin master
```

Você também pode usar o GitHub Desktop, caso prefira usar essa interface. Em caso de dúvidas, busque ajuda do seu professor.

Você chegou ao fim de mais uma aula cheia de novidades, parabéns! Para fortalecer o que você aprendeu hoje, faça o desafio e os exercícios propostos no material.

Até a próxima!!

---

1 Comentário

---

Lucas Faustino

06/09/2024 às 16:03

```html
<!--Exemplo da tabela do brasileirão:-->

<!DOCTYPE html>
<html>
  <head>
    <title>Hello, World!</title>
    <link rel="stylesheet" href="styles.css" />
    <meta charset="utf-8" />
  </head>

  <style>
    tr:nth-child(1) {
      background: #ff00f7;
    }

    tr:nth-child(even) {
      background: #00ff97;
    }

    tr:nth-child(odd) {
      background: #ff0080;
    }

    body {
      color: gray;
    }

    td {
      text-align: center;
    }

    img {
      width: 32px;
    }

    img:hover {
      width: 64px;
    }
  </style>
  <body>
    <table border="1">
      <tr>
        <th>Posição</th>
        <th>Clubes</th>
        <th>Pontos</th>
      </tr>

      <tr>
        <td>1</td>
        <td>
          <img
            src="https://ssl.gstatic.com/onebox/media/sports/logos/KLDWYp-H8CAOT9H_JgizRg_48x48.png"
          />
          Botafogo
        </td>
        <td>50</td>
      </tr>

      <tr>
        <td>2</td>
        <td>
          <img
            src="https://ssl.gstatic.com/onebox/media/sports/logos/me10ephzRxdj45zVq1Risg_48x48.png"
          />
          Fortaleza
        </td>
        <td>48</td>
      </tr>

      <tr>
        <td>3</td>
        <td>
          <img
            src="https://ssl.gstatic.com/onebox/media/sports/logos/7spurne-xDt2p6C0imYYNA_48x48.png"
          />
          Palmeiras
        </td>
        <td>47</td>
      </tr>
    </table>
  </body>
</html>
```
