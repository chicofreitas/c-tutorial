# Entendenndo o código fonte

## Objetivos de aprendizagem
- Entender a estrutura de um código fonte escrito em C.

Quando vamos iniciar no mundo da programação é quase uma tradição escrever um programa que imprime a frase _"Olá mundo!"_. Não vamos fazer muito diferente aqui.
Nosso primeiro código compilado exibe na tela do terminal a seguinte frase: _"Hello, World!"_ (Olá mundo! na tradução livre do inglês).

Abaixo está o código fonte que compilamos na aula anterior:

    #include<stdio.h>
    
    int main(){
        printf("Hello, World!\n");
        
        return 0;
    }
    
Vamos analisar linha por linha esta estrutura, iniciando com o comando __#include__ encontrado na primeira linha do nosso código.

    #include<stdio.h>
      
Esta instrução diz ao programa que desejamos "incluir" uma biblioteca dentro do nosso código para ser utilizada como parte da nossa lógica de programação.
No include acima, estamos incluindo a biblioteca __stdio.h__, uma abreviação para _Standard Input and Output_ (Entrada e Saída Padrões). A stdio.h é uma das
bibliotecas mais utilizadas em códigos escritos em C, pois ela é esponsável por imprimir mensagens e receber entradas vindas do usuário por meio de algum dispositivo, 
como um teclado por exemplo.

Na terceira linha temos a declaração da __função__ _main_. Entraremos em detalhes sobre declaração de funções nas próximas aulas. Por enquanto, precisamos entender que todo o código que queremos executar deve ficar entre o par de chaves (_{ }_).
     
     int main(){
     }
     
Note que antes do nome da função main temos um __int__ escrito. Este termo indica o tipo de retorno que a função deve nos fornecer ao final de sua execução.

Entre o par de chaves vemos a primeira atuação da biblioteca _stdio.h_. A função __printf()__ é parte da stdio.h e se encarrega de imprimir um __string__(um texto, em poucas palavras). Abaixo, estamos realizando uma __chamada__ à função printf().

    printf("Hello, World!");
    
Por último, temos o valor de retorno. No início da declaração da função main vimos que o tipo de retorno esperado é int (um número inteiro). Observe que o retorno é igual a 0. Isto é, estamos retornando o valor __falso__ em binário (1 significa __verdadeiro__), indicando que não houve erros durante a execução da função main.

    return 0;

Em resumo, esta é a estrutura básica de um código fonte escrito em C. Tente modificar o texto entre aspas duplas "Hello, World!/n" para algo como "Meu primeiro programa em C/n". Em seguida, no terminal, compile novamente:

    $ gcc main.c

e execute com o comando abaixo:

    $ ./a.out
[Introdução]() | Sum | [Variáveis](https://github.com/chicofreitas/c-tutorial/blob/main/variaveis.md)
