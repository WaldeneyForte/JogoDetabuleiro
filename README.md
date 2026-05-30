# Jogo de Tabuleiro

Um jogo de tabuleiro totalmente desenvolvido em Java com suporte para até 6 jogadores, modos de jogo variados e mecânicas especiais de gameplay.

## 🎮 Características

### Jogadores e Cores
- Suporte para **até 6 jogadores simultâneos**
- Cores disponíveis: RED, BLUE, GREEN, YELLOW, BLACK, WHITE

### Modos de Jogo
- **Modo Normal**: Mecânica tradicional com dois dados (d6)
- **Modo Debug**: Controle manual do movimento dos jogadores para testes e prototipagem

### Casas Especiais

| Casa | Efeito |
|------|--------|
| **TileDontPlay** | O jogador não pode jogar na próxima rodada |
| **TileChange** | Retira 3 cartas; a sorte muda conforme a carta sorteada |
| **TileLucky** | Ativa o modo sortudo, aumentando a soma dos dados do jogador |
| **TileSwitch** | Troca de posição com o jogador mais adiantado |
| **TileJogaDeNovo** | O jogador joga novamente os dados nesta rodada |
| **TileTroca** | O jogador compra um item que pode dar buff ou debuff |


## 🚀 Como Começar

### Compilação

```bash
javac -d bin src/**/*.java
```

### Execução

```bash
java -cp bin Main
```

## 📝 Estrutura do Projeto

```
JogoDetabuleiro/
├── src/
│   ├── game/
│   │   ├── Game.java              (Controlador principal do jogo)
│   │   ├── Main.java              (Ponto de entrada)
│   │   └── TurnController.java    (Gerencia turnos dos jogadores)
│   │
│   ├── board/
│   │   └── Board.java             (Gerencia o tabuleiro e suas casas)
│   │
│   ├── player/
│   │   ├── Player.java            (Classe abstrata - Mãe de todos os tipos de jogador)
│   │   ├── PlayerNormal.java      (Herdeira - Jogador com probabilidade normal)
│   │   ├── PlayerLucky.java       (Herdeira - Jogador com sorte aumentada)
│   │   ├── PlayerUnlucky.java     (Herdeira - Jogador com sorte reduzida)
│   │   ├── NotEnoughCoinException.java
│   │   └── enums/                 (Enumerações do sistema de jogador)
│   │
│   └── tile/
│       ├── Tile.java              (Classe abstrata - Mãe de todas as casas)
│       ├── TileBasic.java         (Herdeira - Casa comum sem efeito especial)
│       ├── TileStart.java         (Herdeira - Casa de início do jogo)
│       ├── TileFinish.java        (Herdeira - Casa de fim do jogo)
│       ├── TileDontPlay.java      (Herdeira - O jogador pula a próxima rodada)
│       ├── TileChange.java        (Herdeira - Muda a sorte do jogador)
│       ├── TileLucky.java         (Herdeira - Ativa modo sortudo)
│       ├── TileUnlucky.java       (Herdeira - Desativa modo sortudo)
│       ├── TileSwitch.java        (Herdeira - Troca posição com jogador adiantado)
│       ├── TileJogaDeNovo.java    (Herdeira - Jogador joga novamente)
│       └── TileTroca.java         (Herdeira - Compra item com buff/debuff)
│
├── bin/                           (Arquivos compilados)
└── README.md
```

### Hierarquia de Classes

#### Jogadores (Player)
```
Player (abstrata)
├── PlayerNormal
├── PlayerLucky
└── PlayerUnlucky
```

#### Casas/Tiles (Tile)
```
Tile (abstrata)
├── TileBasic
├── TileStart
├── TileFinish
├── TileDontPlay
├── TileChange
├── TileLucky
├── TileUnlucky
├── TileSwitch
├── TileJogaDeNovo
└── TileTroca
```

## 🎯 Próximas Melhorias

- [ ] Interface gráfica (GUI)
- [ ] Sistema de persistência de partidas
- [ ] Ranking e estatísticas
- [ ] Testes unitários
- [ ] Documentação JavaDoc

## 📄 Licença

Este projeto é de código aberto.

## ✉️ Contato

Para dúvidas ou sugestões, abra uma issue no repositório.

---

**Desenvolvido com ☕ em Java**
