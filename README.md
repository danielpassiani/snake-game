<div align="center">
  <h1>🐍 Jogo da Cobrinha (Snake Game)</h1>
  <p>
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" alt="HTML5" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white" alt="CSS3" />
    <img src="https://img.shields.io/badge/JavaScript-323330?style=flat&logo=javascript&logoColor=F7DF1E" alt="JavaScript" />
  </p>
  <p><i>Uma versão nostálgica do clássico Jogo da Cobrinha, desenvolvida com foco em manipulação de DOM, Canvas API e lógica bidimensional.</i></p>
</div>

---

## 📖 Sobre o Projeto

Este projeto é uma recriação completa do clássico "Snake Game" utilizando puramente **Vanilla JavaScript**, HTML e CSS. O objetivo principal desta aplicação é demonstrar a aplicação prática de fundamentos essenciais da programação web, como estruturas de dados, loops de renderização e consumo de APIs nativas do navegador, sem a dependência de bibliotecas ou frameworks externos.

## 🧠 Lógica e Arquitetura do Código

O código foi estruturado de forma procedural, focando na clareza do fluxo de execução. Alguns destaques técnicos da implementação incluem:

* **Estruturas de Dados:** A cobrinha é gerenciada como um *Array* de coordenadas `{x, y}` na malha do jogo. O movimento é simulado de forma eficiente inserindo uma nova "cabeça" no início da matriz (`unshift()`) e removendo a "cauda" no final (`pop()`), a menos que a cobra tenha se alimentado.
* **Motor Gráfico (Canvas API):** Toda a renderização visual é feita desenhando formas geométricas (`fillRect`) diretamente no contexto 2D do `<canvas>`.
* **Gerenciamento de Estado (Game Loop):** O jogo roda através de um ciclo contínuo gerido por `setInterval`, onde a cada "tick" (milissegundos) o estado lógico do jogo é calculado (`update()`) e imediatamente redesenhado na tela (`draw()`).
* **Áudio Sintetizado (Web Audio API):** Em vez de utilizar arquivos `.mp3` externos pesados, os efeitos sonoros (captura da maçã e o *Game Over*) são gerados matematicamente no próprio navegador usando osciladores (`AudioContext`), economizando banda e demonstrando domínio sobre APIs multimídia.
* **Tratamento de Eventos Rigoroso:** Captura de *inputs* do teclado com `e.preventDefault()` (para evitar que a página inteira role junto com as setas) e implementação de validação lógica para impedir que o jogador faça uma reversão instantânea de 180 graus (causando um *game over* acidental).

## ✨ Funcionalidades Adicionais

* **Controle de Dificuldade:** Seletor de velocidade dinâmico (Lento, Normal, Rápido) que ajusta o tempo de resposta do *Game Loop* em tempo real.
* **Sistema de Pausa:** Interrupção segura do intervalo do jogo com a capacidade de retomá-lo exatamente do mesmo quadro.
* **Feedback Visual:** Placar atualizado dinamicamente e sombreamento interno (*box-shadow*) no CSS para simular a profundidade de um monitor retrô.

## 🚀 Como Rodar Localmente

Por ser um projeto *Front-End* puro construído em um único arquivo de execução, não há necessidade de instalação de dependências ou servidores complexos.

1. Faça o clone do repositório ou o download do arquivo `index.html`.
2. Dê um duplo clique no arquivo para abri-lo diretamente no seu navegador.
3. **Ou**, se preferir usar a linha de comando (ex: PowerShell), digite:

```powershell
start index.html
