# 🧪 Testes Automatizados - Webdojo (Cypress)

Este projeto contém testes automatizados end-to-end (E2E) utilizando o Cypress para a aplicação Webdojo.

---

## 📁 Estrutura do Projeto


cypress/
└── support/
├── actions/
├── commands.js
├── e2e.js
└── utils.js


### 📌 Descrição

- **actions/**: Ações reutilizáveis (interações com a UI)
- **commands.js**: Comandos customizados do Cypress
- **e2e.js**: Configuração global dos testes
- **utils.js**: Funções utilitárias

---

## 🚀 Como executar o projeto

A aplicação Webdojo está no mesmo repositório.

### ▶️ Subir aplicação

```bash
npm run dev

A aplicação ficará disponível em:

http://localhost:3000
▶️ Executando os testes
Executar todos os testes (headless)
npm run test
Executar testes com interface
npm run test:ui
Executar testes de login
npm run test:login
Executar login em mobile
npm run test:login:mobile
⚙️ Scripts
"scripts": {
  "dev": "serve -s dist -p 3000",
  "test": "npx cypress run --config viewportWidth=1440,viewportHeight=900",
  "test:ui": "npx cypress open",
  "test:login": "npx cypress run --spec cypress/e2e/login.cy.js --config viewportWidth=1440,viewportHeight=900",
  "test:login:mobile": "npx cypress run --spec cypress/e2e/login.cy.js --config viewportWidth=414,viewportHeight=896"
}
🧩 Padrões adotados
✔️ Organização
Separação por responsabilidades
Reutilização de código
✔️ Estrutura de testes
Uso de actions para abstração
Commands customizados
Utils compartilhadasx