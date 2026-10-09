## Introdução

Seja muito bem-vindo, tripulante, a mais uma aula do Ctrl+Young 2! Nessa etapa, você irá finalizar sua ficha de personagem, aprendendo como alinhá-la.

Mãos à obra!

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-0faf4126-8538-48a2-98e2-0d8be1114c88.png)

Imagem 01 - Logotipos do HTML5 e do CSS3

## Objetivos

- Conhecer o _display flex_;
- Aprender sobre o funcionamento do _display grid_;
- Finalizar o projeto.

## _Displays_

## O que é _display_

Dentro do estilo CSS, a propriedade _CSS display_ é utilizada para indicar a forma como os elementos HTML serão dispostos na página ou em espaços delimitados. Outra característica dessa propriedade é a facilidade para criar _layouts_ responsivos, que são facilmente adaptados para diferentes tamanhos de tela. Desse modo, o _display_ é um recurso essencial para manter a organização dos elementos na página.

Para entender o que faz a propriedade _display_, é preciso lembrar que existem dois tipos de elementos HTML:

1. **Elemento em bloco (ou _block_):** ocupa 100% da largura disponível e é sempre iniciado em uma nova linha. Alguns exemplos são os títulos, divs e parágrafos, nos quais toda a linha correspondente deve ser reservada a cada elemento mesmo se os seus conteúdos forem apenas uma palavra;
2. **Elementos em linha (ou _inline_):** ocupam apenas o espaço necessário para exibir o seu conteúdo – por exemplo, imagens e _links_.

A propriedade _display_ permite modificar a forma como esses elementos são renderizados, o que permite organizá-los de diferentes maneiras na página HTML.

## _Display Flex_

O valor _CSS display flex_ é utilizado para organizar os elementos HTML de forma responsiva. Na prática, ao definir um elemento com esse valor, ele funciona como um contêiner para agrupar os elementos-filhos, que são considerados _flex-items_ e são organizados nos sentidos horizontal ou vertical.

Em sistemas de RPG que usam regras mais complexas de combate, calculando deslocamento e tamanho de personagens, é comum o uso de um plano em grade, em que os personagens andam para frente, para trás, para os lados e nas diagonais.

Porém, existem também sistemas que usam mapas com células hexagonais, que permitem que os jogadores se locomovam em seis direções diferentes sem precisar calcular o deslocamento na diagonal. Esse padrão é muito usado para tratar de grandes distâncias, como as várias áreas de uma floresta ou bairros de uma grande cidade, mas pode também ser usado para combates.

Ao definir o _display_ como _flex_, pode-se utilizar outras propriedades adicionais para estabelecer como os elementos serão dispostos na página ou em um espaço específico. São elas:

- _**flex-direction**_: tem como função determinar a direção em que os elementos serão dispostos, que pode ser _row_ (linha) ou _column_ (coluna), como também pode ser _row-reverse_ ou _column-reverse_ para exibir os itens na posição invertida;
- _**flex-wrap**_: tem como função definir como o conteúdo de um elemento será exibido dentro do espaço. No caso de texto, por exemplo, ele pode ser forçado a permanecer na mesma linha ou dividido conforme a necessidade. Os valores possíveis são: _nowrap_ (para não quebrar a linha), _wrap_ (para quebrar a linha) e _wrap-reverse_ (conteúdo é preenchido no sentido de baixo para cima);
- _**flex-flow**_: tem como função representar uma forma abreviada de escrever os valores dos atributos _flex-direction_ e _flex-wrap_;
- _**justify-content**_: tem como função indicar como os elementos-filhos serão alinhados horizontalmente no espaço definido como contêiner. Os valores possíveis são: _flex-start_, _flex-end_, _center_, _space-between_, _space-around_ e _space-evenly_;
- _**align-items**_: tem como função representar o alinhamento vertical dos elementos pertencentes ao contêiner. Os valores possíveis são: _flex-start_, _flex-end_, _stretch_, _center_ e _baseline_;
- _**align-content**_: funciona de maneira semelhante ao _align-items_, mas tem como função alinhar o conteúdo verticalmente em relação às linhas.

## _Display Grid_

O _CSS display grid_ permite organizar os elementos da página de forma horizontal e vertical, simultaneamente. Para tanto, ele também conta com uma série de propriedades adicionais, para ajudar a definir como os itens serão dispostos na página ou no espaço disponível.

Basicamente, o _grid_ é formado por um conjunto de linhas e de colunas. Se nada for especificado, os elementos são organizados em bloco, ou seja, um em cada linha. Por esse motivo, é preciso definir outras propriedades para organizar no formato desejado. São elas:

- _**column-gap**_: define o espaço entre as colunas;
- _**row-gap**_: define o espaço entre as linhas;
- _**gap**_: estabelece o mesmo espaço de distanciamento entre linhas (_row-gap_) e colunas (_column-gap_);
- _**grid-area**_: determina a área do elemento, ou seja, quantas linhas e colunas o item ocupará no _grid_;
- _**grid-auto-columns**_: define o valor automático para a coluna;
- _**grid-auto-flow**_: indica o sentido em que os itens serão inseridos automaticamente na grade;
- _**grid-auto-rows**_: define o valor automático para a linha do _grid_;
- _**grid-column-start**_: especifica o início do _grid_;
- _**grid-column-end**_: específica o final do _grid_;
- _**grid-column**_: define a junção das propriedades _grid-column-start_ e _grid-column-end_;
- _**grid-row-gap**_: indica o tamanho do espaço entre as linhas;
- _**grid-column-gap**_: indica o tamanho do espaço entre as colunas do _grid_;
- _**grid-gap**_: representa a junção das propriedades _grid-row-gap_ e _grid-column-gap_;
- _**grid-row-start**_: indica a linha em que o item será posicionado;
- _**grid-row-end**_: indica em que linha será o fim do item;
- _**grid-row**_: representa a união das propriedades _grid-row-start_ e _grid-row-end_;
- _**grid-template**_: representa a união das propriedades _grid-template-rows_, _grid-template-columns_ e _grid-areas_;
- _**grid-template-areas**_: especifica a área do _grid_ com o nome dos itens do _grid_;
- _**grid-template-columns**_: estabelece o tamanho das colunas e a quantidade para o _layout do grid_;
- _**grid-template-rows**_: indica o tamanho das linhas do _grid_.

## Outras propriedades

Além das propriedades mais comuns apresentadas acima, também há:

- _Table_;
- _List-item_;
- _Run-in_;
- _Block_;
- _Inline_:
- _None_;
- _Initial_;
- _Inherit_;
- _Contents_.

## Comunicação

Apesar de CSS parecer uma aplicação que apenas embeleza uma página da _internet_, ele na verdade facilita a comunicação com o usuário, permitindo a este encontrar e interagir com maior facilidade com os elementos da página. Porém, essa comunicação artística não se restringe ao ambiente virtual.

A arte é a forma mais antiga de comunicação do ser humano de que se tem registro, começando pelas artes rupestres em cavernas. Mesmo nos dias atuais, em que a escrita é fundamental para a comunicação, a arte ainda é muito usada para comunicar algo, especialmente informações que precisam ser comunicadas de maneira explícita, como onde está a saída de emergência ou qual botão liga e desliga uma máquina.

Nesse contexto, existe uma ciência chamada **semiótica** que estuda a formação de signos (ou seja, símbolos, linguísticos ou não, que têm significado). Dentro dela, existe a ramificação que estuda a formação de signos através de símbolos pictográficos, chamada semiótica pictórica.

O uso de códigos pictográficos para comunicação é mais comum do que parece. Um exemplo são os sinais de trânsito: uma pessoa caminhando sobre uma faixa listrada representa uma faixa de pedestre, uma seta tortuosa indica um trecho sinuoso da pista e assim por diante.

Indo ainda mais além, há os próprios emojis, largamente usados nas redes sociais, em que desenhos e símbolos representam sentimentos, objetos, comidas e conceitos ainda mais diversos. O uso de vários emojis combinados pode, inclusive, transmitir mensagens complexas, como instruções ou descrição de um acontecimento.

Agora, junto com seu professor, pesquise mais sobre códigos pictográficos e sobre semiótica pictórica. Anote suas descobertas em um bloco de notas, combinado?

## Estilizando o projeto - Index.HTML

Chegou a hora de aplicar tudo o que você aprendeu nesta aula para finalizar o seu projeto!

Comece adicionando as classes às _tags_ do seu arquivo index.html. Começando pela _tag_ `<main>`, no contêiner principal, adicione as classes às _tags_ de cada div, como mostra a imagem 02.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-f7c035bc-374e-49cf-9e4d-5e2608404f96.png)

Imagem 02 - Classes do contêiner principal

Em seguida, faça o mesmo no contêiner vdv-img, adicionando as classes dos contêineres dentro dele.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-7ae03111-4936-4885-bf76-798836a24971.png)

Imagem 03 - Classes do contêiner vdv-img

Para deixar sua página mais completa, adicione mais uma _section_ para exibir informações secundárias sobre o seu personagem, como as suas características físicas e os equipamentos que ele carrega. Em seguida, crie as classes para essa nova seção de conteúdo secundário e para suas divs.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-303bd0f2-4667-4848-8ce0-4f59133554e5.png)

Imagem 04 - Classes do contêiner secundário

Da mesma forma, adicione um _footer_ ao seu código HTML e adicione uma classe a ele. 

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-4258bdad-5d3c-4028-bd20-d86d548b6bbb.png)

Imagem 05 - Classe do rodapé

Em seguida, será programado o código de CSS.

## Estilizando o projeto - Style.CSS

Com as classes adicionadas, será necessário criá-las. Vá até o seu arquivo style.css e crie as classes que você adicionou no seu documento index.html, dando a elas as configurações recomendadas nas imagens abaixo.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-3e1068ca-6a41-413a-96be-4b5f9fe7b390.png)

Imagem 06 - CSS do contêiner principal

Como mostra a imagem 06, você deve aplicar tanto um `display: flex` quanto o _grid_. O _grid_ será usado para criar um _layout_ de três colunas do conteúdo da página. Quanto à parte interna dessas colunas, você usará o _flex_ para organizar o conteúdo em colunas.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-8a4465eb-345c-49dc-a9c7-7db22a55541c.png)

Imagem 07 - CSS dos campos “Vida”, “Defesa” e “Imagem”

Agora, na parte central que irá conter as informações de vida, defesa, velocidade e a imagem do seu personagem, use a classe “`conteiner-vdv-img`” para fazer uma coluna com os campos. Na parte interior dos conteúdos, utilize _display grid_ para que cada informação (vida, defesa e velocidade) fique uma do lado da outra.

Para a imagem, com o _display flex_ é possível alinhá-la ao centro, tanto horizontal quanto verticalmente.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-ee5bd614-ce89-4ab7-99b7-b7f90cc00c5a.png)

Imagem 08 - CSS do campo de “Biografia”

Por fim, no “conteiner-biografia”, faça um `display: flex` para que o título e a área de texto sejam uma coluna.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-e693ead3-b4f4-41c4-ad0d-f732d06b6cf3.png)

Imagem 09 - CSS da seção secundária

A segunda parte do conteúdo da sua página seguirá o mesmo padrão, utilizando _display grid_ para fazer o _layout_. Porém, neste caso, não será necessário usar o _display flex_.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/image-c0eaaa26-8b93-4a64-8210-d8c01f4760e8.png)

Imagem 10 - CSS do _footer_

Para finalizar, falta apenas estilizar o rodapé, aplicando o _display flex_ para que os elementos fiquem lado a lado, removendo a linha sublinhada do _link_ e alterando a cor do fundo. Mãos à obra!

Muito bem, tripulante! Na aula de hoje, você viu diversos comandos para manipular o estilo de elementos de uma página _web_. Na próxima aula, você dará início a uma nova aventura em JavaScript.

Lembre-se de fazer os exercícios e o desafio propostos para a aula, combinado?

Até a próxima!
