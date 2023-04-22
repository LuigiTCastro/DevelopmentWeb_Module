# CSS [CascadingStyleSheets]
Folha de estilo em cascata
Aplica estilos em linguagens de marcaçao (xml, xhtml, html...)

> W3C
Organização de padronização da WWW.
Atualizam e mantém o HTML e CSS.

> Syntax:
<h1{color:...; font-size:...; ...}

h1 - Selector: indica o elemento html a estilizar.
{a:b} - Declaration: regras aplicadas na estilização.
a - Property
b - Value

# APPLICATION
> How to apply?

1) InLine
    <button style="background-color: red;"></button>

2) InPage
    <style>
        p{color: blue;}
        .btn-green{background-color: green} 
<!-- to declare as a CLASS, its necessary to put the point at the beginning -->
       #btn-red{background-color: red}
<!-- to declare as a ID, its necessary to put the hash at the beginning -->
    </style>

<p>
    ... <!-- (will turn blue) -->
</p>
<button class="btn-green">
    ... <!-- (will turn green) -->
</button>

3) In Link
<!-- Its not necessary to apply the style tag <style> in the css file. -->

h1{
    color:red
} /*selector*/

.color-green ul li a{
    color:green
} /*class*/

#color-black{
    color: black;
} /*id*/

#link-home{
    color: black;
} /*id*/


``Good Practice`` <!-- Its considered a GOOD PRACTICE to apply css in a page -> implement the styles in a file with .css extension separated from html file. -->

__Responsividade__
__Mobile First__ desenvolver primeiro para os dispositivos móveis depois para as telas maiores.
__DevTools__ developer tools (f12) or right button > inspect or ...


**CSS NAO TEM EFEITO NA HEAD.


# VIEWPORT
[MetaTag-type]
Ajuda a adaptar o conteúdo de uma página da web para diferentes dispositivos.
Allows to control the page size and scale on mobile devices.

``Responsive Design Technique.``

<meta name="viewport" content="width=device-width, initial-scale=1.0">


# SPECIFICS STYLES...
global.css [html,body]
header.css
index.css [main?]
footer.css


# MEDIA QUERY
Define custom styles for differents types of devices and medias.
**Tamanhos de tela específicos.
**Tipos de dispositivos específicos.

``Responsive Design Technique.``

ex.: 
@media screen and (min-width: 992px){
    body{
        color: ...;
    }
}


__Take note!__
[BreakpointsCss]: screen limits.
Default: 992px is even the limit of a TABLET. (more than this is a DESKTOP).

``Relative position: follows the default flow of screen design.``
``Absolute position: has a fixed position.``


__ToolsTips__
W3Schools.com
DeveloperMozilla.com
(inspecionar sites para ver os códigos; f12)


# PSEUDO-ELEMENTS
Selectors that allow selecting multiple elements for to apply styles on a specific element according with
his state or position inside father element.

<Syntax ex.:>
<footer section span:first-child{...}>    <first-child>
<header nav ul li a:hover{...}>          <hover>

<!-- its not necessary to use the tags -->


__TakeNote!__
<fatherElement child1 child2 child3..>

<Syntax ex.:>
header a img{}
header nav ul li a{}


# EM x REM
A unidade em (em) define um valor em relação à fonte do elemento pai. Por exemplo, se um elemento tem um tamanho de fonte definido como 1.5em, isso significa que sua fonte será 1,5 vezes maior do que a fonte do elemento pai.

Já a unidade rem (root em) define um valor em relação à fonte raiz do documento, que normalmente é definida no elemento html. Por exemplo, se a fonte raiz do documento tem um tamanho definido como 16px, um valor de 2rem seria equivalente a 32px, independentemente das dimensões da fonte do elemento pai.

A principal diferença entre as unidades em e rem é que a unidade em é relativa ao tamanho da fonte do elemento pai, enquanto a unidade rem é relativa ao tamanho da fonte raiz do documento.


# SELETOR DE ATRIBUTO
<Syntax ex.:>
input[type="checkbox"] {}


# ...
> O seletor <main .section-capa, .section-video> afeta dois tipos de elementos:
Nesse caso, o seletor não é definido para a tag 'main, a main serve apenas como base da hierarquia.
Todos os elementos que possuem a classe .section-capa dentro do elemento main.
Todos os elementos que possuem a classe .section-video, independentemente de sua posição na árvore de elementos.

> Quando a unidade é definida em pixels é verdade dizer que:
Quando a unidade é definida em pixels, o tamanho do elemento será fixo e não irá se adaptar ao tamanho da tela ou do dispositivo utilizado para visualizar o site. Isso pode tornar o site menos responsivo e dificultar a visualização em dispositivos com telas menores ou maiores do que o tamanho definido em pixels. No entanto, a definição em pixels pode ser útil para elementos que precisam ter um tamanho fixo, como ícones ou elementos de interface gráfica.

> Para que serve a propriedade 'important'? <h1 {color: red !important;}>
É uma regra de estilo deve ter prioridade sobre as outras regras definidas para o mesmo elemento.
Define a declaração com prioridade mais alta, independente da hierarquia.






