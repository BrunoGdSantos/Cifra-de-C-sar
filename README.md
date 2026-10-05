Criptografia em C

Esse é um programa simples de criptografia feito em linguagem C.

A ideia é usar o método da Cifra de César, onde cada letra da palavra é deslocada de acordo com o valor de SHIFT escolhido pelo usuário.

Como funciona

Primeiro, o programa pede uma palavra:

Digite uma palavra:

Depois, pede o valor do SHIFT:

Digite o valor do shift:

O SHIFT indica quantas posições cada letra será deslocada.

Por exemplo, se o SHIFT for 3:

A → D
B → E
C → F

Então, se eu digitar:

CASA

com SHIFT 3, o resultado será:

FDVD
Como o código faz isso

O programa utiliza um for para passar por cada letra da palavra:

for (i=0; i < strlen(palavra); i++){
    palavra[i] = palavra[i] + shift;
}

A variável i indica a posição da letra dentro da palavra.

A função strlen() verifica quantas letras a palavra possui.

Depois, cada letra recebe o valor do SHIFT.

Bibliotecas utilizadas

O programa utiliza duas bibliotecas:

#include <stdio.h>
#include <string.h>

A stdio.h permite utilizar comandos como:

printf()
scanf()

A string.h permite utilizar a função:

strlen()

que serve para descobrir o tamanho da palavra.

Exemplo de execução
Digite uma palavra: CASA
Digite o valor do shift: 3
Palavra criptografa : FDVD
Tecnologias utilizadas
Linguagem C
Visual Studio Code
GitHub


Autores

Bruno Gabriel dos Santos
Alex Sander de Jesus Carvalho
Isaac Ben Fernandes dos Santos
Guilherme Silva Alves

Projeto desenvolvido para fins acadêmicos.
