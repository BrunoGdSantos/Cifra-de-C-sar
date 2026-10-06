Criptografia Matemática em C

Descrição

Este projeto foi desenvolvido em linguagem C para a disciplina de Algoritmo e Pensamento Computacional. O sistema combina conceitos de criptografia e sequências matemáticas para realizar a codificação de palavras.

O programa utiliza o método de deslocamento baseado em SHIFT, combinado com uma sequência matemática escolhida pelo usuário. O objetivo é aplicar conceitos de programação, raciocínio lógico e matemática em uma aplicação prática.

Funcionalidades

Criptografia de palavras com até 15 letras.

Validação da entrada, permitindo somente letras sem acentos.

Definição de um valor de SHIFT pelo usuário.

Seleção da sequência matemática utilizada na criptografia.

Implementação das seguintes sequências:

Progressão Aritmética (PA);

Progressão Geométrica (PG);

Fibonacci;

Números Primos.

Exibição dos valores da sequência utilizados durante a execução.

Geração do arquivo resultado_criptografia.txt.

Registro das execuções no arquivo log_criptografia.txt.

Menu interativo para utilização do sistema.

Funcionamento

Para cada caractere da palavra, o programa calcula o deslocamento utilizando o valor do SHIFT e o valor correspondente da sequência escolhida.

Deslocamento = SHIFT + valor da sequência

A partir desse valor, cada letra é deslocada dentro do alfabeto, gerando a palavra codificada.

Sequências disponíveis

Progressão Aritmética (PA)

1, 3, 5, 7, 9, ...

Progressão Geométrica (PG)

1, 2, 4, 8, 16, ...

Fibonacci

1, 1, 2, 3, 5, 8, 13, ...

Números Primos

2, 3, 5, 7, 11, 13, ...

Arquivos gerados

resultado_criptografia.txt

Armazena as informações referentes à execução da criptografia, incluindo:

Palavra original;

Palavra codificada;

Valor do SHIFT;

Tipo de sequência utilizada;

Quantidade de letras.

log_criptografia.txt

Registra as execuções realizadas pelo programa, permitindo manter um histórico das criptografias realizadas.

Tecnologias

Linguagem C

Biblioteca stdio.h

Biblioteca string.h

Biblioteca ctype.h

Manipulação de arquivos

Funções

Estruturas condicionais

Estruturas de repetição

Objetivo

O projeto tem como objetivo desenvolver e aplicar conhecimentos de algoritmos, programação estruturada, criptografia básica e sequências matemáticas, relacionando conceitos teóricos com uma implementação prática em linguagem C.

Autores

João Victor Martines
Bruno Gabriel dos Santos
Alex Sander de Jesus Carvalho
Isaac Ben Fernandes dos Santos
Guilherme Silva Alves

Projeto desenvolvido para fins academicos.
