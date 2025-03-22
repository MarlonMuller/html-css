# 📘 Exercício do Livro
Utilizando o que vimos em aula, faça o possível para implementar a seguinte tela:

![Imagem da tela](https://i.imgur.com/bj3yX4C.png)

## DON'T PANIC!
A base da tela já está pronta, a única coisa que você irá fazer é o corpo da página (que barbada heim?!)

🚧 Não apague o conteúdo da pasta `prints`.

🚧 Você deve salvar o arquivo html como index.html para que a pipeline de correção funcione corretamente.

### Observações
 - Testem o código usando apenas o Google Chrome.
 - Não precisa tentar entender o que foi feito na base (mas se quiser, go ahead)
 - Bote o CSS que vocês criarem em um arquivo separado (facilitei pra vocês, facilitem pra mim)
 - Não me faça gambiarra. A cada `!important`, um dedo ser cortado.
 - O Texto está logo abaixo.

``` txt
Hypertext Markup Language (HTML) is the standard markup language for creating web pages and web applications. With Cascading Style Sheets (CSS) and Javascript it forms a triad of cornerstone technologies for the World Wide Web.
HTML elements are the building blocks of HTML pages. With HTML constructs, images and other objects, such as interactive forms, may be embedded into the rendered page. It provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other itens. HTML elements are delineated by tags, written using angle brackets. Tags such as <img /> and <input /> introduce content into the page directly. Others such as <p>...</p> surround and provide information about document text and may include other tags as sub-elements. Browsers do not display the HTML tags, but use them to interpret the content of the page.
HTML can embed programs written in a scripting language such as Javascript which affect the behavior and content of web pages. Inclusion of CSS defines the look and layout of content. The World Wide Web Consortium (W3C), maintener of both the HTML and the CSS standards, has encouraged the use of CSS over explicit presentational HTML since 1997.
In 1980, physicist Tim Berners-Lee, a contractor at CERN, proposed and prototyped ENQUIRE, a system for CERN researchers to use and share documents. In 1989, Berners-Lee wrote a memo proposing an Internet-based hypertext system. Berners-Lee specified HTML and wrote the browser and server software in late 1990. That year, Berners-Lee and CERN data systems engineer Robert Cailliau collaborated on a joint request for funding, but the project was not formally adopted by CERN. In his personal notes from 1990 he listed "some of the many areas in which hypertext is used" and put an encyclopedia first.
After the HTML and HTML+ draft expired in early 1994, the IETF created an HTML Working Group, which in 1995 completed "HTML 2.0", the first HTML specification intended to be treated as a standard against which future implementations should be based.
HTML versions timeline:
November 25, 1995: RFC 1867 (form-based file upload)
May 1996: RFC 1942 (tables)
August 1996: RFC 1980 (client-side image maps)
January 1997: RFC 2070 (internationalization)
Some cool stuff
"What if highlighting the text actually looked like a highlighter? "
"What if I wanted it to be pink ?"
" Blue?"
" Green?"
" Orange?"
"What if I found a typo and wanted to make a correction ?"
"What if I was viewing this on mobile—"
```


```html
<!-- index.html -->
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Crescer HTML/CSS</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div id="wrapper">
    <div id="container">

      <section class="open-book">
        <header>
          <h1>CWI Software</h1>
          <h6>Projeto Crescer</h6>
        </header>
        <article>
          <h2 class="chapter-title">MÓDULO HTML/CSS</h2>

          <!-- AQUI É CONTIGO -->

        </article>
        <footer>
          <ol id="page-numbers">
            <li>1</li>
            <li>2</li>
          </ol>
        </footer>
      </section>

    </div>
  </div>
</body>
</html>
```

```css
/* styles.css */
@import url(https://fonts.googleapis.com/css?family=Crimson+Text:400,700,900,400italic,700italic,900italic|Playfair+Display:400,700,900,400italic,700italic,900italic|Rock+Salt:400);

*,
:before,
:after {
  box-sizing: border-box;
}

body {
  background-color: #1d1f20;
  color: #e5e5e5;
  font: 16px/1.25 'Crimson Text', sans-serif;
  margin: 0;
}

#wrapper {
  margin-left: auto;
  margin-right: auto;
  max-width: 1280px;
}

#container {
  float: left;
  padding: 16px;
  width: 100%;
}

.open-book {
  background: #fff;
  box-shadow: rgba(0,0,0,0.5) 0 16px 48px;
  color: #000;
  padding: 32px;
}

.open-book * {
  position: relative;
}

.open-book *::-moz-selection {
  background: rgba(222,255,0,0.75);
}

.open-book *::selection {
  background: rgba(222,255,0,0.75);
}

.open-book header {
  padding-bottom: 16px;
}

.open-book header *,
.open-book footer * {
  font: 700 16px/1.25 'Playfair Display', sans-serif;
  letter-spacing: 2px;
  margin: 0;
}

.open-book header * {
  font-size: 12px;
  text-transform: uppercase;
}

.open-book footer {
  padding-top: 16px;
}

.open-book footer #page-numbers {
  display: none;
  list-style: none;
  padding: 0;
  text-align: left;
}

.open-book footer #page-numbers > li:last-child {
  text-align: right;
}

.open-book .chapter-title {
  background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiDQoJIHZpZXdCb3g9IjAgMCA2NCA2NCIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgNjQgNjQ7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCiAgICA8Zz4NCiAgICAJPHBhdGggZD0iTTAsMzJMMzIsMGwzMiwzMkwzMiw2NEwwLDMyeiBNOCwzMmwyNCwyNGwyNC0yNEwzMiw4TDgsMzJ6IE0xNiwzMmwxNi0xNmwxNiwxNkwzMiw0OEwxNiwzMnogTTI0LDMybDgsOGw4LThsLTgtOEwyNCwzMnoiIC8+DQogICAgPC9nPg0KPC9zdmc+) bottom center no-repeat;
  background-size: 0.5em 0.5em;
  font: 700 7vw/1.25 'Playfair Display', sans-serif;
  letter-spacing: 0.125em;
  margin: 0 0 1em 0;
  padding: 1em 0;
  position: relative;
  text-align: center;
  text-transform: uppercase;
}

.open-book .chapter-title:before,
.open-book .chapter-title:after {
  border: solid 0 #000;
  border-width: 0.05em 0;
  bottom: calc((0.125em / 2) * 3);
  content: '';
  height: 0.15em;
  position: absolute;
  width: calc(50% - (1em / 2));
}

.open-book .chapter-title:before {
  left: 0;
}

.open-book .chapter-title:after {
  right: 0;
}

@media only screen and ( min-width: 830px ) {

  .open-book {
    margin: 16px;
    position: relative;
  }

  .open-book:before {
    background-color: #8B4513;
    border-radius: 4px;
    bottom: -16px;
    content: '';
    left: -16px;
    position: absolute;
    right: -16px;
    top: -16px;
    z-index: -1;
  }

  .open-book:after {
    background: linear-gradient(to right, transparent 0%,rgba(0,0,0,0.2) 46%,rgba(0,0,0,0.5) 49%,rgba(0,0,0,0.6) 50%,rgba(0,0,0,0.5) 51%,rgba(0,0,0,0.2) 52%,transparent 100%);
    bottom: -16px;
    content: '';
    left: 50%;
    position: absolute;
    top: -16px;
    transform: translate(-50%,0);
    width: 64px;
    z-index: 1;
  }

  .open-book > * {
    column-count: 2;
    column-gap: 96px;
    position: relative;
    z-index: 1;
  }

  .open-book header:before,
  .open-book header:after,
  .open-book footer:before,
  .open-book footer:after {
    background: #fff;
    border-radius: 25%;
    content: '';
    height: 32px;
    position: absolute;
    z-index: -1;
    width: calc(50% + 32px);
  }

  .open-book header:before,
  .open-book footer:before,
  .open-book footer:after {
    border-top-left-radius: 0;
  }

  .open-book header:after,
  .open-book footer:before,
  .open-book footer:after {
    border-top-right-radius: 0;
  }

  .open-book header:before,
  .open-book header:after,
  .open-book footer:after {
    border-bottom-right-radius: 0;
  }

  .open-book header:before,
  .open-book header:after,
  .open-book footer:before {
    border-bottom-left-radius: 0;
  }

  .open-book header:before,
  .open-book header:after {
    top: -42.4px;
  }

  .open-book header:before,
  .open-book footer:before {
    right: 50%;
  }

  .open-book header:before {
    transform: rotate(-2deg);
  }

  .open-book header:after,
  .open-book footer:after {
    left: 50%;
  }

  .open-book header:after {
    transform: rotate(2deg);
  }

  .open-book footer:before,
  .open-book footer:after {
    bottom: -42.4px;
  }

  .open-book footer:before {
    transform: rotate(2deg);
  }

  .open-book footer:after {
    transform: rotate(-2deg);
  }

  .open-book header > *:last-child,
  .open-book footer > *:last-child {
    text-align: right;
  }

  .open-book footer #page-numbers {
    display: block;
  }

  .open-book .chapter-title {
    font-size: 48px;
  }

  .open-book .chapter-title:before,
  .open-book .chapter-title:after {
    height: 0.125em;
  }
}
```

