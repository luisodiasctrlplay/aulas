## Introdução

Seja bem-vindo tripulante para mais uma aula avançada de CSS! Com tudo que você já viu nas aulas anteriores, você está pronto para aprender conceitos avançados e até mais difíceis de CSS, mas que vão lhe ajudar bastante em seus projetos.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/07c02154-68c3-4f46-bd30-e3653f2ffeee-image9.png)

Imagem 01 - Logotipo da linguagem CSS.

## Objetivos

- Aprender sobre Hierarquias em CSS;
- Criar expressões regulares;
- Organizar sites de acordo com _layout_ pré estabelecidos.

- Atividades para casa

A avaliação será utilizada pelo time de pedagógico para melhorar o curso, não esqueça de pedir também para o aluno avaliar a aula

## Hierarquias DOM

Para iniciar essa aula, crie um arquivo CSS, nele configure o tipo de fonte dos textos do escopo da `<body>` para Verdana e os textos do escopo da `<h3>` para Comic Sans MS. Agora, escreva textos em uma página HTML utilizando essas duas _tags_ e tente responder.

Os textos presentes nas duas _tags_ estão com a mesma fonte? Se sua resposta foi “Não”, parabéns! Mas como CSS não formatou os dois textos igualmente? O texto de `<h3>` não estava também dentro do escopo de <body>; Para entender como isso ocorre, você precisa aprender sobre a hierarquia em códigos HTML e CSS.

Os códigos CSS obedecem a hierarquia DOM (_Document Object Model_) das páginas HTML para formatar os elementos de um site. A hierarquia DOM representa páginas em forma de árvores. O DOM é importante, pois é através dele que você acessa os elementos dentro de uma página HTML. Veja um exemplo, de como uma página HTML é transformada em uma “árvore” por meio do DOM nas imagens seguintes.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/2b84d5b6-2bda-4f41-ad9b-1ef4380a7406-image6.png)

Imagem 02 - Exemplo de documento HTML.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/9b0ac7dc-92db-4e20-ae4b-f0b5724b9dc5-image4.jpg)

Imagem 03 - Árvore da Imagem 02 gerada por meio da hierarquia DOM.

**Obs**: Criar árvores como a da Imagem 02 é um bom modo para visualizar grandes códigos-fonte de sites e assim criar planos com uma equipe de desenvolvedores web.

Elementos mais específicos (por exemplo `<p>`) são encontrados na parte de baixo da tabela, enquanto que os elementos mais genéricos (por exemplo <html>) são encontrados no topo da árvore.

A formatação CSS começa pelas “folhas da árvore” (mais específicos) e vai até o “topo da árvore” (mais genéricos). No primeiro exemplo que você fez, a formatação do corpo do arquivo HTML é válida para todos os elementos que não tem outra formatação configurada. O tipo de fonte do texto será Verdana, exceto para os trechos marcados com `<h3>`, que serão formatados com uma fonte tipo Comic Sans MS. Isso porque `<h3>` se localiza em um nível hierárquico DOM abaixo de `<body>`, portanto, sua formatação tem preferência em relação à `<body>`.

Saber utilizar bem a hierarquia DOM pode ser bastante útil para agilizar a produção de códigos e tornar o código até mais simples. Por exemplo, no lugar de configurar cada uma das células de uma tabela, você pode configurar apenas a _tag_ `<table>` e todas as células serão afetadas.

Outro modo para facilitar a formatação é o uso de configurações para padrões recorrentes em seus códigos, comumente chamadas de expressões regulares.

## Expressões regulares

Como o nome indica, as expressões regulares descrevem os padrões (regularidades) de texto em um formato. Ao combinar configurações CSS com expressões regulares, você vai poder selecionar e restringir elementos que desejar aplicar uma determinada formatação.

Geralmente uma expressão regular é formada pelo conjunto operador e valor como indicado na Imagem 04.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/245625e5-14c9-4a3c-a384-3fe309d37c68-image14.jpg)

Imagem 04 - Estrutura genérica de uma expressão regular.

Na tabela a seguir, você pode consultar os operadores mais usados nas expressões regulares, o significado e o efeito de cada um.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/030b7e78-ba5a-47a8-bec9-d68e44043dcb-image10.png)

Tabela 01 - Principais operadores, seus significados e efeitos.

Aqui você vai ver um exemplo de uso de dois operadores. Mas depois irá testar os outros dois, combinado?

## Exatamente igual

Imagine que no seu site, apenas uma imagem deve ser mais redonda que as demais (Imagem 05). Para isso, você deve utilizar o operador de igualdade “=” (Imagem 06).

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/f330ef9a-b2a5-427f-bfd3-f298df845232-image17.jpg)

Imagem 05 - Página HTML com três imagens.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/0a715e8a-d5e1-40d4-946e-481ff3616059-image2.jpg)

Imagem 06 - Apenas a <img> com fonte igual a “img/imagem2.jpg” será formatada.

## Inicia com

Agora, suponha que você dividiu as páginas do seu site em pastas. Dessa forma, poderá criar links coloridos no seu site para cada uma dessas páginas, levando em consideração as pastas criadas.

Como o endereço de cada link vai ser diferente, você pode definir que apenas os endereços que começarem com “pasta1” terão o link da cor verde. Veja como implementar essa solução nas imagens a seguir.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/93ee769a-df17-4b63-aa3e-b362361a341e-image8.jpg)

Imagem 07 - Página com links de endereços diferentes.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/91c69221-d469-4c74-a7ba-4fe8f80338ef-image11.jpg)

Imagem 08 - Apenas os links iniciados com a palavra “pasta1/” serão laranjas e apenas os links iniciados com “pasta3/” serão vermelhos.

## Na prática!

Agora, como combinado, crie exemplos que utilizem os outros operadores (“termina com” e “contém”) . Também compartilhe seus exemplos com seus colegas e o professor.

Tudo isso que você já viu nesta aula serve para facilitar a organização do código-fonte de seus sites. Mas e o visual? A organização visual de um site é conhecida como layout. Assim, criar um bom layout é o primeiro passo para proporcionar ao seu visitante uma melhor navegação e uma experiência mais prazerosa no seu site.

## WebSite Layout

Um site é frequentemente dividido em cabeçalhos, menus, conteúdo e rodapé. Veja um exemplo na tabela a seguir:

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/aca9a675-55dc-40e0-849c-967ea45cdc7a-image7.png)

Tabela 02 - Exemplo de layout.

**Obs**: Você poderia criar vários outros projetos de _layout_ diferentes. No entanto, a estrutura que você viu na Tabela 02, é uma das mais comuns na internet.

Seguindo os próximos passos, você vai poder criar um site com o mesmo _layout_.

## Cabeçalho

Você deve começar pelo cabeçalho. Normalmente, um cabeçalho está localizado na parte superior do site (ou logo abaixo de um menu de navegação superior). Geralmente contém um logotipo ou o nome do site.

Para configurar um cabeçalho, você pode utilizar como seletor a _tag_ `<header>` que você aprendeu na aula sobre HTML5. Na Imagem 09, é feita a formatação de um cabeçalho.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/64f45dd9-f632-434a-8830-76d1e2b90df1-image3.jpg)

Imagem 09 - Formatando um cabeçalho.

## Barra de navegação

Uma barra de navegação contém uma lista de links para ajudar os visitantes a navegar pelo seu site. Para criar uma barra de navegação, você deve primeiramente definir uma classe e configurá-la. No exemplo a seguir, foi criado uma classe .topnav para definir a formatação de barras de navegação que irão aparecer no topo do site.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/aedb9213-953e-4c50-85ab-34967fc09bee-image12.jpg)

Imagem 10 - Configurando uma barra de navegação.

No seu código HTML, crie divisões (`<div>`) da classe .topnav, assim como na Imagem 11.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/27736477-6db3-4f39-9e16-2c005ff2019a-image13.jpg)

Imagem 11 - Exemplo de página HTML com a barra de navegação configurada pelo código CSS da Imagem 10.

## Conteúdo

O layout nesta seção geralmente depende de quem serão os usuários do seu site. Pensando em seus visitantes, você deve definir como eles gostariam de ver o conteúdo do seu site. O layout mais comum é um (ou um combinado) dos seguinte:

- 1 coluna (geralmente por usuários de celulares)
- 2 colunas (geralmente usado para usuários de _tablets_)
- Layout de 3 colunas (usado em desktops)

Nesta aula você vai criar um _layout_ de 3 colunas (Imagem 12) e alterá-lo para um layout de 1 coluna para quando o seu site for acessado em celulares.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/2efd7d24-1432-4ef5-8be2-d1d059fce429-image5.jpg)

Imagem 12 - Cada coluna ocupará 33,33% da tela, logo serão possíveis até três colunas (100%) uma ao lado da outra.

Para criar um layout de 2 colunas, altere a largura para 50%. Para criar um layout de 4 colunas, use 25%, etc. Se seu celular possui largura menor ou igual a 600px, utilize o código da Imagem 12 para adaptar o seu site ao seu dispositivo.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/ceb0828f-526c-4a09-9f30-716d027ccbad-image1.jpg)

Imagem 13 - Adaptando a página para dispositivos com largura menor ou igual a 600px.

**Obs**: Os layouts que se adequam ao dispositivo em que estão sendo exibidos são conhecidos como _layouts_ responsivos. No exemplo, você está criando um layout que será diferente em desktops e celulares.

## Colunas Desiguais

Geralmente, o conteúdo que aparece no centro do seu site é o principal, e deve aparecer maior. Para isso, você deve definir colunas desiguais, de modo que a maior parte do espaço é reservada para o conteúdo principal.

O conteúdo secundário (se houver) é frequentemente usado como uma navegação alternativa ou para especificar informações relevantes para o conteúdo principal. Copie o código da imagem a seguir, e altere as larguras como quiser, porém lembre-se que deve somar 100% no total.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/db4b6bbb-41a2-4026-8194-f0d67bc6fd48-image15.jpg)

Imagem 14 - Configurando colunas desiguais.

## Rodapé

O rodapé é colocado na parte inferior da sua página. Nele, você deve indicar informações como direitos autorais e informações de contato.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpkwbzp2wf.upload/compressed_images/266bd264-f646-4664-a9be-f4fc0e012d46-image16.jpg)

Imagem 15 - Formatando o rodapé.

Lembre-se de salvar os códigos que você desenvolveu hoje. Caso tenha um repositório no Git e essa ferramenta instalada no seu computador, salve o desenvolvimento da aula de hoje através do prompt de comando do computador usando o código abaixo, fornecendo seu usuário e seu diretório como parâmetros.

```
git remote add origin https://github.com/USUÁRIO/DIRETÓRIO.git
git push -u origin master
```

Você também pode usar o GitHub Desktop, caso prefira usar essa interface. Em caso de dúvidas, busque ajuda do seu professor.

Essa foi a sua última aula sobre CSS, na próxima aula você verá o que foi adicionado na versão CSS3. Por isso, é muito importante que você pratique bastante os conceitos aprendidos até aqui. Faça todos os exercícios e o desafio, tentando utilizar o máximo de conceitos de todas as aulas que você teve de CSS.

Até a próxima!!
