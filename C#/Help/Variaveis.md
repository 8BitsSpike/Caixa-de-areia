# VARIÁVEIS

## DEFINIÇÃO DE VARIÁVEIS EM C#

C# usa uma definição de variável muito semelhante ao usado em JAVA, variáveis neste caso se refere a todo valor que vai ser "negociado" durante a execução do codigo.
Essa "negociação" pode ser leitura de um valor armazenado na memoria, leitura de um arquivo, entrada de um imput, computação de valores outros usando algum method ou valores absolutos definidos por padrão(Zero, Pi e etc).

Esse Valores são identificados por um tipo(type) e posição definida na memoria(mesmo os que são lidos de outros arquivos ou inceridos pelo usuário durante o uso do app), alguns podem mudar dinamicamente de valor, outros são fixos e alguns que servem apensas de "ponteira" já que só informam sobre a posição na memoria de algum valor.

## TIPOS(TYPES) DE VARIÁVEIS

Variáveis quando declaradas recebem uma definição de tipo(type), essas podem ser:

- `int` - armazena números INTEIROS, sem valores decimais, como 123 ou -123
- `float` - armazena números com virgula tendo de 6 até 9 casas decimais, como 	±1,5 x 10<sup>−45</sup> até ±3,4 x 10<sup>38</sup>
- `double` - armazena números com virgula tendo de 15 até 17 casas decimais, como ±5.0 × 10<sup>−324</sup> até ±1.7 × 10<sup>328</sup>
- `decimal` - armazena números com virgula tendo de 28 até 29 casas decimais, como ±1,0 x 10<sup>-28</sup> para ±7,9228 x 10<sup>28</sup>
- `char` - armazena um único charactere(letra), como 'a' ou 'B'. Variáveis Char são marcadas pelo tracinho(simple qoute) '
- `string` - armazena texto, como "Hello World". Variáveis String são marcadas por aspas(double quotes) " 
- `bool` - armazena valores nos estados verdade ou falso(true or false)

Cada um desses tipos de variável pode receber uma grande variedade de valores, no geral quando um valor é informado para C#, seja esse valor numérico ou não ele passa por uma uma "conversão assumida", ou seja, os valores são armazenados na memoria com o tipo mais seguro que C# entende que eles podem pertencer.

Por exemplo, no caso de números temos os seguintes casos:

```
int a = 42;
double b = a; // Implicit conversion de int para double (seguro)

float c = 3.14f;
double d = c; // Implicit conversion de float para double (seguro)

```
### HIERARQUIA DE CONVERSÕES IMPLÍCITAS

Abaixo temos uma sequência que determina quais conversões acontecem automaticamente:

sbyte → short → int → long → float → double
byte → short → ushort → int → uint → long → ulong → float → double
char → ushort → int → uint → long → ulong → float → double
decimal não convertem implicitamente para float nem double porque ele já tem maior precisão.

Para evitar ou contornar essa conversão podemos usar alguns metodos:

A. Usar Conversão Explicita (Casting)

Forçar a Conversão Explicita usando casts para evitar conversões implicitas naõ desejaveis:

```
double d = 5.75;
int x = (int)d; // Conversão Explicita (corta a parte decimal)
```

Usando o cast para definir qual o tipo de valor que precisamos antes dele ser informado muda o padrão como o número é avaliado dessa forma mantendo a integridade do valor.

B. Usar Specific Data Types na variáveu

Declarar variaveis com explicit data types:

```
decimal price = 12.99m; // Evita que ocorra conversão para double
```
O "m" no final do valor informa que este valor tem que permanecer como decimal, existem outros padrões usados para cada tipo de valor:

```
Os tipode de declaração específicas usam os sufixos:

O valor declarado sem sufixo ou com d ou D é do type double
O valor declarado com f ou F é do type float
O valor declarado com m ou M é do type decimal
```

C. Usando Convert Class

Use o Convert methods para controlar o como os valores são convertidos:

```
double d = 3.14;
int i = Convert.ToInt32(d); // Arredonda o valor invés de ignorar a parte decimal
```

D. Usar Parse() ou TryParse()

Se for lidar com input do usuário use string parsing para especificar o type:

```
string input = "42.5";
decimal value = decimal.Parse(input, System.Globalization.CultureInfo.InvariantCulture); // Converte o input usando o metodo descrito no atalho apontado
```