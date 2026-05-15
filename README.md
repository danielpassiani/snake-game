<div align="center">
  <h1>🐍 Jogo da Cobrinha (Snake Game)</h1>
  <p>
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" alt="HTML5" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white" alt="CSS3" />
    <img src="https://img.shields.io/badge/JavaScript-323330?style=flat&logo=javascript&logoColor=F7DF1E" alt="JavaScript" />
  </p>
  <p><i>Uma versão nostálgica do clássico Jogo da Cobrinha, com foco na lógica de programação e renderização gráfica.</i></p>
</div>

---

## 📖 Sobre o Projeto

Este projeto é uma recriação simples e funcional do clássico "Snake Game", desenvolvida utilizando apenas tecnologias web nativas (Vanilla JS). É uma excelente aplicação prática para exercitar lógica bidimensional, sistema de coordenadas e gerenciamento de eventos (inputs do usuário).

## ✨ Recursos Implementados

- 🎨 **Área de Jogo:** Renderização dinâmica utilizando a API gráfica do `<canvas>` (400x400).
- ⌨️ **Controles de Precisão:** Movimentação fluida com as setas do teclado, incluindo uma trava de segurança para impedir a reversão instantânea (evitando o "game over" acidental ao inverter a direção).
- ⚙️ **Mecânicas Clássicas:**
  - Sistema de pontuação (+10 pontos por comida).
  - Crescimento automático da cobrinha a cada pontuação.
  - Rigorosa detecção de colisões (com as paredes limitadoras e com o próprio corpo).
  - Reinício automático da partida.
- 🕹️ **Recursos Extras:** Controles de velocidade, sistema de Pausar/Continuar e efeitos sonoros básicos para maior imersão.

## 🚀 Como Rodar Localmente

Como o projeto foi construído puramente no front-end, sem necessidade de build ou dependências complexas, executá-lo é super rápido:

1. Faça o download ou clone este repositório.
2. Abra o arquivo `index.html` diretamente no seu navegador preferido (dando um duplo clique).
3. **Ou**, se preferir usar o terminal (ex: PowerShell), navegue até a pasta do projeto e execute:

```powershell
start index.html
