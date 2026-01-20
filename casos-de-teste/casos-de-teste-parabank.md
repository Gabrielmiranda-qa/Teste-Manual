# 🧪 Testes Manuais – Sistema Bancário (ParaBank)

## 📌 Visão Geral
Este repositório contém o **relatório de testes manuais** realizados no sistema bancário fictício **ParaBank**, com foco na validação funcional, regras de negócio e identificação de falhas críticas de segurança.

Os testes foram executados simulando cenários reais de uso, abrangendo funcionalidades essenciais como **login, transferências, atualização de dados, empréstimos, ATM e pagamento de contas**.

---

## 👤 QA Responsável
- **Nome:** Gabriel Miranda  
- **Perfil:** QA Júnior  
- **Tipo de Teste:** Manual  
- **Plataforma:** Web  

---

## 🎯 Objetivo dos Testes
Garantir que:
- As funcionalidades principais operem corretamente
- As regras de negócio sejam respeitadas
- Os dados sejam validados adequadamente
- Vulnerabilidades críticas sejam identificadas

---

## 🧩 Escopo Testado
- Login
- Página principal (saldo da conta)
- Transferências
- Atualização de dados do usuário
- Empréstimos
- ATM
- Pagamento de contas

---

## ✅ Pontos Validados com Sucesso
- O sistema bloqueia login com campos obrigatórios vazios.
- Login realizado com sucesso com credenciais válidas.
- Mensagens de erro exibidas corretamente para usuário inexistente ou campos não preenchidos.
- Bloqueio de acesso quando apenas usuário ou senha é informado.
- Navegação fluida ao acessar a página principal via tecla **Enter**.
- Sistema aceita letras maiúsculas sem impacto no login.
- Mensagens de erro claras e compreensíveis.
- Pagamento de contas funcionando corretamente.
- Sistema sem lentidão perceptível durante os testes.

---

## 🚨 Falhas Identificadas

### 🚨 Vulnerabilidade Crítica – Exposição de Código-Fonte
**Severidade:** Crítica  

O módulo **ATM** apresenta falha funcional e expõe o **código-fonte completo do sistema bancário** ao usuário final.

**Impacto:**
- Alto risco de invasão
- Possível vazamento de dados sensíveis
- Comprometimento total da segurança da aplicação

---

### 🔴 Regra de Negócio – Transferência Acima do Saldo
**Severidade:** Alta  

O sistema permite realizar transferências com valores **superiores ao saldo disponível**, sem bloqueio ou mensagem de erro.

**Impacto:**
- Saldo negativo
- Inconsistência financeira
- Risco de prejuízo

---

### 🟡 Validação de Dados – Código Postal (CEP)
**Severidade:** Média  

Na funcionalidade de atualização de dados, o campo de código postal:
- Aceita letras
- Permite envio em branco

Esse comportamento diverge da validação aplicada na página principal.

**Impacto:**
- Dados inconsistentes
- Falta de padronização

---

### 🔴 Empréstimos – Erro em Valores Elevados
**Severidade:** Alta  

O sistema apresenta erro ao processar valores de empréstimo muito altos.  
Em casos de saldo insuficiente, a mensagem **"fundos insuficientes"** é exibida corretamente.

---

## ⚠️ Priorização de Correção

| Item | Severidade | Justificativa |
|------|-----------|---------------|
| Exposição de Código | 🚨 Crítica | Compromete a segurança do sistema |
| Transferência sem Saldo | 🔴 Alta | Viola regra de negócio |
| Validação de CEP | 🟡 Média | Inconsistência de dados |

---

## 🧠 Conclusão Técnica
O sistema apresenta boa estabilidade funcional, porém possui **falhas críticas de segurança e validação de regras de negócio**.

A correção imediata da vulnerabilidade do **ATM** e das regras de transferência é essencial antes de qualquer evolução do sistema.

---

## 🔄 Próximos Passos
- Correção das falhas críticas
- Execução de testes de regressão
- Reforço das validações numéricas
- Revisão de segurança
