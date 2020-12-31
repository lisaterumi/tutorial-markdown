
# Comandos Avançados Markdown

Apresentamos a sintaxe estendida, ou seja, recursos avançados que se baseiam na sintaxe básica do Markdown de John Gruber. Os recursos avançados são tabelas, blocos de código, realce de sintaxe, link automático de URL e notas de rodapé. 

Obs: Verifique a documentação do seu processador para saber se ele suporta esses recursos avançados.

## Indice
1. [Tabelas](#Tabelas)
1. [Realce de sintaxe](#Realce&nbs;de&nbs;sintaxe)
1. [Tachado](#Tachado)
1. [Listas de Tarefa](#Listas de Tarefa)
1. [Emoji](#Emoji)
  1. [Copiando e colando emoji](#Copiando e colando emoji)
  1. [Usando códigos de atalho de emoji](#Usando códigos de atalho de emoji)
1. [Desativando Link Automático de URL](#Desativando Link Automático de URL)


## Tabelas
Para adicionar uma tabela, use três ou mais hífens (---) para criar o cabeçalho de cada coluna e verticais (|) para separar cada coluna. Opcionalmente, você pode adicionar bordas em qualquer extremidade da tabela.

Para alinhar o texto, basta adicionar dois-pontos (:) à esquerda, à direita ou em ambos os lados dos hifens na linha do cabeçalho.

Obs: Podemos formatar o texto dentro da tabela, como links, código, negrito, etc. Mas não podemos adicionar títulos, blockquotes, listas, linhas horizontais, imagens ou tags HTML.

Ex.

<pre>
| Sintaxe     | Descrição  |
| ----------- | -----------|
| Cabeçalho   | Titulo     |
| Paragrafo   | Texto      |

| Sintaxe     | Descrição | Outro Texto|
| :---        |   :----:  |       ---: |
| Cabeçalho   | Titulo    | Mais texto |
| Paragrafo   | Texto     | E mais     |

</pre>


Saída:

| Sintaxe      | Descrição |
| ----------- | ----------- |
| Cabeçalho      | Titulo    |
| Paragrafo   | Texto        |

| Sintaxe     | Descrição | Outro Texto|
| :---        |    :----: |       ---: |
| Cabeçalho   | Titulo    | Mais texto |
| Paragrafo   | Texto     | E mais     |


Dica: Para acelerar o processo, você pode usar o [Gerador de tabelas Markdown](https://www.tablesgenerator.com/markdown_tables).

## Realce de sintaxe

Muitos processadores Markdown suportam realce de sintaxe para blocos de código protegidos. Este recurso permite adicionar realce de cor para qualquer idioma em que seu código foi escrito. Para adicionar realce de sintaxe, especifique um idioma próximo aos crases antes do bloco de código protegido.

Ex:

<pre>
```json
{
  "nome": "Camila",
  "sobrenome": "Silva",
  "idade": 41
}
```
</pre>

Saída:

```json
{
  "nome": "Camila",
  "sobrenome": "Silva",
  "idade": 41
}
```

## Tachado
Você pode tachar palavras colocando \~\~ antes e depois das palavras.

Ex:

\~\~A Terra é plana.\~\~ Agora sabemos que é redonda.

Saída:

~~A Terra é plana.~~ Agora sabemos que é redonda.

## Listas de Tarefas
As listas de tarefas são listas de itens com caixas de seleção. Em aplicativos Markdown que suportam listas de tarefas, as caixas de seleção serão exibidas ao lado do conteúdo. Para criar uma lista de tarefas, adicione (-) e colchetes com um espaço ([ ]) na frente dos itens da lista de tarefas. Para selecionar uma caixa de seleção, adicione um x entre colchetes ([x]).

Ex:

<pre>
- [x] Tarefa 1
- [ ] Tarefa 2
- [ ] Tarefa 3
</pre>

Saída:

- [x] Tarefa 1
- [ ] Tarefa 2
- [ ] Tarefa 3

## Emoji
Existem duas maneiras de adicionar emoji a arquivos Markdown: copie e cole o emoji em seu texto formatado em Markdown ou digite códigos de atalho de emoji .

### Copiando e colando emoji
Podemos apenas copiar um emoji de uma fonte como a Emojipedia e colá-lo em nosso documento. Muitos aplicativos Markdown exibirão automaticamente o emoji no texto formatado em Markdown. 

Obs: se você estiver usando um gerador de site estático, certifique-se de codificar as páginas HTML como UTF-8 .

### Usando códigos de atalho de emoji
Alguns aplicativos Markdown permitem inserir emoji digitando códigos de atalho de emoji. Eles começam e terminam com dois pontos e incluem o nome de um emoji.

Ex:

<pre>
Fomos acampar! :tent: Voltamos logo.

Foi divertido! :joy:
</pre>

Saída:

Fomos acampar! :tent: Voltamos logo.

Foi divertido! :joy:

## Desativando Link Automático de URL
Muitos processadores Markdown transformam URLs em links automaticamente. Isso significa que se digitarmos http://www.example.com, o processador Markdown o transformará automaticamente em um link, mesmo que você não tenha usado colchetes.

Para evitar que uma URL seja vinculada a um link automaticamente, basta remover o link usando crases.

Ex: 

\`http://www.example.com\`

Saída:

`http://www.example.com`


Adaptado de: https://www.markdownguide.org/extended-syntax/
