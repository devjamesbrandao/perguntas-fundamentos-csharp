### Perguntas e respostas sobre os fundamentos do C#

1. O C# é uma linguagem compilada, tipada e gerenciada, o que isto significa?
> Linguagem compilada significa que ela precisa de um <strong>Compilador</strong> para tansformar o <strong>Código-fonte</strong> em um <strong>Arquivo binário</strong> executável pelo <strong> Sistema Operacional</strong> de destino (Mac, Windows, Linux). Já a linguagem tipada refere-se ao uso de variáveis, classes e métodos com tipos específicos (int, string, decimal). Por fim, gerenciada significa que sua execução depende de um gerenciador (também é conhecido como Runtime). No caso do C# quem faz este gerenciamento é o <strong>CLR (Common Language Runtime)</strong>. O CLR gerencia serviços importantes como gestão de memória, segurança entre outros.

2. O que diferencia uma linguagem compilada de uma interpretada?
> A linguagem compilada precisa converter o nosso <strong>código-fonte</strong> inteiro para <strong>linguagem de máquina</strong> de uma só vez através de um programa chamado <strong>compilador</strong>. Nesse caso, o usuário recebe o código pronto para ser executado. Já a linguagem interpretada interpreta o <strong>código-fonte</strong> em partes por meio de um programa chamado <strong>interpretador</strong>, que irá então converter nosso código para <strong>linguagem de máquina</strong>. Assim, é necessário que o código seja interpretado e convertido para o cliente e então executado (o código não vem pronto igual ocorre na linguagem compilada). 

3. Explique como o C# funciona
> Primeiro o código em C# é compilado para a Intermediate Language (IL). Depois o CLR pega o IL e compila-o para código nativo do sistema operacional, ou seja, código executável.

4. O que é o CLR?
> O <strong>CLR (Common Language Runtime)</strong> é o gerenciador da linguagem C#. O CLR recebe o código gerenciado, compila-o em código que a máquina entenda e o executa. Além disso, o CLR é responsável pela gestão de memória, segurança, entre outros. Assim, podemos concluir que o CLR é a infraestrutura responsável pela execução do programa

5. O que é IL?
> IL é a <strong>Intermediate Language</strong>, ou seja, é uma linguagem intermediária gerada pelos compiladores que pretendem rodar em cima do CLR. O compilador compila o código-fonte e o transforma em IL.

6. O que é um Framework?
> O <strong>Framework</strong> é uma estrutura composta por um conjunto de bibliotecas e códigos genéricos que permitem o desenvolvimento de sistemas e aplicações. Um framework funciona como uma espécie de template o qual oferece certos artifícios estruturais básicos para criação de alguma aplicação ou software.

6. O que é o .NET?
> O <strong>.NET</strong> é uma plataforma de desenvolvimento atualmente open-source, criada pela Microsoft, e que é composta por uma biblioteca padrão, um compilador e uma máquina virtual. Esses componentes da plataforma possibilitam a criação de códigos em algumas linguagens, como C#, VB.NET e F#.

7. O que é o .NET Standard?
> <strong>.NET Standard</strong> é uma especificação formal de APIs .NET que estão disponíveis em várias implementações .NET. A motivação por trás do .NET Standard foi estabelecer maior uniformidade no ecossistema .NET.

8. Explique o que é versão semântica
> A <strong>versão semântica</strong> é uma convenção formal para determinar o número de versões de novos lançamentos de software. A norma ajuda os utilizadores de software a compreender a gravidade das mudanças em cada nova distribuição. Um projeto que utiliza a versão semântica deve possuir um número <strong>Maior (Major number)</strong>, <strong>Menor (Minor number)</strong> e de <strong>correção (Patch number)</strong> para cada lançamento. Por exemplo, a versão `1.2.3` indica uma versão maior de 1, uma versão menor de 2 e um número de correção de 3.

9. O que significa LTS na versão do software?
> <strong>LTS</strong> significa apoio a longo prazo. Aqui, apoio significa que ao longo da vida de um lançamento há um compromisso de atualizar, corrigir e manter o software. Para um LTS, existe um ciclo de desenvolvimento mais curto, onde engenheiros e colaboradores acrescentam ao corpo da versão.

10. O que é um Runtime?
> <strong>Runtime</strong> descreve software/instruções que são executadas enquanto o programa está em execução, especialmente as instruções que não são escritas explicitamente, mas que são necessárias para a execução adequada do código.

11. O que é um SDK?
> <strong>SDK</strong> significa kit de desenvolvimento de software ou <strong>devkit</strong> para abreviar. É um conjunto de ferramentas e programas de software utilizados pelos programadores para criar aplicações para plataformas específicas. As ferramentas SDK incluem uma gama de coisas, incluindo bibliotecas, documentação, amostras de código, processos e guias que os programadores podem utilizar e integrar nas suas próprias aplicações. Os SDK são concebidos para serem utilizados em plataformas ou linguagens de programação específicas.

12. O que é um CLI?
> <strong>CLI</strong> significa <strong>Command Line Interface</strong> ou <strong>Interface de linha de comando</strong>. CLI é um programa de linha de comando que aceita a entrada de texto para executar funções do sistema operacional. Por exemplo, o gerenciador de pacotes <strong>NPM</strong> utiliza linha de comando para instalar componentes necessários ao desenvolvimento de software.

13. Cite 3 tipos de projetos que temos no .NET?
> <strong>Biblioteca de classes</strong>, <strong>Aplicativo Console</strong>, <strong>Aplicativo WEB ASP.NET Core</strong> e <strong>API WEB ASP.NET Core</strong>.

14. O que é uma Solution?
> Uma <strong>solução</strong> uma espécie de container de trabalho que contém uma coleção de projetos, juntamente com informações sobre as dependências entre esses projetos.

15. Qual comando para executar uma aplicação .NET?
> dotnet run

16. Qual comando para compilar uma aplicação .NET?
> dotnet build

17. Qual comando para publicar uma aplicação .NET?
> dotnet publish

18. Qual nome do método principal de um Console App?
> Main()

19. O que significa Debug?
> <strong>Debug</strong> ou <strong>Depuração</strong> é o processo de detecção e remoção de erros existentes ou potenciais (também chamados de 'bugs') num código de software que pode causar o seu comportamento inesperado ou a sua queda. Para evitar o funcionamento incorrecto de um software ou sistema, a depuração é utilizada para encontrar e resolver bugs ou defeitos.

20. Como executamos uma aplicação .NET em modo Debug?
> No <strong>Visual Studio Code</strong> é necessário adicionar uma pasta chamada <strong>.vscode</strong>. Ela contém dois arquivos: <strong>launch.json</strong> e <strong>task.json</strong>. Esses dois arquivos são importantes para executar comandos como dotnet build e publish. Além disso, graças a eles conseguimos executar o debug da nossa aplicação. Para isso, depois de adicionar a pasta e os arquivos anteriormente mencionados, precisamos adicionar <strong>breakpoints</strong> nos trechos de códigos os quais queremos debugar. Feito isso, basta clicar em <strong>F5</strong>, assim o debug será executado. Já no caso do <strong>Visual Studio</strong>, o processo e mais simples, pois basta adicionar os <strong>breakpoints</strong> no código e, após isso, clicar em <strong>F5</strong>.

21. Qual a finalidade da pasta Properties?
> A pasta <strong>Properties</strong> contém um arquivo chamado <strong>launchSettings.json</strong> que contém toda a informação necessária para iniciar a aplicação. Contém também os perfis através dos quais a aplicação pode ser executada, cada perfil é mapeado para um <strong>commandName</strong>, <strong>applicationUrl</strong> em que a aplicação é lançada, <strong>environmentVariables</strong>, etc.

22. Qual a finalidade das pastas Bin e Obj?
> O diretório <strong>obj</strong> é para ficheiros de objetos intermediários e outros ficheiros de dados transitórios que são gerados pelo compilador ou sistema de construção durante uma construção. O diretório <strong>bin</strong> é o diretório onde serão escritos os binários de saída final (e quaisquer dependências ou outros ficheiros destacáveis).

23. Quais partes compoe um programa em C#?
> A estrutura de um programa em C# pode ser dividida em um ou mais arquivos contendo os seguintes elementos:
> - Namespaces;
> - Tipos (classes, estruturas, interfaces, delegações, enums);
> - Membros (constantes, campos, métodos, propriedades, indexadores, eventos, operadores, construtores);
> - Outros (declarações, comentários, instruções).

24. O que são Namespaces?
> A palavra-chave <strong>namespace</strong> é utilizada para declarar um âmbito que contém um conjunto de objetos relacionados. Pode usar um namespace para organizar elementos de código e para criar tipos únicos a nível global da aplicação. Dentro de um espaço de nomes, pode declarar zero ou mais dos seguintes tipos: 
> - classes;
> - Interfaces;
> - Structs;
> - Enum;
> - Delegate;

25. Qual a finalidade do Using?
> Em C#, a utilização da palavra-chave <strong>using</strong> tem dois objetivos: a primeira é a diretiva de utilização, que é utilizada para importar namespaces no topo de um arquivo de código. A segunda é a declaração de utilização. No C# 8, utilizar declarações <strong>using</strong> asseguram que as classes que implementam a interface IDisposable chamem o seu método de Dispose.

26. Qual a diferença entre uma variável e uma constante?
> Uma <strong>variável</strong> é como um recipiente que contém os valores ou dados de um determinado tipo de dados que ajudam a executar o programa. O valor de uma variável <strong>pode mudar</strong> dependendo das condições ou informações dadas no tempo de execução do programa. Já a <strong>constante</strong> é um valor fixo cujo valor <strong>não pode ser alterado</strong> durante a execução do programa ou uma vez que o valor é definido.

27. Cite 3 nomes reservados que temos no C#
> abstract, var, private, switch, etc.

28. Quais formas temos de comentar código em C#?
> No C#, há 3 tipos de comentários: comentário de linha única (//), comentário de várias linhas (/* */) e comentários em XML (///).

29. O que são tipos primitivos?
> Os mais famosos tipos primitivos são: <strong>int, object, short, char, float, double, char, bool</strong>. Eles são chamados de primitivos porque eles são os principais <strong>built-in types</strong> (fazem parte do C# nativamente), e podem ser usados para construir outros tipos de dados (structs).

30. Qual tipo base no .NET?
> A classe <strong>Object</strong> é a base para todas as classes do .NET. Ela está presente no namespace <strong>System</strong>.

31. Dado um var de um número real, qual tipo seria o var?
> var seria do tipo Double

32. Dado um var de um número inteiro, qual tipo seria o var?
> var seria do tipo Int32

33. Qual a diferença entre char e string?
> A principal diferença entre <strong>Char</strong> e <strong>String</strong> é que char se refere a uma única letra, número, espaço, sinal de pontuação ou um símbolo que pode ser representado utilizando um caractere enquanto string se refere a um conjunto de caracteres.

34. Qual valor padrão do tipo char?
> O valor por padrão do tipo char é <strong>\0</strong> , ou seja, <strong>U+0000</strong>.

35. Qual a diferença entre var e object?
> Tudo é <strong>object</strong> porque é um tipo de base para cada tipo no .NET. Por exemplo, <strong>int</strong> herda de <strong>object</strong>. O <strong>var</strong> é usado para definição implícita do tipo das variáveis, uma vez que o compilador se encarrega de descobrir o tipo da variável. Além disso, não é possível iniciar uma variável com <strong>var</strong> e não atribuir valor a ela, exemplo: 
```
// Compilador lança um erro
var nome; 
```
> Entretanto, o compilador permite você definir uma variável com o tipo <strong>object</strong> e não atribuir valor a ela, exemplo:
```
// O compilador permite tranquilamente
object nome;
```

36. O que são tipos nulos?
> O tipo <strong>Nullable</strong> ou <strong>tipo nulo</strong> permite atribuir um valor nulo a uma variável.

37. O que são alias? Cite 3 exemplos
> <strong>Alias</strong> tem a função de evitar ambiguidades e facilitar a importação de namespaces e structs. O <strong>char</strong> é um alias para o struct <strong>System.Char</strong>. <strong>int</strong> é um alias para o struct <strong>Int32</strong>. <strong>string</strong> é um alias para <strong>System.String</strong>.

38. O que são conversões implícitas?
> <strong>Conversões implícitas</strong> não precisam de sintaxe especial porque a conversão é sempre bem sucedida e nenhum dado será perdido. Exemplo:
```
// O tipo int possui 32 bits
int num = 2147483647;
// O tipo long possui 64 bits. Portanto, é possível realizar a conversão implícita de int para long sem perca de dados
long bigNum = num;
```

39. O que são conversões explícitas?
> <strong>Conversões explícitas (casts)</strong> requerem uma <strong>cast expression</strong>. O <strong>Casting</strong> é necessário quando a informação pode ser perdida na conversão, ou quando a conversão pode não ser bem sucedida por outras razões. Exemplo:
```
double x = 1234.7;

int a;

// Cast double para int utilizando expressão cast (o int antes da variável x é o casting)
a = (int)x;
```

40. Qual a diferença entre parse e Convert?
> O <strong>Parse</strong> não aceita valor nulo na conversão, mas o <strong>Convert</strong> aceita. Por exemplo, <strong>Parse</strong> e <strong>Convert</strong> para <strong>Int32</strong> são dois métodos para converter uma string para um número inteiro. A principal diferença entre int Parse e Convert para Int32 em C# é que passando um valor nulo para int Parse lançará um ArgumentNullException enquanto que passando um valor nulo para Convert ToInt32 dará zero.

41. O que são operadores aritméticos e quais temos no C#?
> Os <strong>operadores aritméticos</strong> são utilizados para realizar operações matemáticas comuns. São eles:
> - Adição: +
> - Subtração: -
> - Multiplicação: *
> - Divisão: /
> - Módulo (o famoso resto da divisão): %
> - Incremento: ++
> - Decremento: --

42. O que são operadores de atribuição e quais temos no C#?
> Os <strong>operadores de atribuição</strong> são utilizados para atribuir valores a variáveis. São eles:
> - = 
> - += 
> - -=
> - *=
> - /=
> - %=
> - &=
> - |=
> - ^=
> - \>\>=
> - <<=

43. O que são operadores de comparação e quais temos no C#?
> Os <strong>operadores de comparação</strong> são utilizados para comparar dois valores. São eles:
> - ==
> - !=
> - \>
> - <
> - \>=
> - <=

44. O que são operadores lógicos e quais temos no C#?
> Os <strong>operadores lógicos</strong> são utilizados para determinar a operação lógica entre variáveis ou valores. São eles:
> Operação lógica AND: &&
> Operação lógica OR: ||
> Operação lógica NOT: !

45. Cite duas estruturas condicionais que temos no C#
> `if()` e `switch()`

46. Cite duas estruturas de repetição que temos no C#
> `for()` e `while()`

47. Qual a diferença entre while e do/while?
> Enquanto o laço de repetição <strong>while</strong> verifica primeiro a condição e depois executa a(s) declaração(ões), o laço <strong>do while</strong> executa a(s) declaração(ões) pelo menos uma vez, depois verifica a condição.

48. Como definimos que um método não retorna valor algum?
> Adicionamos a palavra <strong>void</strong> no retorno do método. Exemplo:
```
public void MetodoVoid()
{
  Console.WriteLine("Hola, compañeros soy un método sin retorno");
}
```

49. Podemos ter métodos sem parâmetros no C#?
> Sim, tranquilamente. Exemplo:
```
public List<Produto> ObterTodosOsCandidadosAPresidente()
{
  return new List<string>(6){ "Jair Bolsonaro", "Lula", "Ciro Gomes", "Simone Tebet", "Luiz Felipe d’Avila", "Soraya Thronicke" };
}
```

50. Como tornamos um parâmetro opcional no C#?
> Devemos adicionar um valor padrão no parâmetro do método. Exemplo:
```
public void AumentarSalarioDoDev(decimal valorAumento = 2000)
{
  SalarioDoDev += valorAumento;
}
```

51. O que são heap e stack?
> São áreas da memória RAM onde o processador busca dados da aplicação.

52. O que são tipos de valor e tipos de referência?
> Ao atribuir um valor a uma variável que seja do <strong>tipo de valor</strong>, você está armazenando uma instância desse tipo na memória. Ao atribuir essa variável a uma outra variável desse mesmo tipo, acontece uma cópia do valor. Diferentemente das variáveis de tipo de valor, ao iniciar uma variável do <strong>tipo de referência</strong> além de ser alocado um espaço na memória para armazenar o conteúdo atribuído, a variável iniciada é armazenada em um outro espaço de memória, onde existe uma referência para a primeira posição de memória do conteúdo. Isso significa que ao atribuir uma variável do tipo de referência a outra, apenas o valor da referência é copiado.

53. Onde são armazenados os tipos de valor?
> As variáveis do <strong>tipo valor</strong> são armazenadas na memória <strong>stack</strong>.

54. Onde são armazenados os tipos de referência?
> As variáveis do <strong>tipo referência</strong> são armazenadas na memória <strong>heap</strong>.

55. O que são Structs?
> Em C#, <strong>struct</strong> é o tipo de dado de valor que representa as estruturas de dados. Pode conter um construtor parametrizado, construtor estático, constantes, campos, métodos, propriedades, indexadores, operadores, eventos e tipos aninhados.

56. O que são enumeradores?
> Na linguagem C#, <strong>enum</strong> é um tipo de valor definido pelo usuário usado para representar uma lista de constantes inteiras nomeadas. Ele é criado usando a palavra-chave <strong>enum</strong> dentro de uma classe, estrutura ou espaço de nomes. Ele melhora a legibilidade, a manutenção e reduz a complexidade de um programa.

57. O que é um GUID?
> <strong>GUID</strong> significa <strong>Global Unique Identifier (Identificador Único Global)</strong>. Um GUID é um inteiro de 32 bits (16 bytes) que você pode usar em todos os computadores e redes onde quer que um identificador único seja necessário. Exemplo de GUID no C#: <strong>0f8fad5b-d9cb-469f-a165-70867728950e</strong>

58. O que é interpolação de String?
> A interpolação de string em C# é um método de concatenação, formatação e manipulação de string. Exemplo:
```
var estadosBrasileiros = 27;

Console.WriteLine($"O Brasil é composto por {estadosBrasileiros} estados");

```

59. Qual a finalidade do método CompareTo?
> O método <strong>Int16.CompareTo()</strong> em C# é usado para comparar a instância de um objeto com outro objeto especificado ou outra instância Int16 e retorna um inteiro que indica se o valor desta instância é menor, igual ou maior que o valor do objeto especificado ou da outra instância Int16.

60. Qual a finalidade do método Contains?
> O método Contains() em C# é usado para retornar um valor indicando se uma substring específica ocorre dentro de outra string. Exemplo:
```
var fruta = "Abacaxi";

if(fruta.Contains("xi"))
{
  Console.WriteLine("Sim");
}
else
{
  Console.WriteLine("Não");
}
```

61. Qual a finalidade do método StartsWith e EndsWith?
> O método <strong>StartsWith</strong> verifica se uma palavra começa com determinada letra. Já o método <strong>EndsWith</strong> verifica se uma palavra termina com determinada letra.

62. Qual a finalidade do método Equals?
> Em C#, <strong>Equals(String, String)</strong> é um método String. É usado para determinar se dois objetos String têm ou não o mesmo valor. Basicamente, ele verifica a igualdade. Se ambas as strings têm o mesmo valor, ele retorna verdadeiro, caso contrário, retorna falso.

63. Qual a finalidade do método IndexOf e LastIndexOf?
> O método <strong>IndexOf()</strong> retorna o número de índice do primeiro caractere correspondente, enquanto que o método <strong>LastIndexOf()</strong> retorna o número de índice do último caractere correspondente.

64. Qual a finalidade do método ToLower e ToUpper?
> O método <strong>ToLower()</strong> coloca os caracteres de uma string ou char em caixa baixa. Já o método <strong>ToUpper</strong> colocar os caracteres de uma string ou char em caixa alta.

65. Qual a finalidade do método Insert?
> O método <strong>Insert()</strong> em C# é usado para retornar uma nova string na qual uma string especificada é inserida em uma posição de índice especificada neste caso. 

66. Qual a finalidade do método Length?
> <strong>String Length</strong> em C# retorna o número de caracteres de uma string. Além disso, o método <strong>Length</strong> também pode ser utilizado para contar a quantidade de itens de um array. Exemplo com string:
```
string palavra = "Docker";
int tamanhoPalavra = palavra.Length;
Console.WriteLine("A palavra " + palavra + " possui " + tamanhoPalavra + "letras.");
```

67. Qual a finalidade do método Remove?
> No C#, o método <strong>Remove()</strong> é um método String. Ele é usado para remover todos os caracteres da posição especificada de uma string. Se o comprimento não for especificado, então ele removerá todos os caracteres após a posição especificada. Além disso, o método Remove() também pode ser utilizado para remover elementos de uma lista.

68. Qual a finalidade do método Replace?
> Em C#, o método <strong>Replace()</strong> é um método de string. Este método é usado para substituir todos os caracteres Unicode especificados ou string especificada do objeto string atual e retorna uma nova string modificada. Este método pode ser sobrecarregado ao passar argumentos para ele.

69. Qual a finalidade do método Split?
> Em C#, <strong>Split()</strong> é um método de classe de string. O método <strong>Split()</strong> retorna um conjunto de string geradas pela divisão da string original separada pelos delimitadores passados como um parâmetro no método Split(). Os delimitadores podem ser um caractere ou um array de caracteres ou um array de cadeias de caracteres.

70. Qual a finalidade do método Substring?
> O método <strong>Substring()</strong> em C# é usado para recuperar um substring da string atual, ou seja, retorna um "pedaço" da string atual. O substring começa em uma posição de caracteres especificada e continua até o final da string.

71. Qual a finalidade do método Trim?
> O método <strong>String Trim()</strong>, geralmente, é utilizado para remover os espaçamentos em branco no início e no fim da string.

72. O que é StringBuilder e quando devemos utilizar?
> Em c#, <strong>StringBuilder</strong> é uma classe que é útil para representar uma sequência <strong>mutável</strong> de caracteres, e é um objeto do namespace <strong>System.Text</strong>. Em c#, tanto <strong>string</strong> quanto <strong>StringBuilder</strong> representarão uma sequência de caracteres e executarão o mesmo tipo de operações, mas a única diferença é que as <strong>strings</strong> são <strong>imutáveis</strong>, e <strong>StringBuilder</strong> é <strong>mutável</strong>.<br />
> Geralmente, em c# a <strong>string</strong> não pode ser modificado uma vez que é criada. Se alguma alteração for feita na string, como adicionar ou modificar um valor existente, ela simplesmente descartará a instância antiga na memória e criará uma nova instância para manter o novo valor. Se fizermos modificações repetidas no objeto string, isso afetará o desempenho do aplicativo. Para resolver esse problema, o c# introduziu uma alternativa chamada <strong>StringBuilder</strong>, que é uma classe de string <strong>mutável</strong>. Mutabilidade significa que uma vez criada uma instância da classe, a mesma instância será usada para executar quaisquer operações como inserir, appending, remover ou substituir os caracteres em vez de criar uma nova instância para cada vez.

73. O que é Regex e quando devemos utilizar?
> Em C#, <strong>Expressão Regular</strong> é um padrão que é usado para analisar e verificar se o texto de entrada dado está combinando com o padrão dado ou não. Em C#, as Expressões Regulares são geralmente chamadas de C# <strong>Regex</strong>. O .Net Framework fornece um mecanismo de expressão regular que permite a correspondência do padrão. Os padrões podem consistir de quaisquer caracteres literais, operadores ou construtores. 

74. O que é o DateTime?
> O <strong>DateTime</strong> no C# é um tipo de dados <strong>struct</strong>. Com isto sabemos que ele é composto por outros tipos e métodos, além de ser iniciado com um valor padrão. O <strong>DateTime</strong> ajuda o desenvolvedor a descobrir mais informações sobre Data e Hora como obter mês, dia, ano, dia da semana. Também ajuda a encontrar diferença de data, adicionar número de dias a uma data, etc.

### ` 🌐 Referências`
- <p> Perguntas para entrevista de C# e .NET: https://balta.io/blog/perguntas-entrevista-csharp</p>

- <p> C#: Tipos de Valor e Tipos de Referência: https://calegari.dev/posts/c-sharp-tipos-de-valor-e-referencia/#:~:text=Em%20C%23%2C%20quando%20voc%C3%AA%20cria,valor%20e%20tipos%20de%20refer%C3%AAncia</p>

- <p> Por que utilizar C#?: https://balta.io/blog/csharp</p>

- <p>Estrutura de um Programa em C#: https://andrielleazevedo.wordpress.com/2011/12/10/estrutura-de-um-programa-em-c/</p>
