# 🐍 Snake Game — Jogo da Cobrinha

Um jogo clássico da cobrinha desenvolvido com **HTML5, CSS3 e JavaScript puro (Vanilla JavaScript)**. O projeto recria a experiência do Snake em uma interface moderna, responsiva e com tema escuro, sem necessidade de instalar dependências ou configurar servidores.

## 🎮 Sobre o projeto

O objetivo é controlar a cobrinha pelo tabuleiro, coletar alimentos para aumentar a pontuação e crescer, evitando colisões com as paredes e com o próprio corpo. Conforme a pontuação aumenta, o jogo fica progressivamente mais rápido.

O projeto foi construído em um único arquivo `index.html`, reunindo estrutura, estilos e lógica do jogo.

## ✨ Funcionalidades

- 🐍 Movimentação da cobrinha em um tabuleiro de **21 × 21 células**.
- 🍎 Alimentos posicionados aleatoriamente em células livres.
- 🏆 Pontuação de **10 pontos por alimento** e recorde salvo no navegador com `localStorage`.
- ⚡ Aumento gradual da velocidade conforme a pontuação cresce.
- ⏯️ Botões para iniciar, pausar, continuar e reiniciar a partida.
- ⌨️ Controles pelo teclado com **setas direcionais** ou **W, A, S, D**.
- 📱 Controles direcionais na tela para dispositivos com toque ou telas menores.
- 💥 Detecção de colisões com as paredes e com o próprio corpo.
- 🏅 Condição de vitória ao ocupar todas as células do tabuleiro.
- 🎨 Interface responsiva com tema escuro, indicadores de pontuação e mensagens de estado.
- ♿ Identificação acessível de controles, foco visível e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Aplicação |
| --- | --- |
| **HTML5** | Estrutura da página, botões, placar e elemento `canvas`. |
| **CSS3** | Layout responsivo, tema escuro, gradientes e estilos dos controles. |
| **JavaScript (ES6+)** | Lógica do jogo, movimentação, colisões, pontuação e estados da partida. |
| **Canvas 2D API** | Renderização do tabuleiro, da cobrinha e dos alimentos. |
| **Web Storage API (`localStorage`)** | Persistência do recorde no navegador, quando disponível. |

**Sem frameworks, bibliotecas ou dependências externas.**

## 🚀 Como executar

1. Baixe ou clone este repositório.
2. Abra o arquivo `index.html` em um navegador moderno.
3. Clique em **Iniciar** e comece a jogar.

Não é necessário instalar pacotes, executar comandos de build ou iniciar um servidor.

## 🕹️ Controles

| Ação | Controle |
| --- | --- |
| Mover para cima | `↑` ou `W` |
| Mover para baixo | `↓` ou `S` |
| Mover para a esquerda | `←` ou `A` |
| Mover para a direita | `→` ou `D` |
| Pausar / continuar | `Espaço` |
| Iniciar / jogar novamente | `Enter` ou botão na interface |
| Reiniciar | Botão **Reiniciar** |

Em dispositivos móveis, utilize os botões direcionais exibidos abaixo do tabuleiro.

## 📁 Estrutura do projeto

```text
snake-game/
├── index.html   # HTML, CSS e JavaScript do jogo
└── README.md    # Documentação do projeto
```

## ⚙️ Detalhes técnicos

- **Tabuleiro:** 21 × 21 células, desenhado em um `canvas` de 420 × 420 pixels.
- **Velocidade inicial:** intervalo de 150 ms entre atualizações.
- **Progressão:** redução de 4 ms no intervalo a cada 10 pontos, até o mínimo de 65 ms.
- **Estados:** `ready`, `playing`, `paused`, `over` e `won`.
- **Movimentação:** atualização em grade, com bloqueio de inversão imediata de 180°.
- **Geração de alimentos:** seleção aleatória entre as células não ocupadas pela cobrinha.
- **Recorde:** armazenado sob a chave `snakeBest`; o jogo continua funcionando caso o armazenamento esteja indisponível.
- **Troca de aba:** a partida é pausada automaticamente quando a página deixa de estar visível.

## 🎯 Objetivo do desenvolvimento

Praticar conceitos fundamentais de desenvolvimento Front-End, incluindo manipulação do DOM, eventos de teclado e toque, desenho com Canvas, gerenciamento de estados, lógica de colisões, temporização e persistência local de dados.

## 📌 Possíveis melhorias futuras

- 🔊 Efeitos sonoros opcionais.
- 🎚️ Seleção de níveis de dificuldade.
- 🎨 Temas visuais alternativos.
- 📊 Histórico de pontuações.

> **Nota:** as melhorias acima são ideias para futuras versões e não fazem parte da implementação atual.

---

**🐍 Divirta-se e tente superar seu recorde!**
