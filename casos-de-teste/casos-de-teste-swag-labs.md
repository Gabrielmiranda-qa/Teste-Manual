# 🧪 Testes Manuais – Swag Labs (Sauce Demo)

Este repositório contém a execução de **testes manuais** realizados no site **Swag Labs (Sauce Demo)**, com foco no fluxo principal do usuário, usabilidade, responsividade e acessibilidade.

O objetivo deste projeto é **praticar conceitos de QA Manual**, documentar casos de teste, identificar bugs e apresentar tudo de forma clara e organizada para fins de **portfólio profissional**.

---

## 🌐 Site Testado
- **URL:** https://www.saucedemo.com/
- **Projeto:** Swag Labs (Sauce Demo)

---

## 👤 Perfis de Usuário Utilizados
- `standard_user` – Usuário padrão
- `locked_out_user` – Usuário bloqueado
- `problem_user` – Usuário com comportamentos inesperados

---

## 🎯 Escopo dos Testes
- Login e Logout
- Navegação no sistema
- Adição de produtos ao carrinho
- Processo de Checkout
- Usabilidade
- Responsividade
- Acessibilidade básica (Lighthouse)

---

## 📊 Resultado Geral dos Testes

| Área | Resultado |
|-----|----------|
| ✅ Login (standard_user) | Funcionando normalmente |
| 🔐 Usuário bloqueado (locked_out_user) | Bloqueio correto |
| 🧪 Usuário problemático (problem_user) | Login ok, imagens com falha |
| 🛒 Processo de compra | Funciona, mas carrinho não é limpo após a compra |
| 👁️‍🗨️ Usabilidade | Navegação simples e intuitiva |
| 📱 Responsividade | Boa no geral, com falhas em alguns tamanhos de tela |

---

## 📝 Principais Pontos Observados

### 🔐 Login
- Login funcional para usuários válidos.
- Usuário bloqueado impedido corretamente.
- **Sugestão de melhoria:**  
  O ícone de exibir senha desaparece ao retirar o mouse. O ideal seria mantê-lo visível até que o usuário decida ocultar a senha manualmente.

---

### 🛒 Checkout
- O fluxo de compra pode ser concluído.
- **Bug encontrado:**  
  Após finalizar a compra, o produto permanece no carrinho, podendo gerar confusão para o usuário.

---

### 📷 Imagens (problem_user)
- Algumas imagens de produtos não carregam corretamente ao utilizar o usuário `problem_user`.

---

### 📱 Responsividade
- Em resoluções intermediárias, o layout apresenta:
  - Elementos desalinhados
  - Colunas comprimidas

**Sugestão:** ajustes com media queries adicionais.

---

### ♿ Acessibilidade
- **Pontuação Lighthouse:** 57
- Necessita melhorias em:
  - Contraste
  - Semântica
  - Navegação por teclado

---

## 🐞 Bugs Identificados
- Carrinho não é limpo após a finalização da compra
- Falha no carregamento de imagens para usuários específicos
- Pequeno problema de usabilidade no campo de senha
- Falhas de responsividade em alguns tamanhos de tela

---

## 📄 Documentação de Testes

Durante a execução dos testes, foi utilizada uma **planilha de controle**, contendo:
- ID do caso de teste
- Descrição
- Passos executados
- Resultado esperado
- Resultado obtido
- Status (Passou / Falhou)
- Observações e bugs

📎 **Planilha utilizada:**  
🔗 https://1drv.ms/x/c/c24af324cc94e3d9/IQBDSNZJjNvaT65zVH9JZjNjAf-IpWlVmROvBUjN_OsLRZM

---

## ✅ Conclusão Final
O Swag Labs apresenta um fluxo principal funcional e fácil de usar.  
Apesar disso, alguns problemas impactam a experiência do usuário e devem ser tratados com prioridade.

Após a correção dos pontos levantados, recomenda-se a realização de:
- Reteste
- Teste de regressão

---

## 👨‍💻 Autor
**Gabriel Miranda**  
QA Manual | Quality Assurance em formação  

📌 Projeto criado para fins de estudo e portfólio.
