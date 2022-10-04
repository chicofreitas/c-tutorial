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


     
     int main(){
     }
     
some text...

    printf("Hello, World!");
    
as

    return 0;
