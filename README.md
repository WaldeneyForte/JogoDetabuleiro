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
| **TileTroca** | Permite trocar posição, escolhendo entre 3 itens disponíveis |

## 🛠️ Tecnologias

- **Linguagem**: Java
- **Paradigma**: Orientado a Objetos

## 📋 Pré-requisitos

- Java JDK 8 ou superior
- Maven ou Gradle (se aplicável)

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
│   └── [código-fonte Java]
├── bin/
│   └── [arquivos compilados]
└── README.md
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
