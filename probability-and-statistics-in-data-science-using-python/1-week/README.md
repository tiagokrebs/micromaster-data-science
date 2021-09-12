## Probabilidade
- Probabilidade é o framework de teoria matemática para a computação de probabilidade de eventos complexos
- Assume-se que a probabilidade de eventos simples é conhecida

### Flip coin 

Jogando uma moeda os resultados são cara ou coroa ou a probabilidade dos eventos simples são iguais. 
Isso não significa, porém, que ao jogarmos uma moeda 10k vezes os resultados serão iguais tanto para cara quanto para coroa.

Podemos afirmar matematicamente que ao jogar uma modeda 10k vezes o resutado será aproximadamente 5k.
k = 10.000
10.000/2 = 5.000

Go to the notebook - Part 1

--

- Teoria da propabilidade é a matemática envolvida em prover uma versão precisa de afirmações como as do caso flip a coim
- Na maioria dos casos podemos encontrar probabilidades aproximadas utilizando simulações Monte-Carlo como no runbook
- Aproximações, porém, não são suficientes
     - Não proporcionam uma resposta exata e precisam ser repetidas inúmeras vezes até atingir respostas mais precisas
     - Teoria da probailidade sempre será mais rápida do que essas aproximações


## Estatística
- Oposto da definição de Probabilidade
- Dado um conjunto de dados gerado por algum método estocástico propriedades são inferidas sobre probabilidades base

### Flip coin

Jogando uma moeda 1000 vezes e obtendo o resutado "cara" 750 vezes, podemos concluir que a moeda tem tendência a esse resultado? 
Se o resultado for 570 "cara"? Mais próximo dos 50% porém ainda com valores de "cara" maior]
Como decidimos se a moeda é tendenciosa ou não?

Inferência
- Supõem-se que a moeda é justa
- Calculamos qual é a probabilidade das jogadas resultarem em 570 "cara"
- Se essa probabulidade for muito pequena podemos rejeitar **com confiança** a hipótese de que a moeda é justa

Go to the Notebook - Part 2

--

Estatística é sobre analisar dados reais e criar conclusões
- pesquisas
- testes A/B
- decisão sobre eficácia de um método ou produto


## 3-Card Puzzle
Temos 3 cartas com as combinações de cores azul e vemelho em ambos os lados:
- Carta 1: vermellho / azul
- Carta 2: azul / azul
- Carta 3: vermelho / vermelho
A cada jogada uma carta é retirada de um saco e colocada na mesa.
Caso o lado contrário da carta seja igual um jogador ganha um ponto.
Caso o outro lado seja diferente o outro jogador ganha um ponto.
Premissa: é um jogo justo, já que as chances entre vermelho e azul são iguais (50%)

Tesste de Monte-Carlo...
Go to notebook

--

Argumento alternativo: ao escolher uma carta existem 2/3 de chance dela possuir a mesma cor no lado contrário e 1/3 uma cor diferente.
- O arguemento anterior originl é convincente mas está errado
- Como temos certeza de que está incorrero? Através de simulação
- Muitas vezes simulações não são práticas o suficiente, podem demorar muito tempo e vão reproduzir apenas um resultado aproximado, como validar então?
    - Precisamos introduzir conceitos de resultados e eventos (next class)
    - Precisamos de mais formalismo


