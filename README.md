# Sudoku - Desafio DIO

Implementação de um jogo de Sudoku em Java desenvolvida durante os desafios da Digital Innovation One (DIO).

## Sobre o projeto

Este projeto consiste em uma aplicação de linha de comando (CLI) que permite jogar Sudoku diretamente pelo terminal.

O jogo oferece funcionalidades para iniciar uma partida, inserir números, remover valores, verificar o status atual do tabuleiro, limpar o progresso e validar a conclusão do jogo.

O objetivo do desafio é aplicar conceitos fundamentais da linguagem Java, incluindo:

* Programação Orientada a Objetos (POO)
* Estruturas de dados
* Collections Framework
* Streams API
* Enumerações
* Organização em camadas e pacotes
* Manipulação de entrada e saída via terminal

## Funcionalidades

* Iniciar uma nova partida
* Inserir números em posições livres
* Remover números inseridos pelo jogador
* Visualizar o estado atual do tabuleiro
* Verificar o status da partida
* Detectar erros de preenchimento
* Reiniciar o jogo
* Validar a conclusão do Sudoku

## Estrutura do projeto

```text
src/
├── br/
│   └── com/
│       └── dio/
│           ├── Main.java
│           ├── model/
│           │   ├── Board.java
│           │   ├── GameStatusEnum.java
│           │   └── Space.java
│           └── util/
│               └── BoardTemplate.java
```

## Tecnologias utilizadas

* Java 21
* IntelliJ IDEA
* Git
* GitHub

## Conceitos aplicados

### Board

Responsável por representar o tabuleiro do Sudoku e controlar:

* Estado do jogo
* Alteração de valores
* Limpeza de posições
* Validação da conclusão da partida

### Space

Representa uma célula do tabuleiro.

Cada posição possui:

* Valor esperado
* Valor atual
* Informação se o valor é fixo ou editável

### GameStatusEnum

Define os possíveis estados da partida:

* NON_STARTED
* INCOMPLETE
* COMPLETE

## Como executar

Compile os arquivos Java:

```bash
javac -d out $(find src -name "*.java")
```

Execute a aplicação:

```bash
java -cp out br.com.dio.Main
```

## Menu do jogo

Ao iniciar a aplicação, o seguinte menu será exibido:

```text
1 - Iniciar um novo jogo
2 - Colocar um novo número
3 - Remover um número
4 - Visualizar jogo atual
5 - Verificar status do jogo
6 - Limpar jogo
7 - Finalizar jogo
8 - Sair
```

## Melhorias futuras

* Interface gráfica (JavaFX ou Swing)
* Geração automática de tabuleiros
* Diferentes níveis de dificuldade
* Sistema de dicas
* Persistência de partidas
* Testes automatizados com JUnit

## Projeto original

Este projeto foi desenvolvido a partir de um desafio proposto pela Digital Innovation One (DIO) para prática de Programação Orientada a Objetos em Java.

## Licença

Este projeto é destinado a fins educacionais e de aprendizado.
