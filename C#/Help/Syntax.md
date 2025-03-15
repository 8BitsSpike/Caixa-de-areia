# SYNTAX

## CARACTERÍSTICAS DA LINGUAGEM

- Declarações terminam em ";" assim como em JAVA
- C# é sensivel a diferença de letras maiúsculas e minusculas
- Diferente de JAVA classes não precisam ter o memo nome que o arquivo, embora muitas vezes seja usado o mesmo nome por motivo de organização.

## COMO CRIAR COMENTÁRIOS

- Comentários em C# podem ser escritos em linha usando "//" ou em linhas multiplas usando "/_" e "_/"

## EXTRUTURA E SEMELHANÇAS

- C# tem uma extrutura muito semelhante a JAVA, C++ e outras linguagens voltadas para Objeto

Exemplo de codigo em C#:
```

using System;

namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      Console.WriteLine("Hello World!");    
    }
  }
}
```
Linha 1: using System significa que vamos usar uma classe vinda do System namespace.

Linha 2: namespace é usado para organizar o código e os seus containers para classes.

Linha 3: definimos o que iremos criar, neste caso uma classe, e seu nome.

Linha 4: aqui definimos o que o nosso código pode fazer, onde ele tem "domínio" e o ripo de retorno, se algum, que ele fornece e quais são as entradas que ele recebe.

Linha 5: por fim definimos o que o nosso código faz, o "código" em sí.

Essa estrutura é bem prática e fácil de ler, algumas regras devem ser seguidas para manter a legibilidade, funcionalidade e o seu bom funcionamento.

## ELEMENTOS SEMÂNTICOS DA PROGRAMAÇÃO EM C#

Os elementos semânticos da linguagem C# seguem a mesma extrutura das linguagens de programação atual, as linhas de código são chamadas declarações, usamos variáveis para apontar valores, fazemos computação de funções que verificam operadores logicos em valores pré-definidos, usamos chaves, couchetes e parenteses para compor a logica de nossas declarações e, por ser uma linguagem orientada a objetos, temos classes, methodos e objetos.

 - Entendendo os Elementos Semânticos:

### Objetos e linguagens voltadas a eles

Para entendermos o que é uma linguagem orientada a objeto devemos entender o que são objetos e como são as linguagens não voltadas a eles.
Chamamos de programação precedural a forma de programar que monta o código com logica como foco, esse tipo de programação cria algoritimos que trata dados e oferece a resposta. ela é bem objetiva e normalmente é a primeira que aprendemos já que ela iguala a forma como passamos instruções para as varias atividades do dia à dia.
Já as linguagens voltadas a objetos são montadas como um livro de matemática, elas contem as instruções de o que fazer com os dados e os dados em pacotes que chamamos objetos.

>O que são objetos?

Objetos são pacotes de informação, eles podem contem dados e algoritimos, em geral os objetos são associados a uma classe que os define. 

>O que são classes?

Classes são um conjunto de regras que defino o formato de um objeto, podemos comparar classes com a descrição objetiva de algo, por exemplo, bananas são frutas longas, pouco humidas, cultivadas nos trópicos, de cor amarela e que são produzidas em caixos.
Nesse exemplo definimos o que são bananas, quando precisarmos de uma banana podemos pedir/associar ela com a definição que criamos.
Mas como podemos associar um algoritimo a um objeto? nesse caso basta imaginar que a descrição do funcionamento do objeto é parte da descrição, por exeplo, armas de fogo são ferramentas metalicas, com um cilindro para munição, um cano metálico alongado, um gatilho, quando pressionamos o gatilho a monição é deflagrada e o projétil(parte componente da munição) é projetado com alta velocidade para fora da arma seguindo a trajetória definida pelo cilindro.

Desta forma podemos dizer que uma linguagem voltada a objetos é uma linguagem que cria classes para resolver situações em vez de propor um conjunto completo de regrar sempre.

Para esse objetivo usamos algumas regras como o 'DRY' Don't Repeat Yourself(não se repita) que é uma regra muito útil já que ela orienta o programador a MODULARIZAR seu código.

### Variáveis

C# usa uma definição de variável muito semelhante ao usado em JAVA, variáveis neste caso se refere a todo valor que vai ser "negociado" durante a execução do codigo.
Essa "negociação" pode ser leitura de um valor armazenado na memoria, leitura de um arquivo, entrada de um imput, computação de valores outros usando algum method ou valores absolutos definidos por padrão(Zero, Pi e etc).

Esse Valores são identificados por um tipo(type) e posição definida na memoria(mesmo os que são lidos de outros arquivos ou inceridos pelo usuário durante o uso do app), alguns podem mudar dinamicamente de valor, outros são fixos e alguns que servem apensas de "ponteira" já que só informam sobre a posição na memoria de algum valor.

### FUNÇÕES

Funções em C# seguem a mesma definição que em outras linguagens, são um conjunto de procedimentos/regras que usamos para tratar valores para obter um resultado esperado, este pode ser repetido indefinidamente e sempre teremos o mesmo resultado ou formato de resultado.

Seguindo esta definição podemos comparar funções com as instruções que damos/aprendemos quando estamos ensinando/fazendo/aprendendo algo, como tocar musica, lavar louça, dançar e etc.

### DECLARAÇÕES CONDICIONAIS

declarações condicionais, ou estruturas condicionais, são blocos de código que permitem que um programa tome decisões e execute diferentes ações dependendo de uma condição específica, essas decisões são baseadas em operadores que podem ser lógicos, aritiméticos, designadores e comparadores.

### OPERADORES LÓGICOS

Operadores lógicos são símbolos ou palavras que comparam dois ou mais valores, permitindo a combinação de testes relacionais em uma comparação. Eles são usados para criar expressões lógicas que podem ser verdadeiras ou falsas. 

>Quais são estes operadores?

`AND`: Significa que todos os valores de procura devem ser satisfeitos para que um documento seja incluído nos resultados<br>
`OR`: Significa que pelo menos um dos valores de procura deve ser satisfeito para que um documento seja incluído nos resultados<br>
`NOT`: Realiza uma negação lógica de um único operando<br>
`XOR`: Ambos os operandos da expressão são sempre avaliados<br>

### OPERADORES ARITIMÉTICOS

Operadores aritméticos são símbolos que realizam operações matemáticas, como adição, subtração, multiplicação, divisão e resto da divisão. Eles são usados em conjunto com variáveis e valores constantes para criar expressões. 

>Quais são estes operadores?

`Unários`: executam uma ação com um único operando<br>
`Binários`: executam ações com dois operandos<br>

Exemplos de operadores aritméticos Soma `+`, Subtração `-`, Multiplicação `*`, Divisão `/`, Resto da divisão `%`.

### OPERADORES DESGINADORES

Operadores de desginadores ou de designação/atribuição são símbolos que atribuem um valor a uma variável, utilizando o sinal de igual `=` como operador principal.

### OPERADORES COMPARADORES

Operadores comparadores/comparativos, também conhecidos como operadores relacionais, são símbolos que permitem comparar dois valores e retornam True (verdadeiro) ou False (falso) dependendo do resultado da comparação.

Um bom exemplo de uso deles é o operador ternário que define uma variável,
podemos em poucas linhas declarar uma serie de situações como condição para uma única variável.

>Quais são estes operadores?

`==` - Igual a - Verifica se dois valores são iguais<br>
`!=` - Diferente de - Verifica se dois valores são diferentes<br>
`>` - Maior que - Verifica se o valor à esquerda é maior que o valor à direita<br>
`<` - Menor que - Verifica se o valor à esquerda é menor que o valor à direita<br>
`>=` - Maior ou igual a - Verifica se o valor à esquerda é maior ou igual ao valor à direita<br>
`<=` - Menor ou igual a - Verifica se o valor à esquerda é menor ou igual ao valor à direita<br>