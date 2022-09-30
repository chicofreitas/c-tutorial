# Introdução

## O que vamos aprender
- Saber como um computador executa seus programas;
- Compreender os conceitos de linguagem de máquina e seus níveis de abstração;
- Aprender como compilar um código fonte escrito na liguagem C; 

### Sobre Programas e Computadores

O computador é uma máquina eletrônica capaz de realizar uma grande variedade de tarefas com alta velocidade e precisão, desde que receba as __instruções__ adequadas. Estas instruções são como uma receita, em que os passos para a realização de uma tarefa é escrita em uma linguagem apropriada, a __linguagem de máquina__. As instruções adequadas constituem os programas que dirigem o funcionamento do computador e estão escritas em __código binário__.

Isso mesmo! Quando utilizo o termo binário, estou me referindo aos dígitos zero (0) e um (1). A forma mais próxima, e também muito complexa, de se criar um programa para realizar tarefas no computador é por meio da linguagem __Assembly__. Assim tarefas são realizadas através da execução de operações lógicas /aritméticas e tomada de decisões.

A linguagem Assembly é classificada como de __baixo nível__ por causa de sua pouca abstração em relação às intruções escritas. Enquanto que linguagens de médio e ato níveis possuem um grau de abstração maior, utilizando simbolos que são mais amigáveis ao ser humano (como as palavras do nosso idioma nativo). Porém, após a criação de um código, que chamaremos aqui de __código fonte__, geralmente precisamos traduzir nossas linhas para a linguagem de máquina, afim que ela retorne os resultados esperado. Isto é realizado através de outros programas chamados __compiladores__. Para facilitar o entendimento, você pode visualizar um compilador como um tradutor que traduz os símbolos familiares para o ser humano em códigos binários compreensíveis apenas pelo computador.

Desta forma o computador forma o que chamamos de __sistema de computação__, onde temos a parte física (ou hardware) e a parte lógica (o software). Um sistema de computação também realiza as três funções básicas: entrada, processamento e saída. A entrada de um sistema de computação corresponde ao conjunto dos dados necessários para a realização de uma tarefa. O processamento refere-se às modificações realizadas sobre os dados de entrada e à elaboração dos resultados. A saída corresponde ao conjunto de dados resultantes obtidos.

O software é classificado em dois tipos: 
- o software aplicativo:
  - os quais executam uma tarefa específica, uma aplicação. Exemplos são: editores de texto, planilhas eletrõnicas, editores de imagem, etc.
- e o software básico:
  - este realizam funções essenciais no próprio hardware. 

Durante nosso curso vamos desenvolver (criar) nossos próprios códigos fonte e gerar um arquivo executável, um programa, com a ajuda de um compilador apropriado para a linguagem C.

Pra aprofundar um pouco mais, veja o vídeo [Compiladores - O Programa Essencial de Todos os Programadores](https://www.youtube.com/watch?v=afUiVvDUIRA), disponibilizado pelo canal no YouTube [Código Fonte TV](https://www.youtube.com/c/codigofontetv)

### A Linguagem _C_

A linguagem de programação C foi desenvolvida por um cientista da computação americano Dennis M. Ritchie nos Laboratórios Bell (anteriormente AT&T Bell Laboratories) em 1972, para desenvolver o sistema operacional Unix. C é uma linguagem de nível médio porque contém os recursos da linguagem de baixo nível, bem como da linguagem de alto nível. A linguagem de programação C é uma linguagem de programação de computador __procedural__ de __propósito geral__ que suporta __programação estruturada__.

A linguagem de programação C é uma sucessora da linguagem de programação B. Uma versão anterior do padrão de linguagem de programação C era chamado C99, um nome informal para ISO/IEC 9899:1999. C faz parte da criação de outros sistemas operacionais, linguagens de programação e muitas aplicações utilizadas comercialmente.

Assiste ao vídeo [C - A Linguagem de Programação que é uma Mãe](https://www.youtube.com/watch?v=6mUCcsnCn08), disponibilizado pelo canal no YouTube [Código Fonte TV](https://www.youtube.com/c/codigofontetv) para saber um pouco mais sobre a linguagem C.

#### Atividade prática sobre: a linguagem C

[Atividade](https://google.com.br)


### Instalando o Compilador C

Não vamos detalhar aqui a instalação dos compiladores, mas segue abaixo alguns links de tutoriais que podem ajudar nesta tarefa:
- [Instalando o GCC no Linux](https://pt.linuxcapable.com/install-gcc-compiler-build-essential-on-ubuntu-20-04-lts/);
- [Instalando o GCC no Windows](https://terminaldeinformacao.com/2015/10/08/como-instalar-e-configurar-o-gcc-no-windows-mingw/);

### Compilando Nosso Primeiro Código Fonte

Neste seção vamos executar nosso primeiro programa. O código fonte abaixo é um exemplo de código escrito utilizando a linguagem C. Os detalhes sobre a estrutura do código serão discutidas em breve. Por isso, não fique assustado com as linhas a princípio sem sentido. Vamos focar nossa atenção no processo de compilação.

    #include <stdio.h>
    
    int main()
    {
          printf("Hello, World!\n");
          return 0;
    }

O download do código fonte acima pode ser realizado [aqui](https://github.com/chicofreitas/c-tutorial/blob/main/src/main.c). Sugiro que salve o código em uma pasta com o nome do seu projeto, por exemplo:

_C:/Documentos/meu_projeto/main.c_ caso esteja utilizando Windows, 

ou _/home/usuario/Code/meu_projeto/main.c_ no caso de estar operando no Linux.

Note que o arquivo está nomeado como __main.c__. Todos os arquivos que utilizaremos para programar em C devem conter a extensão __\*.c__. Por exemplo: *calculadora.c*, *imprimir.c*, *open_files.c*,...

Tendo o arquivo *main.c* em mãos, agora vamos realizar a sua compilação utilizando o compilador __GCC__. Abra o terminal e navegue até o diretório em que o arquivo foi salvo. Em seguida, execute o comando abaixo:

    $ gcc main.c -o main
    
Se tudo ocorrer bem, um arquivo executável *main* será gerado no mesmo diretório do arquivo *main.c*. Vocẽ pode conferir executando o comando

    $ ls
    main    main.c

para listar todos os arquivos no diretório. Observe que o novo arquivo não possui uma extensão, como *.c* ou *.bin*.

Agora, chegou a hora de testar nosso primeiro primeiro programa. Execute o arquivo *main* da seguinte forma:

    $ ./main
  
Após executar o comando acima, uma frase com o texto "Hello, World!" deve aparecer na linha seguinte.

    $ Hello, World!\n
    
## Em resumo

- Um computador executa as tarefas escritas em uma linguagem binária ou Assembly;
- Um programador precisa escrever um código fonte em alguma linguagem, para em seguida ser compilado em código de máquina para ser utilizado pelo computador;
- Ao utilizar o comand __gcc main.c -o main__ um novo arquivo (__main__) executável é gerado e pode ser executado através do comando __./main__.
- 
## O que vem em seguida:

Agora que aprendemos um pouco sobre como criar programas executáveis, nosso próximo passo é aprender como armazenar alguns tipos de dados e utilizá-los de alguma forma em um momento seguinte.

[Variáveis > ](https://github.com/chicofreitas/c-tutorial/blob/main/variaveis.md)
