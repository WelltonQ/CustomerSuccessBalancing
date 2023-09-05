<h1 align="center">
   Teste - RD STATION
</h1>
<p align="center">
   <img width="200px" alt="Imagem demonstrativa rd station" src="https://github.com/WelltonQ/CustomerSuccessBalancing/assets/12499627/d85326cc-f28b-4544-980e-e302a2fefd0b" />
</p>
<p align="center">
  <a href="#page_facing_up-descrição">Descrição</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#closed_book-executar">Executar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#man-autor">Autor</a>
</p>

## :page_facing_up: Descrição

# RD Challenge
## Nossas expectativas
A equipe de engenharia da RDStation tem alguns princípios onde baseamos nosso trabalho diário. Um deles é: Projete seu código para ser mais fácil de entender, não mais fácil de escrever. 

Portanto, para nós é mais importante um código de fácil leitura do que um que utilize recursos complexos e/ou desnecessários.

O que gostariamos de ver:

- O código deve ser fácil de ler. [Clean Code](https://medium.com/rd-shipit/clean-code-23580b4e556c) pode te ajudar
- Notas gerais e informações sobre a versão da linguagem e outras informações importantes para executar seu código.
- Código que se preocupa com a performance (Complexidade de Algoritmo)
- O seu código deve cobrir todo os casos de usos presentes no README, mesmo que não haja um teste implementado para tal.
- Você deve enviar para nós `um arquivo zip` contendo o código-fonte da solução e as instruções para rodá-lo ou pode fazer
o upload da solução para repositórios públicos (GitHub, BitBucket, etc) e nos enviar o link de acesso.
- Testes. Você pode adicionar novos testes, mas sem alterar o pacote original

## O Desafio - CustomerSuccess Balancing

Este desafio consiste em um sistema de balanceamento entre clientes e Customer Success (CSs). Os CSs são os Gerentes de Sucesso, são responsáveis pelo acompanhamento estratégico dos clientes.

Dependendo do tamanho do cliente - aqui nos referimos ao tamanho da empresa - nós temos que colocar CSs mais experientes para atendê-los.

Um CS pode atender mais de um cliente, além disso os CSs também podem sair de férias, tirar folga, ou mesmo ficarem doentes, então é preciso levar esses critérios em conta na hora de rodar a distribuição.

Dado este cenário, o sistema distribui os clientes com os CSs de capacidade de atendimento mais próxima (maior) ao tamanho do cliente.

### Exemplo

Se temos 6 clientes com os seguintes níveis: 20, 30, 35, 40, 60, 80 e dois CSs de níveis 50 e 100, o sistema deveria distribui-los da seguinte forma:

- 20, 30, 35, 40 para o CS de nível 50
- 60 e 80 para o CS de nível 100

Sendo `n` o número de CSs, `m` o número de clientes e `t` o número de abstenções de CSs, calcular quais clientes serão atendidos por quais CSs de acordo com as regras apresentadas.


### Premissas

- Todos os CSs têm níveis diferentes
- Não há limite de clientes por CS
- Clientes podem ficar sem serem atendidos
- Clientes podem ter o mesmo tamanho
- 0 < n < 1.000
- 0 < m < 1.000.000
- 0 < id do cs < 1.000
- 0 < id do cliente < 1.000.000
- 0 < nível do cs < 10.000
- 0 < tamanho do cliente < 100.000
- Valor máximo de t = n/2 arredondado para baixo

## Input

A função `customerSuccessBalancing()` recebe 3 parâmetros:

- id e nivel da experiencia do CS
- id e nivel de experiência dos Clientes
- ids dos CustomerSuccess indisponíveis


## Output

O resultado esperado deve ser o id do CS que atende mais clientes. Com esse valor a empresa poderá fazer um plano de ação para contratar mais CS's de um nível aproximado.

Em caso de empate retornar `0`.

### Exemplo

No input de exemplo, CS's 2 e 4 estão de folga, sendo assim o CS 1 vai atender os clientes de tamanho até 60 (clientes 2, 4, 5, 6), enquanto o CS 3 vai atender os clientes 1 e 3.

Para este exemplo o retorno deve ser `1`, que é o id do CS que atende 4 clientes:

```
1
```
## Choose your weapon:
Nós vamos aceitar o teste em qualquer uma das linguagens abaixo.
### Testes já implementados
- [Ruby](ruby/README.md) 
- [JavaScript](javascript/README.md)
- [Java](java/README.md)
- [Go](go/README.md)


## 🛠 Tecnologias

Este projeto foi desenvolvido com a seguinte tecnologia

- [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)

## :closed_book: Executar

### Clone este repositório.

```bash
## JavaScript

# Entre na pasta
$ cd javascript

# Instale as dependências
$ yarn

# Execute aplicação
$ yarn test

```

## :man: Autor

✔ By [Wellton Quirino](https://www.linkedin.com/in/welltonquirino/)
