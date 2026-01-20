# Teste-Manual
# 🧪 Projeto de Testes Manuais – Swag Labs (Sauce Demo)

## 📌 Contexto do Teste

Os testes foram realizados no site **Swag Labs (Sauce Demo)** com foco no fluxo principal do usuário  
(**login → navegação → compra**), além da verificação de **usabilidade, responsividade e acessibilidade**.

Para apoiar a execução e organização dos testes, foi utilizada uma **planilha de controle**, onde foram registrados:
- Casos de teste  
- Status de execução  
- Observações  
- Bugs identificados  

De forma geral, o sistema funciona bem, porém foram encontrados alguns **bugs e pontos de melhoria** que impactam a experiência do usuário.

---

## 📊 Resultado Geral dos Testes

| Área | Resultado |
|-----|----------|
| ✅ Login (standard_user) | Funcionando normalmente |
| 🔐 Usuário bloqueado (locked_out_user) | Bloqueio correto |
| 🧪 Usuário problemático (problem_user) | Login ok, porém imagens com falha |
| 🛒 Processo de compra | Funciona, mas carrinho não é limpo após a compra |
| 👁️‍🗨️ Usabilidade | Navegação simples e intuitiva |
| 📱 Responsividade | Boa no geral, com falhas em alguns tamanhos de tela |

---

## 📝 Pontos Observados Durante os Testes

### 🔐 Login

- O login com **standard_user** funciona conforme esperado.
- O usuário **locked_out_user** é corretamente impedido de acessar o sistema.

**Observação de usabilidade:**
- O ícone para exibir a senha desaparece quando o mouse sai da área.
- Isso pode atrapalhar o usuário.
- O ideal seria manter o ícone visível até que o usuário decida ocultar a senha manualmente.

---

### 🛒 Checkout

- O fluxo de compra pode ser finalizado sem erros.

**Problema encontrado:**
- Após concluir a compra, o produto continua aparecendo no carrinho.
- Isso pode causar confusão e passar a sensação de que a compra não foi concluída corretamente.

---

### 📷 Imagens de Produtos (problem_user)

- Ao utilizar o usuário **problem_user**, algumas imagens de produtos não carregam.
- O problema ocorre de forma recorrente, indicando falha no carregamento visual para esse perfil de usuário.

---

### 📱 Responsividade

- Em resoluções intermediárias, o layout apresenta problemas visuais.

**Foram observados:**
- Elementos desalinhados  
- Colunas comprimidas  

**Sugestão:**
- Ajustes adicionais com **media queries** podem resolver o problema.

---

### ♿ Acessibilidade

- **Pontuação Lighthouse:** 57
- A pontuação indica necessidade de melhorias, principalmente em:
  - Contraste
  - Semântica
  - Navegação por teclado

---

## 📄 Planilha de Testes Utilizada

Durante a execução dos testes, foi utilizada uma **planilha de controle** para organizar e acompanhar os testes realizados.

A planilha contém:
- ID do caso de teste  
- Descrição do teste  
- Passos executados  
- Resultado esperado  
- Re

