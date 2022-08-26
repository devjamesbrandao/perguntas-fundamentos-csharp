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
> Em C#, a utilização da palavra-chave <strong>using</strong> tem dois objetivos: a primeira é a diretiva de utilização, que é utilizada para importar namespaces no topo de um arquivo de código. A segunda é a declaração de utilização. No C# 8, utilizar declarações <strong>using</strong> asseguram que as classes que implementam a interface IDisposable chamem o seu método de Dispose .

26. Qual a diferença entre uma variável e uma constante?
> Uma <strong>variável</strong> é como um recipiente que contém os valores ou dados de um determinado tipo de dados que ajudam a executar o programa. O valor de uma variável <strong>pode mudar</strong> dependendo das condições ou informações dadas no tempo de execução do programa. Já a <strong>constante</strong> é um valor fixo cujo valor <strong>não pode ser alterado</strong> durante a execução do programa ou uma vez que o valor é definido.

### ` 🌐 Referências`
- <p> Perguntas para entrevista de C# e .NET: https://balta.io/blog/perguntas-entrevista-csharp</p>

- <p> Por que utilizar C#?: https://balta.io/blog/csharp</p>

- <p>Estrutura de um Programa em C#: https://andrielleazevedo.wordpress.com/2011/12/10/estrutura-de-um-programa-em-c/</p>
