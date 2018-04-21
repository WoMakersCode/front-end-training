# Estrutura de uma página Web (revisão)

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

## Tabelas (revisão)

Através de linhas e colunas, as tabelas abrem inúmeras possibilidades de distribuição dos elementos em um documento, permitindo melhor aproveitamento do espaço, além de tornar sua visualização mais agradável que simples textos corridos. São, portanto, importantes para o trabalho de diagramação e desenho de uma página HTML.

DicaAbaixo, um exemplo da aparência final dos elementos distribuídos em cada célula de uma tabela e, em seguida, sua real estrutura de linhas e colunas (em vermelho).

![](http://www.educacaopublica.rj.gov.br/oficinas/informatica/html/tabelas/img/02.gif)

São três as tags básicas para a montagem de uma tabela: `<table>`, que abre a tabela e indica suas características (borda, etc). `<tr>`, que define linha e `<td>`, cada uma das células de uma linha. Todas elas devem ser finalizadas, nunca esquecendo da hierarquia que rege abertura e fechamento de todas as tags: as que foram abertas primeiro, devem ser fechadas primeiro.

* `<table>` e `</table>`

Definição: Indica o início da tabela. Os atributos definidos dentro dessa tag valem para toda a tabela.

**Atributos:**

width =	largura da tabela (em pixels ou porcentagem)

height =	altura da tabela (em pixels ou porcentagem)

border =	espessura da borda (em pixels). Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

cellspacing =	espaço entre duas células (pixels). Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.
cellpadding =	espaço entre o conteúdo da célula e sua borda (pixels). Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

bordercolor =	cor da borda. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

bgcolor =	cor de fundo para toda a tabela. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

background =	define uma imagem de fundo para a tabela. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

align =	controla o alinhamento da tabela (não de seu conteúdo). Valores: left|right|center. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.



* `<tr>` e `</tr>`

Definição: indicam abertura e encerramento de linha de tabela. Seus atributos valem para toda a linha. Só podem ser usadas dentro da tag `<table>`.

**Atributos:**

align =	controla o alinhamento horizontal do conteúdo em todas as células da linha. Valores: left|right|center. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

valign =	controla o alinhamento vertical do conteúdo em todas as células da linha. Valores: top | middle | bottom. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

bgcolor =	define a cor de fundo de toda a linha. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

background =	define uma imagem de fundo de toda a linha `<td>` e `</td>`. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing**.

* `<td>` e `</td>`

Definição: indicam a abertura e encerramento de cada célula de uma linha. Só podem ser usadas entre `<tr>` e `</td>`. Não é recomendável deixar uma `<td>` sem conteúdo.

**Atributos:**

align =	alinhamento horizontal do conteúdo da célula. Valores: left|right|center. Default: left. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

valign =	alinhamento vertical do conteúdo da célula. Valores: top | middle | bottom. Default: middle. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

colspan =	define o número de células horizontais unidas (mescladas). Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

rowspan =	define o número de células verticais unidas (mescladas).

bgcolor =	cor de fundo da célula. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

background =	define uma imagem de fundo para a célula. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

width =	largura da célula. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

height =	altura da célula. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**

nowrap =	indica que o texto contido na célula não deve receber quebra automática de linha. Evite utilizar este atributo, pois você pode definir isso via CSS. Esse atributo é recomendado **somente na programação de e-mails marketing.**


### Prática de Tabelas

![image](https://user-images.githubusercontent.com/2198735/39086552-962ff236-4569-11e8-8c29-5f49068b66a5.png)

**Exemplo 1**

```html 
<table> <!-- abertura da table -->
    <tr> <!-- abertura da linha da tabela -->
        <td>L1 C1</td> <!-- criação da coluna dentro da linha da tabela -->
        <td>L1 C2</td>
        <td>L1 C3</td>
        <td>L1 C4</td>
    </tr>
        <td>L2 C1</td>
        <td>L2 C2</td>
        <td>L2 C3</td>
        <td>L2 C4</td>
    </tr>
    <tr>
        <td>L3 C1</td>
        <td>L3 C2</td>
        <td>L3 C3</td>
        <td>L3 C4</td>
    </tr>
        <td>L4 C1</td>
        <td>L4 C2</td>
        <td>L4 C3</td>
        <td>L4 C4</td>
    </tr>
</table>
```

**Exemplo 2**

![image](https://user-images.githubusercontent.com/2198735/39086708-68370970-456c-11e8-9213-28fb7940eac2.png)

```html
<table border="1"> <!-- estamos adicionando o border aqui para que você possa visualizar a junção das linhas e colunas, seguindo as regras definidas no rowspan (união/merge de linhas) e colspan(união/merge de coluna)
    <tr>
        <td colspan="2">L1 C1 (unindo a "C2")</td>
        <td>L1 C2</td>
        <td>L1 C3</td>
    </tr>
     </tr>
        <td>L2 C1</td>
        <td>L2 C2</td>
        <td>L2 C3</td>
        <td>L2 C4</td>
    </tr>
     </tr>
        <td>L2 C1</td>
        <td>L2 C2</td>
        <td rowspan="2">L2 e L3 C3</td>
        <td>L2 C4</td>
    </tr>
     </tr>
        <td>L2 C1</td>
        <td>L2 C3</td>
        <td>L2 C4</td>
    </tr>
</table>
```
