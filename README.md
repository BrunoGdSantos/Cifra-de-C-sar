Atualização do Projeto de Criptografia - V2

Nesta segunda versão do projeto, realizamos uma atualização no programa de criptografia desenvolvido em C.

Na V1, o programa utilizava apenas o valor de SHIFT para fazer o deslocamento das letras.

Na V2, adicionamos a sequência de Fibonacci para deixar o deslocamento diferente em cada posição da palavra.

O que foi atualizado

A principal mudança foi a inclusão da sequência de Fibonacci no processo de criptografia.

Na V1, o funcionamento era:

SHIFT

Na V2, passou a ser:

SHIFT + Fibonacci

A sequência utilizada começa com:

1 1 2 3 5 8 13...

Dessa forma, cada letra recebe um deslocamento diferente.

Exemplo da atualização

Considerando:

Palavra: CASA
SHIFT: 3

Na V2, utilizamos:

Fibonacci: 1 1 2 3

Os deslocamentos ficam:

C → 3 + 1 = 4
A → 3 + 1 = 4
S → 3 + 2 = 5
A → 3 + 3 = 6

Resultado:

GEXG
Alteração no código

Foi adicionada a lógica responsável por gerar a sequência de Fibonacci:

int a = 1;
int b = 1;
int proximo;

Também adicionamos o cálculo do próximo número:

proximo = a + b;
a = b;
b = proximo;

E o deslocamento passou a considerar a sequência:

deslocamento = shift + a;
Objetivo da V2

A atualização foi feita para cumprir uma nova etapa da atividade, utilizando um conceito de matemática aplicada à programação.

Com a utilização da Fibonacci, a criptografia deixou de usar somente um deslocamento fixo e passou a utilizar valores diferentes para cada letra.

Autores

Bruno Gabriel dos Santos
Alex Sander de Jesus Carvalho
Isaac Ben Fernandes dos Santos
Guilherme Silva Alves

Projeto desenvolvido para fins acadêmicos.
