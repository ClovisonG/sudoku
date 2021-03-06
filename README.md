# sudoku

### Descrição

Deverá ser implementado em linguagem Python, em modo texto, um jogo SUDOKU estilo
quebra-cabeça, baseado na colocação de números.

“O objetivo do jogo é a colocação de números de 1 a 9 em cada uma das células vazias numa
grade de 9x9, constituída por 3x3 sub grades chamadas regiões. O quebra-cabeça contém
algumas pistas iniciais, que são números inseridos em algumas células, de maneira a permitir
uma indução ou dedução dos números em células que estejam vazias. Cada coluna, linha e
região só pode ter um número de cada um dos 1 a 9.” http://pt.wikipedia.org/wiki/Sudoku

### Requisitos

### Interface com o usuário

```python

SUDOKU-LOKU
Regras:                           +-------+-------+-------+        Comandos:
                                  | 5 3 2 | . 7 . | . . 8 |
Preencha a grade de forma         | 6 . . | 1 9 5 | . . . |            w
que cada coluna, linha e          | . 9 8 | . . . | 6 . . |          a   d        move o cursor
região contenha todos os          +-------+-------+-------+            s
dígitos de 1 a 9.                 | 8 . . | . 6 . | . . 3 |           1-9         entra com um dígito
                                  | 4 5 . | 8 . 3 | . . 1 |            0 .        limpa o dígito
                                  | 7 . . | . 2 . | . . 6 |            n          novo jogo
                                  +-------+-------+-------+            z          salva o jogo
                                  | . 6 . | . . 7 | 2 8 . |            f          fecha o jogo
                                  | 2 . . | 4 1 9 | . . 5 |            x          resolve
                                  | 2 . . | 4 1 9 | . . 5 |            x          resolve
                                  +-------+-------+-------+
```

Ao abrir a aplicação, o jogo salvo deve ser carregado. Caso não exista um jogo salvo, um novo
jogo deve ser gerado (ver item 4).

As opções deverão funcionar da seguinte forma:

### 1. MOVE O CURSOR (w, a, d ou s)
Move o cursor no tabuleiro do jogo. Onde:

w) Para cima
a) Para esquerda
d) Para direita
s) Para baixo

A posição do cursor deve ser indicada por uma cor diferente de background e foreground
(recomendado: cinza claro e preto).

### 2. ENTRA COM UM DÍGITO (1, 2, 3, 4, 5, 6, 7, 8 ou 9)
Altera o valor da célula onde o cursor estiver posicionado, inserindo o caractere digitado. A cor
de background das células preenchidas deve ser preto e a de foreground diferente da utilizada
nas células geradas automaticamente (recomendado: amarelo).

### 3. LIMPA O DÍGITO (0 ou .)
Limpa o valor da célula onde o cursor estiver posicionado, inserindo o caractere '.' ponto como
indicador de célula vazia. A cor de background das células preenchidas deve ser preto e a de
foreground branco.

### 4. NOVO JOGO (n)
Cria um novo jogo, limpando todas as células e preenchendo o tabuleiro com valores gerados
automaticamente em algumas células. Será disponibilizada uma biblioteca com as sub rotinas
necessárias para a geração dos valores aleatórios.

As células com valores gerados automaticamente devem ter uma cor de foreground diferente
das células preenchidas pelo jogador (recomendado: branco);

Deverá ser solicitada a confirmação do usuário.

### 5. SALVA O JOGO (z)
Salva o jogo atual em arquivo para que o usuário possa continuar a jogar em outro momento,
exibindo uma mensagem de confirmação.

### 6. FECHA O JOGO (f)
Fecha o aplicativo, solicitando a confirmação do usuário.

### 7. RESOLVE (x)
Verifica se o jogador resolveu corretamente o jogo atual, exibindo uma mensagem de acordo.
Caso a solução esteja incorreta, o jogo deve continuar. Caso a solução esteja correta, deverá
ser executada a opção de novo jogo (confirmando a ação com o usuário).

#### ATENÇÃO!
Utilize sub rotinas e arquivos separados para modularizar o algoritmo implementado.

##### Avaliação

A avaliação do projeto será realizada na aula anterior à prova da terceira unidade e consistirá
na seguinte etapa:

##### Apresentação (5,0 pontos - Equipe)
A equipe deverá apresentar o programa funcionando. A pontuação será distribuída entre os
requisitos solicitados.
