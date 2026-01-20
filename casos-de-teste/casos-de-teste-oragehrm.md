# 🧪 Resultados dos Testes Manuais – OrangeHRM

## 📌 Informações Gerais
- **Sistema:** OrangeHRM (Demo)
- **URL:** https://opensource-demo.orangehrmlive.com/
- **Tipo de Teste:** Manual
- **Plataforma:** Web
- **QA Responsável:** Gabriel Miranda

---

## 🎯 Objetivo
Documentar os **resultados da execução dos casos de teste manuais** realizados no sistema OrangeHRM, avaliando funcionalidades principais, regras de negócio e comportamento do sistema em cenários válidos e inválidos.

---

## ✅ Resultados dos Casos de Teste

### 🔐 Login
O sistema **atendeu corretamente** todos os cenários de teste relacionados ao login:

- Login realizado com sucesso com credenciais válidas
- Campos vazios **não são aceitos**
- Senhas incorretas são recusadas
- Informações inválidas são corretamente bloqueadas
- Mensagens de erro exibidas de forma clara
- Nenhum erro funcional identificado neste módulo

**Status:** ✅ Aprovado

---

### 👤 Cadastro de Funcionário (Add Employee)
- O cadastro de funcionários ocorreu de forma fluida
- Todos os campos obrigatórios foram validados corretamente
- Nenhum erro funcional identificado durante o processo

**Status:** ✅ Aprovado

---

### ⏱️ Timesheet (Controle de Horas)
- O sistema **permite adicionar horas referentes a dias futuros**, sem validação se o colaborador trabalhou nesses dias

**Observação:**  
Esse comportamento pode representar **falha de regra de negócio**, dependendo da política da empresa.

**Status:** ⚠️ Aprovado com ressalva

---

### 🛠️ Administração / Manutenção
- Acesso à área de manutenção realizado com sucesso
- Registros de acesso podem ser visualizados normalmente
- É possível limpar registros de funcionários sem erros

**Status:** ✅ Aprovado

---

### 💰 Reivindicações (Claims)
- É possível atribuir reivindicações normalmente
- O sistema aceita diferentes moedas
- Nenhum erro funcional identificado

**Status:** ✅ Aprovado

---

### 📊 Performance
- Visualização da performance de colaboradores cadastrados ocorre sem erros
- Alteração das informações de performance funciona corretamente

**Status:** ✅ Aprovado

---

### 🏖️ Leave (Licenças)
- Adição e exclusão de configurações de licença funcionam corretamente
- Geração de relatórios de licença ocorre sem falhas
- Atribuição e remoção de direitos de licença aos funcionários ocorre normalmente

**Status:** ✅ Aprovado

---

### ⏳ Regras de Tempo
- O sistema reprova corretamente:
  - Jornadas com tempo excessivo
  - Registros sem balanceamento de horas

**Status:** ✅ Aprovado

---

### 🔒 Sessão do Usuário
- O sistema realiza **logout automático** após longo período de inatividade
- Nenhum erro identificado nesse comportamento

**Status:** ✅ Aprovado

---

## ⚠️ Pontos de Atenção Identificados

| Módulo | Observação | Severidade |
|------|-----------|-----------|
| Timesheet | Permite lançar horas em dias futuros | Média |

---

## 🧠 Conclusão
O sistema OrangeHRM apresentou **alto nível de estabilidade e confiabilidade** durante a execução dos testes manuais.  
A maioria dos módulos funcionou conforme esperado, sem erros funcionais.

O único ponto de atenção identificado refere-se ao **controle de horas no Timesheet**, que pode permitir inconsistências dependendo das regras de negócio da organização.

---

## 📌 Considerações Finais
Este relatório demonstra:
- Execução completa de testes manuais
- Validação de múltiplos módulos do sistema
- Análise crítica de regras de negócio
- Documentação clara e profissional

