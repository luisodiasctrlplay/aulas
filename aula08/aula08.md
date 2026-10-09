## Introdução

Olá tripulante! Nas primeiras aulas, você estudou primeiro a linguagem HTML por inteira para depois ver quais foram as atualizações que vieram com a versão 5, correto? Do mesmo modo, nas últimas aulas você viu a parte fundamental de CSS e agora você vai ver as atualizações trazidas pelo CSS3.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/0f52daf4-d3e3-43dc-a4c2-ec29f04d9a2a-image14.png)

Imagem 01 - Logotipo da linguagem CSS.

## Objetivo

- Aprender novos recursos do CSS3 e quando utilizá-los

Ao longo das últimas aulas, você acabou utilizando propriedades que só foram implementadas na versão CSS3. Logo, você já está fazendo códigos modernos e prontos para grandes projetos.

Porém, nessa aula você vai aprender alguns recursos novos, que vão dar um toque ainda mais profissional a suas páginas. Os dois primeiros são: _border-radius e_ o _box-sizing_, eles vão facilitar bastante o seu trabalho.

## Formatação da Página

## Border-radius

Para você conseguir ver a novidade que a propriedade border-radius pode acrescentar no seu código, inicie criando um código-fonte HTML com um texto no escopo de uma <div>, como no exemplo da Imagem 02.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/371e8291-f44b-4e22-b255-c2f74e1fa050-image11.jpg)

Imagem 02 - Divisão que será configurada como uma “box”.

Agora você vai criar um arquivo CSS para configurar essa “box”. Nela, você pode colocar as propriedades que você já estava utilizando, como _width_ e _height_ (Imagem 03). Abra o código HTML em algum navegador e veja a “caixinha” que se forma ao redor do texto.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/2553a6a7-6ab2-4cc7-9588-dec075485e1e-image12.jpg)

Imagem 03 - Formatação da “box” por meio de CSS.

Porém, para deixar o seu site com um estilo ainda melhor, coloque bordas arredondadas nas caixas utilizando a propriedade _border-radius_ que surgiu apenas na versão 3 do CSS. Se o texto ficar fora da caixa, utilize a propriedade _padding_ para “afastar” o texto das bordas e concentrá-lo no meio da caixa.

Atualize o código CSS que você está produzindo para ele ficar como o código da Imagem 04, e novamente execute o seu site em um navegador.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/30f499e5-86ce-405c-9db4-49324cfe6ac5-image1.jpg)

Imagem 04 - Arredondando bordas com a propriedade _border-radius_ do CSS3.

Também é possível arredondar cada uma das extremidades. Experimente utilizar a propriedade _border-radius_ com os valores “20px 80px” e veja o que acontece, dessa forma: “_border-radius_: 20px 80px;”. Agora, tente definir quatro valores (_border-radius_: 20px 80px 50px 150px;), assim você vai formatar os quatro cantos da caixa.

## Box-sizing

Se você aumentar bastante o valor da propriedade _padding_, vai acabar mudando o tamanho da sua caixa. Para evitar que isso aconteça, utilize a propriedade _box-sizing_ do CSS3 com o valor igual a “_border-box_”. Na Imagem 05, você pode ver um exemplo de um código CSS3 utilizando essa propriedade. Nessa imagem, a caixa gerada vai sempre manter o tamanho definido pelas propriedades _width_ e _height_, mesmo que o padding seja maior, posicionando apenas o texto de acordo com o _padding_.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/adb1a8ac-5fc1-4eb4-b2fc-a4f5b659660a-image7.jpg)

Imagem 05 - Fixando o tamanho da “box” utilizando _box-sizing_.

Um efeito bem legal para o seu site é posicionar textos em frente a imagens, que você pode fazer utilizando a mesma box que você acabou de configurar. Utilize o código da Imagem 06, para adicionar uma imagem de fundo na sua _box_.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/039d0884-1114-4893-9087-55814184a7f6-image2.jpg)

Imagem 06 - Adicionando uma imagem de fundo (_background_) na _box_.

Porém, o seu texto pode ficar escondido pela imagem. Configurar transparências e degradês também ficou mais fácil com o CSS3!

## Efeitos estáticos

## Transparências

Para resolver o problema citado anteriormente, você pode utilizar o valor rgba(r,g,b,alfa) para a propriedade background, onde o r se refere a saturação de cor vermelha que vai aparecer sobre uma a imagem, g é a saturação de verde e b é a saturação de azul. Combinando as três variáveis, você poderá produzir qualquer cor!

Já a variável alfa se refere ao grau de transparência que essas cores irão ter, ela pode variar de 0 (0% transparente) a 1 (100% transparente). Na Imagem 07, o cabeçalho do texto da box terá transparência, além disso, foi inserido uma linha branca em baixo do <h1>.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/31fbae59-ab57-4b06-af55-80f5fa7df242-image15.jpg)

Imagem 07 - Cabeçalho do texto com fundo 80% transparente.

## Degradês

Se você não tiver uma imagem, é possível preencher a box com um degradê entre duas cores, por exemplo, de vermelho para verde como na Imagem 08.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/e5a783cf-a9a5-463f-90f5-26b21b858caf-image9.jpg)

Imagem 08 - Degradê entre a cor vermelha e a cor verde.

Existem dois valores de degradê no CSS3, o _linear-gradient_ e o _radial-gradient_.

### linear-gradient

O _linear-gradient_ por padrão começa de cima para baixo, porém você pode adicionar o parâmetro “_to right_”, “_to left_” ou “_to top_”, para começar pela esquerda, pela direita ou por baixo, respectivamente. Veja um exemplo de um degradê da esquerda para direita na Imagem 09.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/4f6f9e0e-e904-4f7c-81b1-184a03106a04-image6.jpg)

Imagem 09 - Degradê iniciando da direita para a esquerda.

**Obs**: É possível informar os graus de rotação das cores no lugar do parâmetro que você acabou de ler. Experimente utilizar “80deg” no lugar de “_to left_” no código da Imagem 09, para rotacionar as cores em 80 graus.

### radial-gradient

Já o radial-gradient cria circunferências coloridas a partir do centro da box, criando um efeito bastante bonito. Substitua o código da Imagem 09 pelo código da Imagem 10 e veja como são criadas várias circunferências coloridas na sua box. Você pode configurar várias cores, basta separá-las por vírgulas “,”.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/68c10c68-cb30-4b28-96ce-af694745ea95-image3.jpg)

Imagem 10 - Exemplo utilizando gradiente radial.

Você sabia que apenas com sombras, é possível criar efeitos de profundidade em textos? Aprenda a utilizar esse novo recurso do CSS3 e produzir esse efeito profissional em seus sites.

## Sombras

Para criar sombras no seu texto basta utilizar a nova propriedade text-shadow. Nela é necessário definir os seguintes valores:

- **Posição horizontal da sombra** - Definida em pixels, o valor igual a zero fica exatamente embaixo do texto. Para posicionar a sombra mais à esquerda, utilize valores negativos. Para posicionar a sombra mais à direita, utilize valores positivos.
- **Posição vertical da sombra** - Também definida em pixels, quando o valor é igual a zero a sombra fica exatamente embaixo do texto. Para posicionar a sombra mais para cima, utilize valores negativos. Para posicionar a sombra mais para baixo, utilize valores positivos.
- **“Grau de borrão”**\- Opcional. Deixa a sombra com os contornos mais suaves.
- **Cor da sombra** - Aqui você pode definir uma cor diretamente, por exemplo “_black_”, ou utilizar o valor rgba que você aprendeu na seção sobre transparência, criando sombras com cores transparentes.

Você também pode adicionar sombras em uma <div>. Nela, além dos valores que você já viu, é possível definir várias sombras ao mesmo tempo e adicionar mais um valor além do “grau de borrão”, esse valor representa o “grau de espalhamento” da sombra.

Seguindo a disposição das imagens aqui abaixo, veja na Imagem 11 o exemplo de uma página construída com os conceitos vistos nesta seção. Nas imagens 12 e 13 estão os códigos necessários para produzir essa página.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/71a874b2-bb68-4909-847c-3b438ab87d54-image5.jpg)

Imagem 11 - Página HTML com degradês e transparências.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/f912a947-162a-4617-b583-7948c2bca42e-image4.jpg)

Imagem 12 - Código HTML da página da Imagem 11.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/fdeca5e9-64a9-4921-b9b6-e57a56415a82-image10.jpg)

Imagem 13 - Código CSS3 da página da Imagem 11.

Para terminar essa aula, você vai aprender dois recursos avançados que surgiram no CSS3 para tornar sites mais dinâmicos, sem a necessidade de utilizar outras linguagens de programação. Os recursos são: animações e transições.

## Efeitos dinâmicos

## Animações

Para criar uma animação, comece digitando o código `@keyframes` seguido do nome da animação no seletor de um código CSS3. No escopo desse seletor devem ser informados como se encontra o elemento que vai sofrer a animação, na propriedade “from”, e como ele vai ficar após a animação, na propriedade “_to_”.

Essas duas propriedades são um pouco diferentes das demais, pois elas possuem outras propriedades dentro de seus escopos. Assim, no lugar de utilizar “:” para inserir um valor nessas propriedades, utilize o “{“ para começar a inserir propriedades e utilize “}” quando terminar.

Veja na Imagem 14 como utilizar essas novas propriedades. Nessa imagem, você também pode ver como inserir essa animação em uma outra configuração. O seletor #box configura o tamanho de uma `<div>`, a cor, e o posicionamento de um texto.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/197a9494-b38d-48fa-ba55-daca56b68bea-image8.jpg)

Imagem 14 - Configurando uma animação com CSS3.

Na última linha, o nome da animação que vai ser utilizada é configurado através da propriedade _animation_, no caso “animacao”, com a duração da animação (10 segundos), o tempo até a animação iniciar (delay de 2 segundos) e quantas vezes a animação vai repetir (3 vezes). Por fim, a palavra alternate indica que a animação deve “ir e voltar”, como um bumerangue.

Teste o código da Imagem 14, altere os valores e observe o que acontece. Você consegue explicar para que servem as propriedades _left_ e _top_?

Elas indicam a posição de um elemento. Valores positivos movimentam o elemento para direita e para baixo, nas propriedades _left_ e top respectivamente. Já valores negativos, movimentam para a esquerda e para cima.

## Transições

Em aulas passadas, você aprendeu como adicionar efeitos em elementos em seus sites quando o mouse “passava por cima” deles. Porém esse efeito era feito muito rápido, sendo acionado instantaneamente quando o mouse se posicionava.

**Obs**: Transições são muito utilizadas em botões e em menus de navegação, para sinalizar ao visitante o local que ele vai clicar.

Agora, com CSS3, você pode criar transições nesses efeitos fazendo o seu site ficar ainda mais bonito. Basta utilizar a propriedade _transition_ e informar quais propriedades devem demorar um tempo X (que você vai indicar) para se realizar. Veja um exemplo de transição configurada na Imagem 15.

![](https://nyc3.digitaloceanspaces.com/astro-space-prod/courses/book-images/.cache/tmpfdlr_04f.upload/compressed_images/c9cbdf77-f407-4b87-af14-23dfe48c6ce4-image13.jpg)

Imagem 15 - Formatando duas transições ao mesmo tempo.

**Obs**: Se todas as transições tiverem o mesmo tempo, por exemplo 5 segundos, utilize a seguinte linha de código: `transition: all 5s`. Assim seu código fica muito mais simples e fácil de entender.

Lembre-se de salvar os códigos que você desenvolveu hoje. Caso tenha um repositório no Git e essa ferramenta instalada no seu computador, salve o desenvolvimento da aula de hoje através do prompt de comando do computador usando o código abaixo, fornecendo seu usuário e seu diretório como parâmetros.

```
git remote add origin https://github.com/USUÁRIO/DIRETÓRIO.git
git push -u origin master
```

Você também pode usar o GitHub Desktop, caso prefira usar essa interface. Em caso de dúvidas, busque ajuda do seu professor.

Até o momento, você já aprendeu como implementar sites do zero com códigos modernos e melhores, utilizando as versões mais recentes de HTML e CSS. Porém, em algumas tarefas, você tem gastado muito tempo, não é mesmo. A partir da próxima aula, você vai conhecer um conjunto de ferramentas prontas que vai lhe auxiliar a produzir sites de uma forma mais rápida! Mas antes disso, pratique bastante os novos conceitos desta aula resolvendo os exercícios e desafios.

Até a próxima!
