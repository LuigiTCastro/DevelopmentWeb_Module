# CSS [CascadingStyleSheets]
Folha de estilo em cascata
Aplica estilos em linguagens de marcaçao (xml, xhtml, html...)

> Syntax:
<h1{color:...; font-size:...; ...}

h1 - Selector: indica o elemento html a estilizar.
{a:b} - Declaration: regras aplicadas na estilização.
a - Property
b - Value

> How to apply?

1) InLine
    <button style="background-color: red;"></button>

2) InPage
    <style>
        p{color: blue;}
        .btn-green{background-color: green} 
<!-- to declare as a class, its necessary to put the point at the beginning -->
       #btn-red{background-color: red}
<!-- to declare as a id, its necessary to put the hash at the beginning -->
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



**Responsividade
**Mobile First - desenvolver primeiro para os dispositivos móveis depois para as telas maiores.
**DevTools - ferramentas de desenvolvimento (f12) ou botao direito > inspecionar ou ...

# VIEWPORT
MetaTag

<meta name="viewport" content="width=device-width, initial-scale=1.0">