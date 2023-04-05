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
            <li>Home</li> -tópicos da lista
            <li>Professores</li>
            <li><a href="Conosco.html"> Fale conosco</a></li>
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