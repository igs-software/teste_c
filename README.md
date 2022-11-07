# Teste de Linguagem C

## Introdução

O objetivo deste teste é analisar o seu conhecimento em Linguagem C, objetivando a posição de desenvolvedor na IGS Softwares.

## Requisitos

- A solução deste teste deve ser entregue como um repositório no site github.com, com cada uma das questões apresentadas abaixo tendo sua solução correspondendo a um arquivo fonte .c independente;
- Fique à vontade caso queira adicionar comentários ou instruções adicionais em um arquivo README.md na raiz do projeto;
- Todos os nomes de variáveis e métodos devem ser escritos em inglês;
- As boas práticas de codificação, tipagem e nomenclatura em C serão consideradas na avaliação;

## Questão 01

Desenvolver um algoritmo para encontrar o maior palíndromo (trecho que lido da esquerda pra direita e vice-versa mantem a mesma sequência em ambos os lados).

A sequência deve ser lido a partir de um arquivo de texto. Para sua referência, neste repositório você pode encontrar o arquivo *strings_01.txt* , com a sequência que será utilizada na correção deste teste.

O código deve apresentar a quantidade de letras do maior palíndromo dentro de cada string e zero caso não encontre.

## Questão 02

Desenvolver um programa que receba via teclado um número romano, converta o mesmo em número decimal e apresente em tela o resultado. 

Considerar como números validos: I = 1, V = 5 , X = 10, L = 50, C = 100, D = 500, M = 1000

Exemplos de referência de saída : IV = 4 , VI = 6 , XII = 12 , IX =9 , VIII = 8, MDCDLXXIV = 1974.

## Questão 03

Considerando que o espaço de cor RGB pode ser representada por um uint32, onde os 8 primeiros bits menos significantes representam o canal azul,
seguidos por 8 bits que representam a claridade de verde, que por sua vez são seguidos de 8 bits que nos dizem a intensidade do vermelho. Os 8 bits mais significantes são interpretados como o canal Alpha, ou seja, a transparência.

Podemos, portanto, representar cada canal de cor por um par hexadecimal, de 00 a FF. Conseguimos definir então que:

- 0x0 é equivalente a preto, já que a luminosidade de todos os canais está em 0; 
- 0xFF (255) nos daria o azul mais brilhante;
- 0xFF00 (65280) nos daria o máximo de verde possivel;
- 0xFF0000 (16711680) nos daria o vermelho mais vivo;

Crie com base nisto uma função que gradativamente mude e printe a cor vermelha de r_inicial para r_final em um certo numero de passos;

Referência de saída:

```
cor_inicial = 0x00001A; 
cor_final = 0xFF001A; 
steps = 3;
output_esperado: 0x55001A\n 0xAA001A\n 0XFF001A\n
```

## Questão 04

Dada uma array de k , lista lincada “listas”, cada lista esta em ordem ascendente. Mergear as listas lincadas em uma única lista em ordem ascendente.

Input: 

```
listas = [[1,3,8],[1,3,6],[8,9]] 
```

Output: 

```[1,1,3,3,6,8,8,9]```

Referência:

```
listas = [ ] 
output = [ ]
listas = [ [ ] ] 
output = [ ]
struct ListaNode* mergeKListas(struct ListNode** listas, int listasSize){}
```

## Questão 05

Refatorar o código-fonte contido no arquivo *questao_05.c* deste repositório.

Serão considerados fatores como melhoria na eficiência, identação, e simplicidade.

O código deverá fazer um sorteio e a comparação com o “premio”. Se houver match , deverá ser exibida a saída da string “ganhou”.
