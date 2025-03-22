### ☠ TCC HTML e CSS

*Chegou o momento de misturar tudo que a gente viu até agora em um exercício, o nosso TCC.*

## Layout está [aqui neste Figma](https://www.figma.com/design/tMcQJrlA9vDEzaLCbCplOC/Crescer-TCC-HTML%2FCSS?node-id=1812-324&t=wdtrbAPwMKrHL0Gl-0)

# Regras
- Individual
- Responsivo
- Mais fiel ao layout possível
- Organizado estruturalmente (arquivos, pastas, etc)
- As páginas devem estar linkadas entre elas
- Não deve haver duplicação de código. Ex.: Criar o css do botão duas vezes quando você pode criar uma classe e reaproveitar

## Dicas
- Usem `min-height: 100vh` e `margin: 0` no body
- Nas sections podem usar `min-height: {valor}vh` e a largura deve ser em `%` **NÃO** pode ser em `vw`
- Exportem as fotos em jpg, se tiver fundo transparente usem png
- Ícones e logo, exportem em .svg
- Usem transition nos cards das pessoas
- Voltem as aulas, vários componentes do TCC já foram explicados em aula
- Importante, se você usar `!important` eu vou ter certeza que você não prestou atenção na aula de especificidade
- ⚠Façam commits e pushes regularmente ⚠


## Fontes
Importem a fonte
``` html
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Open+Sans&display=swap" rel="stylesheet">
```

Usem cada uma conforme a necessidade.
```css
font-family: 'Montserrat', sans-serif;
font-family: 'Open Sans', sans-serif;
```


🚧 Não apague o conteúdo da pasta `prints`.

🚧 Para cada página você deve salvar o arquivo html como index.html, dentro de seu respectivo diretório. Exemplo:

Home: `/index.html`

Sobre: `/sobre/index.html`

Contato: `/contato/index.html`


## Estrutura de diretórios ideal
```
│   index.html
│
│
├───/contato
│       index.html
│
├───/sobre
|       index.html
|
└───/assets
    │
    ├───/css
    │   ├───/common
    │   │       style.css
    |   |       header.css
    |   |       footer.css
    │   │
    │   ├───/contact
    │   │       contact.css
    │   │
    │   └───/about
    │           about.css
    │
    └───/img
            logo.svg
            another-img.png


```
