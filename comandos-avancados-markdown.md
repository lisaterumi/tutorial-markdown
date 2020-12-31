
# Comandos Avançados Markdown

Apresentamos a sintaxe estendida, ou seja, recursos avançados que se baseiam na sintaxe básica do Markdown de John Gruber. Os recursos avançados são tabelas, blocos de código, realce de sintaxe, link automático de URL e notas de rodapé. 

Obs: Verifique a documentação do seu processador para saber se ele suporta esses recursos avançados.

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
| :---        |    :----: |       ---: |
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

