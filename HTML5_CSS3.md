# HTML5 CSS3
## Links de apoio

github.com/gustavoguanabara
gustavoguanabara.github.io
------------------------------------------------------------------------------------------------------------------------
# Um pouco da História da Internet
Internet vem da arpanet que surgiu na guerra fria
HTML - Hyper Text Marc Linguage: linguagem de marcação de texto

# DNS
Domain Name Service: como se fosse uma agenda telefonica da internet ele tem o ip que seria o 
numero e o nome da pessoa seria o endereço web (instagram.com).

# Dominio e Hospedagem
Dominio é unico 
Hospedagem é um lugar pra armazenar os seus arquivos
TLD: top level domain
GTLD: São os TLDs genéricos, sem indicação de pais. .com, .net, .org, .info
ccTLD: São TLDs com designação do pais. .com.br, .edu.us, .co.fr

URL - www.github.com/gustavoguanabara
Dominio - github.com
TLD - .com
Sub-dominio - www
Caminho - /gustavoguanabara

# HTML
 Hyper Text Mark Language - Linguagem de Marcação de HiperTexto

## Estrutura básica de documentos HTML
<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <meta name ="viewport"
        content="width=device-width,
        initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <h1>Olá, Mundo!</h1>
    </body>
</html>

## Hierarquia de Titulos

<h1> - Título 
<h2> - subtitulo
<h3> - subTitulos subsequentes
<h4>
<h5>

## Semântica

html é significado, da o significado para as coisas (sentido da coisa)
css é forma, da a forma a cor a animação (forma da coisa)

### Algumas tags semânticamente corretas na data atual (2024)

strong - negrito/destaque
em - itálico/ênfase
mark - texto marcado
small - deixar as letras minusculas (para deixar elas grandes use o CSS)
del - deixar o texto como excluido
ins - deixar o texto sublinhado/inserido
sup - deixar o texto ou letra superior
sub - dexar o texto inferior
abbr - dando significado as abreviações
q - Citação simples
blockquote - Citação completa ex: 
            <blockquote cite="https://www.google.com.br/books/edition/HTML5_e_CSS3/XXCCCwAAQBAJ?hl=pt-BR&gbpv=1&dq=html+para+leigos&printsec=frontcover">
                Da mesma forma que organizamos elementos em exemplos menores, podemos organizar os principais elementos da página utilizando float.
            </blockquote>

code - deixando o texto mono espaçado
pre - pré formatação, tudo dentro do pre vai ser considerado e exebido da mesma forma ex:
            <pre>
                <code>
            num = int(input('Digite um texto'))
            if num % 2 == 0:
                print(f' o numero {num} é PAR')
            else:
                print(f'O número {num} é IMPAR')
            print('fim do programa')
                </code>
            </pre>
    até os espaços contam


### Listas
Lista ordenada - <ol></ol>
    type="" define o tipo da ordem (númerica = "1", romana = "I" ou "i", alfanumérica= "A" ou "a")
    start="" pode definir de onde começãr exemplo: start="5"
Lista desordenadas - <ul></ul>
    type="" define o tipo do marcador ( disc, circle, square)
dentro de cada lista tem os items e adicionar os items é com o li - <li>

exemplo de uma lista ordenada:
    <ol type="1" start="5">
        <li>acordar
        <li>abrir os olhos
        <li>levantar
        <li>colocar os chinelos
        <li>andar até o banheiro
        <li>pegar a escova
        <li>pegar a pasta
        <li>abrir a tampa da pasta
        <li>passar a pasta na escova
        <li>fechar a tampa
        <li>escovar os dentes
    </ol>

Lista de definição
    dl - definição de lista
    dt - item de definição
    dd - descrição da definição
    <dl>
        <dt>HTML</dt>
        <dd>Linguagem de marcação para a criação de conteúdo de um site</dd>
        <dt>CSS</dt>
        <dd>Linguagem de marcação para a criação do design de um site</dd>
        <dt>Javascript</dt>
        <dd>Linguagem de programação para a criação de interatividade de um site</dd>
    </dl>

