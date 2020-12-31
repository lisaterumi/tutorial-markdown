# Tutorial Markdown

## Títulos
Para criar um título, basta adicionar ```#``` na frente de uma palavra ou frase, sendo que o número de cerquilhas corresponde ao nível do título. 

Ex: (equiavlente ao  &lt;h3>)

&#35;&#35;&#35; Meu título nível 3

Saída: 

### Meu título nível 3

#### Sintaxe Alternativa
Como alternativa, podemos adicionar = ou - na linha abaixo do texto. Ex: 

Título de nível 1<br>
&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;&equals;	

Título de nível 2<br>
&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;&minus;	

#### Recomendações 
Procure sempre colocar um espaço entre os sinais numéricos e o nome do título (ex "# Meu título" ao invés de "#Meu título").

## Parágrafos
Para criar parágrafos, use uma linha em branco para separar uma ou mais linhas de texto. Não idente com espaços ou tabulações. 

Ex:

"Parágrafo um.

Parágrafo dois"

Equivale a 

"&lt;p>Parágrafo um.&lt;/p>

&lt;p>Parágrafo dois.&lt;/p>"

## Quebras de linha
Para criar uma quebra de linha (equivalente ao &lt;br>), termine uma linha com dois ou mais espaços e tecle Enter. Ex:

"Linha com quebra de linha.  "

## Negrito

Para texto em negrito, adicione dois asteriscos ou sublinhados antes e depois de uma palavra ou frase, ou ao redor das letras. Ex: 

Texto &lowast;&lowast;em negrito&lowast;&lowast;.	

Texto  &#95;&#95;em negrito &#95;&#95;.	

## Itálico

Para colocar o texto em itálico, adicione um asterisco ou sublinhado antes e depois de uma palavra ou frase. Ex:

Texto &lowast;em itálico&lowast;.	

Texto  &#95;em itálico;&#95;.

## Negrito e Itálico

Para enfatizar o texto com negrito e itálico ao mesmo tempo, adicione três asteriscos ou sublinhados antes e depois de uma palavra ou frase. As citações podem ser aninhadas, com >> na frente do parágrafo que deseja aninhar.

Texto &lowast;&lowast;&lowast;em itálico e negrito&lowast;&lowast;&lowast;.	

Texto  &#95;&#95;&#95;em itálico e negrito&#95;&#95;&#95;.

## Citações em bloco
Para criar um *blockquote*, adicione um &gt; na frente de um parágrafo.

&gt; Texto em citação.

&gt; Outro texto em citação  
&gt;  
&gt; com várias linhas.

&gt; Exemplo de citação  
&gt;  
&gt;&gt; aninhada.

A saída renderizada é semelhante a esta:

> Texto em citação.

> Outro texto em citação
> 
> com várias linhas.

> Exemplo de citação  
>  
>> aninhada.

## Listas Ordenadas
Para criar uma lista ordenada (equivalente ao &lt;ol>&lt;li>), adicione itens de linha com números seguidos de pontos. Os números não precisam estar em ordem numérica, mas a lista deve começar com o número um.

Ex.

1&sdot; Primeiro item  
2&sdot; Segundo item  
3&sdot; Terceiro item  
&nbsp;&nbsp;&nbsp;1&sdot; Subitem

ou

1&sdot; Primeiro item  
1&sdot; Segundo item  
1&sdot; Terceiro item  
&nbsp;&nbsp;&nbsp;1&sdot; Subitem

Saída:

1. Primeiro item
1. Segundo item
1. Terceiro item
   1. Subitem

## Listas não ordenadas
Para criar uma lista não ordenada, adicione - , * ou + na frente dos itens de linha. Recue um ou mais itens para criar uma lista aninhada. Evite misturar os símbolos na mesma lista.

Ex:

&minus;	Primeiro item  
&minus; Segundo item  
&nbsp;&nbsp;&nbsp;&minus; Subitem

ou

&lowast;Primeiro item  
&lowast; Segundo item  
&nbsp;&nbsp;&nbsp;&lowast; Subitem

ou

&plus;	Primeiro item  
&plus; Segundo item  
&nbsp;&nbsp;&nbsp;&plus; Subitem

Saída:

- Primeiro item
- Segundo item
   - Subitem
   
### Adicionando Elementos em Listas
Para adicionar outro elemento em uma lista enquanto preserva a continuidade da mesma, indente o elemento quatro espaços ou uma tabulação. 

Ex:

*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.

Saída:

*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.



https://www.markdownguide.org/basic-syntax/
