A estrutura básica de um documento HTML é composta por três tags (`html`, `head` e `body`), deve estar presente em todos os documentos, e seguir exatamente a seguinte sequência:

![](http://www.educacaopublica.rj.gov.br/oficinas/informatica/html/estrutura/img/01.gif)

Antes de criarmos essa estrutura (esquelo da página), precisamos adicionar o doctype para informar ao (browser) navegador o tipo de documento que ele está recebendo. Essa "leitura" é feita no momento em que acessando o site. Para informar o tipo de documento, adicionamos a tag `<!DOCTYPE html>`.

O resultado será:

```html
<!DOCTYPE html>
<html>
    <head>
        <title></title>
    </head>

    <body>
    
    </body>
</html>
```

A seguir, cada uma delas e, ao final, sua aplicação.

* `<html>` e `</html>`

Definição: Tag utilizada pelo navegador para identificar que o documento em questão trata-se de um HTML e não de texto puro. Entre `<html>` e `</html>` devem estar todas as outras tags, as informações e todo o conteúdo.
**Atributos:** não possui.


* `<head>` e `</head>`

Definição: início e o fim do cabeçalho do documento, onde devem ser inseridas outras tags com dados e informações que não são exibidos na tela do navegador, mas utilizados por ele para fins diversos.
**Atributos:** não possui.
`<title>` e `</title>`

Definição: sempre contida entre `<head>` e `</head>` define o título do documento a ser exibido pela barra de títulos do navegador.
**Atributos:** não possui.


* `<body>` e `</body>`

Definição: corpo do documento. Entre `<body>` e `</body>` está o que vai, efetivamente, ser exibido na tela do navegador.
**Atributos:** você pode adicionar os atributos `class` e `id`, para proporcionar manipulação de [DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model) via JavaScript ou aplicar estilos de CSS. É possível adicionar outros elementos, mas por questões de semântica e qualidade de código, indicamos que restrinja a implementação somente de `class` e `id`.
