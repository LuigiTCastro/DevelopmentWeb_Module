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