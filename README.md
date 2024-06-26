# Projeto Buraco

Desenvolvido por:
- Laysa Bernardes Campos da Rocha - CB3024873
- Lucas Lopes Cruz - CB3025284

Disciplina de Estrutura de Dados I

## Objetivo

O objetivo deste programa é criar uma representação em memória para cada uma das 52 cartas de dois baralhos, a fim de serem utilizadas em um jogo de Buraco. O programa irá distribuir aleatoriamente as cartas, dando 11 cartas para cada um dos 4 jogadores participantes, e finalizará apresentando as "mãos" de cada jogador.

### Notação para identificação das cartas

A identificação de cada carta segue a seguinte notação: `N-99-B`, onde:
- `N`: Naipe (1-Copas / 2-Paus / 3-Ouro / 4-Espada)
- `99`: Número da carta (01-Ás / 13-Rei)
- `B`: Baralho (1 ou 2)

Por exemplo, `4-10-2` representa o 10 de Espadas do segundo baralho.

### Exemplo de representação em memória

```cpp
string baralho[2][52];
string mao[4][11];

baralho[0][1] = "1021";
baralho[0][2] = "1031";
baralho[0][0] = "1011";
// ...
baralho[0][12] = "1131";
baralho[0][13] = "2011";
// ...
baralho[0][51] = "4131";
// ...
baralho[1][0] = "1012";
// ...
baralho[1][51] = "4132";

mao[0][0] = "1012";
mao[1][0] = "1011";
// ...

