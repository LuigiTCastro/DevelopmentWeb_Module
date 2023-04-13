# HTML [LinguagemDeMarcaçãoDeHipertexto]
Padrão de linguagem para paginas e documentos na internet.

> W3C
Organização de padronização da WWW.
Atualizam e mantém o HTML e CSS.

> TAGS
Toda marcação no HTML, utiliza abertura e fechamento de TAG.
<tag> abertura
    conteudo
</tag> fechamento


# HMTL BLOCK SYNTAX
<!DOCTYPE html>
<html> -inicio. todo conteudo dentro da tag html é na linguagem html.
    <head> -'cabeça'. possui configuracoes e parametros.
        <title></title> -titulo do documento.
    </head> -fechamento.
    <body> -'corpo'. tudo dentro dessa tag é o que sera exibido.
        <header> -'cabeçalho' do documento. parte de cima do site. não sofre alteração entre as paginas.
        </header>
        <main> -conteudo principal do documento.
            <section> -secoes do documento.
            </section>
        </main>
        <footer> -'rodape'. conteudo final.
        </footer>
    </body>
<html>

A estrutura possui: ``abertura html, cabeca e corpo.``
**A tag Head nao é o cabecalho! Mas sim, as configurações e parâmetros.
**Header é o cabecalho (its inside the body block)


# HEAD BLOCK SYNTAX [configurations]
<!DOCTYPE html> -indicates that the document is of html type
    <html lang="pt-br"> -indicates the language of the document
    <head>
        <meta charset="utf-8"/> -communicate to browsers the characters codification used in a document (independent of user region)
        <title>...</title>
    </head>
    </html>

__INDEX.HTML - website main page__

Warning!
As good practice, do not uses the login page as an index.


# BODY
# HEADER BLOCK SYNTAX
<header>
    <h1>Hello world. This is my first page.</h1> -marcação de título/subtitulo. (h1,h2,h3...).
    <nav> -marcação de navegação (menu, botões...)
        <ul> -marcação de lista em formato de tópicos. 'ul' indica que vai iniciar uma lista. todo tópico de 
                                                                                    dentro utiliza a tag 'li'.
            <li>...</li> -tópicos da lista
            <li>...</li>
            <li><a href="xxx.html">...</a></li>
        </ul>
    </nav>
</header>

__<a></a> marcação para direcionar para outra página (link)__
__href = para onde se quer ser direcionado. href fica dentro de <a> -> <a herf="...">__


# MAIN BLOCK SYNTAX
<main> -conteúdo principal!! tudo que está depois do header a antes do footer.
    <section> -marcação de uma sessão.
        <div> -marcação de divisão. geralmente possui um css envolvido (parte visual).
            <img src="" width="" height="" alt=""/> -marcação de uma imagem.
        </div>
        <article> -marcação de um artigo ou conteúdo relevante.
            <h2>
            <p> -marcação de paragrafo de texto.
            <strong> -recurso para dar evidência ao texto (negrito).
            <em> -recursos para dar enfase ao texto (italico).
            </p>
        </article>
    <section>
</main>

__src = source = fonte da imagem__
__width = largura__
__height = altura__
__alt = texto alternativo da imagem__


# FOOTER BLOCK SYNTAX
<footer> -rodapé.
<span>
<br/> -quebra de linha.



__Warning!__
> HTML [Head-Body]
    > HEAD [Configurations]
    > BODY [Header-Main-Footer]



# FORM
desenvolvido dentro da main.

<form> marcacaçao de formulario HTML. permite inserir dados em uma pagina da web. dentro das tags form, adiciona-se os tipos de campos de entrada.

Syntax ex.: 
<form action="index.html"> action: indica o destino da açao apos finalizar o formulario.
    <p>
        <label>Nome: </label> marcacao de legenda para um campo do form.
        <input type="text" name="nome" placeholder="Digite seu nome" required/> marcacao do campo do form. type=text: entrada de texto simples.
    </p>
    <p>
        <label>Email: </label><input type="text" name="Email"/>
    </p>
    <p>
        <label>Comentarios: </label>
        <textarea name="Comentarios" rows="4" cols="50"></textarea> marcacao de entrada de texto multi-linhas.
    </p>
    <p>
        <label>Sexo: </label>
        <input type="radio" nome="sexo"> type=radio: botao de opcao.
    </p>
    <p>
        <label>Aonde nos conheceu?: </label>
        <select name="conheceu"> select: lista de opçoes.
            <option selected>...</option>
            <option>...</option>
            <option>...</option>
        </select>
    </p>
    <p>
        <input type="checkbox" name="aceito"> marcacao de um elemento botao de opcao.
        <label>...</label>
    </p>
    <p>
        <input type="submit" .../> marcacao de botao de açao do formulario. (nao é necessario criar label)
        <input type="reset" .../> marcacao de botao de limpeza do formulario. (nao é necessario criar label)
    </p>

    **Radio: quando marca um, desmarca o outro.
    **Checkbox: pode haver varios, e todos serem marcados.
    **Select: lista de opçoes, com apenas uma escolha? (tag propria e nao input)


> tags dos campos de entrada: <INPUT>, <SELECT>, <TEXTAREA> etc.

<INPUT type> diferentes valores do atibruto type. <type= text,email,password,checkbox,radio,submit...>
<INPUT name> nome do campo para identificar o valor do campo.
<INPUT placeholder> espaço reservado. texto de dica para o que inserir.
<INPUT required> torna o campo obrigatório.


# TABLE
<section>
    <h2></h2>
    <table> marcacao do elemento tabela.
        <thead> define linha/grupo de linhas que representam os cabeçalhos de uma tabela.
            <tr> marcacao das linhas. (table row)
                <th></th> marcacao das colunas / celula de cabeçalho / define o nome de uma coluna.
                <th></th> 
            </tr>
        <tbody> define o conjunto de dados de uma tabela.
            <tr>
                <td></td> marcacao das celulas (dados/valores). (table data)
                <td></td> 
            </tr>

**TR - Rows [TableRows]
**TH - Columns [TableHeader]
**TD - Cells/Values [TableData]
**Put the same quantity of TH(columns) and TD(values)


# IFRAME x VIDEO
<section>
    <div>
        <iframe src="..."></iframe> marcacao de uma pagina dentro de outra.
    </div>
</section>

<section>
    <video width="" controls="controls"> marcacao de um video em pasta local.
        <source src="path/file.extension" type="video/extension">
    </video>

**Se quiser pegar um video de uma pagina -> IFRAME.
**Se quiser pegar um video uma pasta local -> VIDEO.


# ABBR, BLOCKQUOTE [goodpractices]
<section>
    <abbr title="Word to be abbreviated">WordAbbreviated</abbr> marcaçao da explicaçao de uma abreviaçao.
    <blockquote cite="...">...</blockquote> marcaçao de uma citaçao. [Bloco de Citaçao]
</section>


# FIGURE, FIGCAPTION [goodpractices]
<section>
    <figure> marcaçao de uma imagem.
        <img src="path/file.extension" width="" alt="">
        <figcpation>...</figcaption> marcaçao da legenda de uma imagem.


# METATAGS (HEAD) [goodpractices]
<meta name="description" content="..."> marcaçao da descriçao do documento. da acesso a descriçao da pagina para os browsers e sites de busca.
<meta name="keywords" content=""> marcaçao das palavras chaves.
<meta name="author" content=""> marcaçao do autor do documento.
<meta http-equiv="refresh" content="50"> marcaçao do tempo de refresh.



__ToolsTips__
W3Schools.com
DeveloperMozilla.com
(inspecionar sites para ver os códigos; f12)