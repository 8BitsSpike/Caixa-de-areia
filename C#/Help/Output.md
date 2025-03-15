# OUTPUT

## TIPOS DE OUTPUT

Em C#, assim como me várias outras linguagens modernas, podemos produzir output de duas formas, "imprimindo" um valor na tela ou "escrevendo" em um documento/arquivo.

### OUTPUT EM TELA

Em C# usamos dois methodos para escrever algo na tela:

`WriteLine()` - escreve uma ou mais linhas e encerra com uma quebra de linha
`Write()` - escreve uma ou mais linhas mas não encerra com uma quebra de linha

- Semantica de uso

Para usar os methodos listados basta informar onde a linha deve ser escrita, por exemplo:

`Console.Write("Hello World! ");` - Neste caso o texto vai ser escrito no console

### OUTPUT EM ARQUIVO

Para acessarmos arquivo e podermos modificalo precimamos da classe `FILE`.

A classe `FILE` tem muitos methodos úteis como:

- Manipulação de Arquivos

`File.Create(string path)`: Cria um novo arquivo no caminho especificado.<br>
`File.Delete(string path)`: Exclui o arquivo especificado.<br>
`File.Exists(string path)`: Verifica se um arquivo existe.<br>
`File.Move(string sourceFileName, string destFileName)`: Move um arquivo para um novo local.<br>
`File.Copy(string sourceFileName, string destFileName)`: Copia um arquivo para um novo local.<br>
`File.Replace(string sourceFileName, string destinationFileName, string destinationBackupFileName)`: Substitui um arquivo por outro e cria um backup do original.<br>
`File.ReadAllText(string path)`: Lê todo o conteúdo do arquivo e retorna uma string.<br>
`File.ReadAllLines(string path)`: Lê todas as linhas do arquivo e retorna um array de strings.<br>
`File.ReadAllBytes(string path)`: Lê todo o conteúdo do arquivo e retorna um array de bytes.<br>
`File.WriteAllText(string path, string contents)`: Escreve uma string em um arquivo, sobrescrevendo se ele já existir.<br>
`File.WriteAllLines(string path, string[] contents)`: Escreve um array de strings em um arquivo, sobrescrevendo se ele já existir.<br>
`File.WriteAllBytes(string path, byte[] bytes)`: Escreve um array de bytes em um arquivo.<br>
`File.AppendText(string path)`: Abre um arquivo para escrita e adiciona conteúdo ao final.<br>
`File.Open(string path, FileMode mode)`: Abre um arquivo no modo especificado e retorna um FileStream.<br>
`File.OpenRead(string path)`: Abre um arquivo para leitura e retorna um FileStream somente leitura.<br>
`File.OpenWrite(string path)`: Abre um arquivo para escrita e retorna um FileStream somente gravação.<br>
`File.CreateText(string path)`: Cria um novo arquivo e retorna um StreamWriter para escrita de texto.<br>
`File.AppendText(string path)`: Abre um arquivo existente para escrita e retorna um StreamWriter para adicionar texto.<br>
`File.GetAttributes(string path)`: Obtém os atributos do arquivo.<br>
`File.SetAttributes(string path, FileAttributes attributes)`: Define os atributos do arquivo.<br>
`File.GetCreationTime(string path)`: Obtém a data/hora de criação do arquivo.<br>
`File.SetCreationTime(string path, DateTime creationTime)`: Define a data/hora de criação do arquivo.<br>
`File.GetLastAccessTime(string path)`: Obtém a data/hora do último acesso ao arquivo.<br>
`File.SetLastAccessTime(string path, DateTime lastAccessTime)`: Define a data/hora do último acesso ao arquivo.<br>
`File.GetLastWriteTime(string path)`: Obtém a data/hora da última modificação do arquivo.<br>
`File.SetLastWriteTime(string path, DateTime lastWriteTime)`: Define a data/hora da última modificação do arquivo.<br>

Para nosso uso em OUTPUT 