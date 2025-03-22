### 🤳 Exercício Post do Instagram com Flexbox

*Agora que você já conhece algumas propridades do flexbox, que tal começar a usar elas para fazer alguns componentes?*

Vamos lá...

- O exercício consistem em criar uma cópia de um post do Instagram;
- Criem um novo arquivo css com as propriedades que vocês vão fazer, e importem no html;
- O layout encontra-se [neste link](https://www.figma.com/file/GSDl0QXN9gGFtfQRvwGJEp/Untitled?node-id=0%3A1);
- Para acessar o layout você vai ter que criar uma conta no [Figma](https://www.figma.com/);
- Para exportar a imagem do Figma, você tem que selecionar ela, e na sidebar da direita tem uma opção **export**. Aqui tem a [documentação do Figma](https://help.figma.com/hc/en-us/articles/360040028114-Guide-to-exports-in-Figma#:~:text=Click%20the%20in%20the%20Export,SVG%2C%20JPG%2C%20or%20PDF.) de como exportar;
- Você deve deixar o resultado o mais fiel possível ao layout.

🚧 Não apague o conteúdo da pasta `prints`.

🚧 Você deve salvar o arquivo html como index.html para que a pipeline de correção funcione corretamente.

Já fiz um html e um css base pra facilitar pra vocês, vocês só precisam salvar e continuar codando 😉:

index.html

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram</title>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <article class="instagram-post">
        <img src="https://i.imgur.com/innWLeZ.png" class="header" alt="Header">
        <!-- AQUI INICIA O SEU CÓDIGO -->



        <!-- AQUI TERMINA O SEU CÓDIGO -->
    </article>
</body>
</html>


```

style.css

```css

* {
    box-sizing: border-box;
}

body {
    font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #d9dbde;
}

.instagram-post {
    min-width: 395px;
    width: 395px;
    height: 700px;
    border: 10px solid #333;
    border-radius: 30px;
    background: #fff;
    overflow: hidden;
}

.header {
    max-width: 100%;
}

```


💡 Uma dica, se você está chutando as propriedades, eu recomendo fortemente pedir ajuda aos colegas ou monitores.

O fato de aprender usar o flexbox sem chutar as propriedades vai te ajudar a ganhar muita velocidade nos próximos exercícios.
