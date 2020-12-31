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

Saída:

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

1&#46; Primeiro item  
2&#46; Segundo item  
3&#46; Terceiro item  
&nbsp;&nbsp;&nbsp;1&#46; Subitem

ou

1&#46; Primeiro item  
1&#46; Segundo item  
1&#46; Terceiro item  
&nbsp;&nbsp;&nbsp;1&#46; Subitem

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

* Este é o primeiro item da lista.
* Este é o segundo item da lista.  
    &#62; Este é um recuo com citação
* Este é o terceiro item da lista.

Saída:

* Este é o primeiro item da lista.
* Este é o segundo item da lista.
    > Este é um recuo com citação
* Este é o terceiro item da lista.

Obs: Também é possivel aninhar uma lista não ordenada em uma lista ordenada ou vice-versa.


### Blocos de Código
Os blocos de código são normalmente recuados em quatro espaços ou uma tabulação (em listas, devem ser recuado oito espaços ou duas tabulações).

Ex:

1&#46; Passo um.  
2&#46; Passo dois.  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#60;html>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#60;head>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#60;title>Teste</title>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#60;/head>  

3&#46; Passo três.

Saída:

1. Passo um.
2. Passo dois.

        <html>
          <head>
            <title>Teste</title>
          </head>
          
3. Passo três.

## Imagens

Para adicionar uma imagem, adicione um ponto de exclamação (!), seguido pelo texto alternativo entre colchetes e o caminho ou URL para o recurso de imagem entre parênteses. Você pode opcionalmente adicionar um título após o URL entre aspas.

&#33;&#91;Imagem](&#47;caminho&#47;da&#47;imagem.png "titulo da imagem")

&#91;&#33;&#91;Imagem com link](&#47;caminho&#47;da&#47;imagem.jpg "titulo da imagem com link")](https://www.link.com)


## Código
Para marcar uma palavra ou frase como código, coloque-a entre crases (&#96;), equivalente à tag &#60;code>.

Ex:

Na linha de comando, digite &#96;comando&#96;.

&#96;&#96;Escapando o sinal de &#96;crase&#96; no meu arquivo.&#96;&#96;

Saída:

Na linha de comando, digite `comando`.

``Escapando o sinal de `crase` no meu arquivo.``

## Blocos de Código
Para criar blocos de código, indente cada linha do bloco em pelo menos quatro espaços ou uma tabulação. Outra maneira é usar blocos de código protegidos, usando três crases (&#96;&#96;&#96;) ou três tis (&#126;&#126;&#126;) nas linhas antes e depois do bloco de código. 

Ex:

&nbsp;&nbsp;&#60;tag1>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#60;tag2>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#60;/tag2>  
&nbsp;&nbsp;&nbsp;&#60;/tag1>  

ou 

&#96;&#96;&#96;  
{  
"nome": "Mateus",  
&nbsp;&nbsp;"sobrenome": "Smith",  
&nbsp;&nbsp;"idade": 41  
}  
&#96;&#96;&#96;

Saída:

    <tag1>  
      <tag2>  
      </tag2>  
    </tag1>  
    

```
{
  "nome": "Mateus",
  "sobrenome": "Smith",
  "idade": 41
}
```

## Linhas horizontais
Para criar uma linha ou régua horizontal, use três ou mais asteriscos (***), traços (---) ou sublinhados (___) em uma linha.

Ex:

&#42;&#42;&#42;

&#45;&#45;&#45;

&#95;&#95;&#95;&#95;&#95;&#95;&#95;&#95;&#95;

Saída:

---

##Links
Para criar um link, coloque o texto do link entre colchetes (por exemplo, [Página]) seguido com a URL entre parênteses (por exemplo, (https://pagina.com)). Para adicionar um título para o link (opcional), basta colocar entre aspas após o URL.

Ex:

<pre>Esta é a minha [Página](https://pagina.com "Titulo da pagina").</pre>

Saída:

Esta é a minha [Página](https://pagina.com "Titulo da pagina").

## URLs e endereços de e-mail
Para transformar rapidamente uma URL ou endereço de e-mail em um link, basta colocar entre < e >.

Ex:

&#60;https://www.pagina.com>
&#60;fake@example.com>

Saída:

<https://www.pagina.com>
<fake@example.com>

## Escapando caracteres
Para exibir um caractere literal que de outra forma seria usado para formatar texto em um documento Markdown, adicione uma barra invertida ( \) na frente do caractere.

Ex:

<pre>\*Sem a barra invertida, isso seria um marcador em uma lista não ordenada.</pre>

Saída:

\* Sem a barra invertida, isso seria um marcador em uma lista não ordenada.

## HTML
Muitos aplicativos Markdown permitem que você use tags HTML em texto formatado por Markdown. Usar HTML é útil quando você precisa alterar os atributos de um elemento, como especificar a cor do texto ou alterar a largura de uma imagem.

Ex:

<pre>This **word** is bold. This <em>word</em> is italic.</pre>

Saída:

This **word** is bold. This <em>word</em> is italic.

Por razões de segurança, nem todos os aplicativos Markdown suportam HTML em documentos Markdown, portanto em caso de dúvida, verifique a documentação do aplicativo Markdown. Alguns aplicativos suportam apenas um subconjunto de tags HTML. Porém, evite misturar a sintaxe Markdown dentro de tags HTML, como <pre><p>italico e **negrito**</p>.</pre>

Referência: https://www.markdownguide.org/basic-syntax/
