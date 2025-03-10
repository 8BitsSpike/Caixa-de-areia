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

Linha 1: using System significa que estaremos usando uma classes vinda do System namespace.

Linha 2: namespace é usado para organizar o codigo e os seus containers para classes.

Linha 3: definimos oque iremos criar, neste caso uma classe, e seu nome.

Linha 4: aqui definimos o que nosso codigo pode fazer, onde ele tem "dominio" e o ripo de retorno, se algum, que ele fornece e quais são as entradas que ele recebe.

Linha 5: por fim definimos o que nosso codigo faz, o "codigo" em sí.

Essa extrutura é bem prática e facil de ler, algumas regras devem ser seguidas para manter sua legibilidade, funcionalidade e o seu bom funcionamento.


