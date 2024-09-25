# Jogo da velha ARM64 - Assembly

**O jogo** é uma implementação simples do jogo da velha para arquitetura ARM64, desenvolvida em Assembly pelo usuário **s33ker**.

## Descrição

Este projeto é uma versão em Assembly do clássico jogo da velha, onde dois jogadores alternam entre os símbolos 'X' e 'O' até que um deles consiga alinhar três marcas consecutivas em linha, coluna ou diagonal, ou até que o tabuleiro fique cheio, resultando em empate.

## Instruções para Compilação e Execução

1. **Pré-requisitos**: 
   - Compilador `as` para ARM64.
   - Emulador `qemu-aarch64` para executar em sistemas que não suportam nativamente a arquitetura ARM64.

2. **Compilação**:
   ```bash
   as -o tic_tac_arm64.o tic_tac_arm64.s
   ld -o tic_tac_arm64 tic_tac_arm64.o
   ```

3. **Execução**:
   - Em um sistema ARM64:
     ```bash
     ./tic_tac_arm64
     ```
   - Em sistemas que não suportam ARM64 nativamente:
     ```bash
     qemu-aarch64 ./tic_tac_arm64
     ```

## Controles do Jogo

- O jogo é jogado no terminal. Para fazer uma jogada, insira um número de 1 a 9, que corresponde às posições do tabuleiro conforme abaixo:

```
1 | 2 | 3
---------
4 | 5 | 6
---------
7 | 8 | 9
```

## Sobre o Autor

Este projeto foi desenvolvido por **s33ker**. Se você tiver dúvidas ou sugestões, sinta-se à vontade para contribuir ou entrar em contato.
