# 💻 Estudos de Electron JS

Repositório dedicado ao aprendizado de **Electron JS**, explorando a criação de aplicativos desktop multiplataforma utilizando tecnologias web (HTML, CSS e JavaScript).

## 🚀 Sobre o Electron

O Electron é um framework que permite o desenvolvimento de aplicações desktop nativas com tecnologias web. Ele combina o motor de renderização do **Chromium** (para o visual) com o ambiente de execução **Node.js** (para acesso ao sistema).

## 📑 Índice

- [💻 Estudos de Electron JS](#-estudos-de-electron-js)
  - [🚀 Sobre o Electron](#-sobre-o-electron)
  - [📑 Índice](#-índice)
  - [🧠 Conceitos Fundamentais](#-conceitos-fundamentais)
  - [📂 Estrutura do Projeto](#-estrutura-do-projeto)

---

## 🧠 Conceitos Fundamentais

Durante os estudos, o foco principal é entender a comunicação entre processos:

- **Main Process:** O coração do app (Node.js). Gerencia o ciclo de vida da aplicação, janelas nativas e eventos do sistema.
- **Renderer Process:** A interface do usuário. Cada janela aberta é um processo de renderização separado.
- **IPC (Inter-Process Communication):** O mecanismo que permite que o `Main` e o `Renderer` conversem de forma segura através do arquivo `preload.js`.

---

## 📂 Estrutura do Projeto

```text
.
├── src/
│   ├── main.js          # Script do Processo Principal
│   ├── preload.js       # Ponte de segurança (Context Isolation)
│   └── renderer/        # Interface (HTML, CSS, JS do front-end)
│       ├── index.html
│       └── style.css
├── package.json         # Dependências e scripts de execução
└── .prettierrc          # Regras de formatação de código
```
