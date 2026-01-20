# 🧪 Testes Manuais – DemoBlaze

Este repositório contém a execução de **testes manuais** realizados no site **DemoBlaze**, uma aplicação web de e-commerce utilizada amplamente para fins educacionais e prática de Quality Assurance.

O projeto tem como objetivo **aplicar conceitos de QA Manual**, validar o fluxo principal do usuário, identificar bugs e documentar resultados de forma organizada para **portfólio profissional**.

---

## 🌐 Site Testado
- **URL:** https://www.demoblaze.com/
- **Projeto:** DemoBlaze – Online Store

---

## 🎯 Objetivo dos Testes
- Validar o funcionamento das principais funcionalidades do sistema
- Identificar falhas funcionais e de usabilidade
- Avaliar o processo de compra (end-to-end)
- Documentar bugs e pontos de melhoria

---

## 📌 Escopo dos Testes
- Login
- Logout
- Navegação entre categorias
- Visualização de produtos
- Adição de itens ao carrinho
- Processo de Checkout
- Usabilidade
- Performance percebida

---

## 📊 Resultado Geral dos Testes

| Área | Resultado |
|-----|----------|
| ✅ Login | Funcionando conforme esperado |
| 🚪 Logout | Funcionando corretamente |
| 🛒 Carrinho | Adição de produtos sem falhas |
| 💳 Checkout | Bug crítico encontrado |
| 👁️‍🗨️ Usabilidade | Boa, porém com pontos de melhoria |
| ⚡ Performance | Funciona, mas apresenta lentidão em alguns momentos |

---

## 📝 Pontos Observados Durante os Testes

### 🔐 Login e Logout
- Login e logout funcionam corretamente.
- O sistema bloqueia tentativas de envio com campos vazios, impedindo ações inválidas.

---

### 🛒 Carrinho
- Os itens são adicionados ao carrinho normalmente.
- Não foram observados atrasos ou falhas durante a inclusão dos produtos.

---

### 💳 Checkout
🚨 **Bug Crítico Identificado**

Durante o processo de checkout, o sistema permite finalizar a compra preenchendo apenas:
- Nome
- Número do cartão de crédito

Os demais campos permanecem vazios, sem qualquer validação ou mensagem de erro.

📌 **Classificação do Bug**
- Severidade: **Alta**
- Prioridade: **Alta**

---

### ⚡ Performance
- O sistema funciona conforme esperado, porém apresenta **leve lentidão na fluidez**, principalmente durante a navegação entre páginas.

---

## 🐞 Bugs Identificados
- Falta de validação nos campos obrigatórios do checkout
- Possibilidade de finalizar compra com dados incompletos
- Lentidão perceptível em algumas interações

---

## 📄 Documentação de Testes

Para apoiar a execução dos testes, foi utilizada uma **planilha de controle**, contendo:
- ID do caso de teste
- Descrição
- Passos executados
- Resultado esperado
- Resultado obtido
- Status (Passou / Falhou)
- Observações e bugs relacionados

📎 A planilha pode ser disponibilizada como anexo ou link no repositório.

---

## ✅ Conclusão Final

O DemoBlaze apresenta um fluxo funcional básico de e-commerce, porém possui **falhas críticas no processo de checkout**, que podem comprometer a integridade das compras e dos dados inseridos.

Recomenda-se:
- Implementação de validações obrigatórias nos campos
- Melhoria na fluidez e performance geral
- Reteste e teste de regressão após correções

---

## 👨‍💻 Autor
**Gabriel Miranda**  
QA Manual | Quality Assurance em formação  

📌 Projeto desenvolvido para fins de estudo, prática e portfólio profissional.
