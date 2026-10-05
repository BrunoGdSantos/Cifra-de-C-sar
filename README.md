Projeto de Criptografia em C

Este projeto foi feito para uma atividade da disciplina de Algoritmo e Pensamento Computacional.

A ideia do projeto é criar um programa simples de criptografia usando a linguagem C. Para isso, utilizei a Cifra de César junto com a sequência de Fibonacci.

Como funciona

O programa pede para o usuário digitar uma palavra e escolher um valor para o SHIFT.

O SHIFT é usado para deslocar as letras da palavra. Além disso, o programa utiliza a sequência de Fibonacci para aumentar ou diminuir o deslocamento de cada letra.

A conta utilizada pelo programa é:

Deslocamento = SHIFT + número da sequência de Fibonacci

A sequência de Fibonacci utilizada começa assim:

1 1 2 3 5 8 13...
Exemplo

Se eu digitar:

Palavra: CASA
SHIFT: 3

O programa vai utilizar:

1 1 2 3

Então o deslocamento de cada letra será:

C → 3 + 1 = 4
A → 3 + 1 = 4
S → 3 + 2 = 5
A → 3 + 3 = 6

Com isso, a palavra é transformada e aparece na tela como resultado da criptografia.

O que eu utilizei

Para fazer o projeto, utilizei:

Linguagem C
Visual Studio Code
GitHub

Também utilizei as bibliotecas:

#include <stdio.h>
#include <string.h>

A biblioteca stdio.h é utilizada para receber e mostrar informações na tela, através de scanf() e printf().

A biblioteca string.h foi utilizada para saber o tamanho da palavra através da função strlen().

Como o programa funciona no código

Primeiro, o programa cria uma variável para guardar a palavra:

char palavra[20];

Depois são criadas as variáveis para o SHIFT e para controlar o for:

int shift;
int i;

Também são criadas as variáveis utilizadas para gerar a sequência de Fibonacci:

int a = 1;
int b = 1;
int proximo;

O programa então pede a palavra e o SHIFT:

printf("Digite uma palavra: ");
scanf("%s", palavra);

printf("Digite o SHIFT: ");
scanf("%d", &shift);

Depois, o for passa por cada letra da palavra e aplica o deslocamento:

deslocamento = shift + a;

palavra[i] = palavra[i] + deslocamento;

Ao mesmo tempo, o programa calcula o próximo número da sequência de Fibonacci.

No final, a palavra criptografada é mostrada na tela.

Exemplo de execução
Digite uma palavra: CASA
Digite o SHIFT: 3
Palavra criptografada: GEXG
Autor

Bruno Gabriel dos Santos
Alex Sander de Jesus Carvalho
Isaac Ben Fernandes dos Santos
Guilherme Silva Alves

Projeto desenvolvido para fins acadêmicos.
