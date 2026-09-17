# Inventário e Mapeamento de Dados Pessoais (Data Mapping) - LGPD

## 1. Objetivo do Projeto
Documentar o ciclo de vida dos dados pessoais tratados por um departamento de Recursos Humanos (RH) fictício, identificando a finalidade, a base legal (conforme Art. 7º da LGPD) e as medidas de segurança aplicadas para mitigar riscos de vazamento.

---

## 2. Inventário de Fluxo de Dados (Data Flow)

Abaixo está o mapeamento detalhado das operações de tratamento de dados realizadas pela organização:

| Processo / Atividade | Dados Pessoais Coletados | Categoria de Dados | Finalidade do Tratamento | Base Legal (Art. 7º LGPD) | Tempo de Retenção | Medidas de Segurança |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Recrutamento e Seleção** | Nome, E-mail, Telefone, Histórico Profissional. | Comuns | Triagem de currículos e contato para entrevistas de emprego. | Consentimento ou Execução de Contrato (Fase Pré-contratual) | 6 meses após o fim do processo seletivo. | Controle de acesso restrito à pasta; Criptografia em repouso. |
| **Admissão de Funcionário** | CPF, RG, Endereço, Dados Bancários, Exame Médico. | Comuns e Sensíveis (Saúde) | Registro em carteira, pagamento de salário e benefícios sociais. | Cumprimento de Obrigação Legal ou Regulatória | Duração do contrato + 5 anos (fins trabalhistas/fiscais). | Controle de acessos baseado em perfil (RBAC); Logs de auditoria ativos. |

---

## 3. Análise de Compartilhamento com Terceiros
*   **Operador Externo:** Empresa terceirizada de contabilidade (Processamento de Folha de Pagamento).
*   **Salvaguardas Contratuais:** Cláusulas de confidencialidade estritas, auditorias de segurança periódicas do parceiro e exigência mútua de conformidade com os padrões da ISO 27001.

---

## 4. Direitos dos Titulares e Eliminação de Dados
*   Os dados são eliminados permanentemente através de métodos seguros de descarte digital após o término do período de retenção estabelecido legalmente.
