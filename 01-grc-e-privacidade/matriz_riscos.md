# Matriz de Análise e Gestão de Riscos Corporativos (ISO 27001)

## 1. Metodologia de Avaliação
O cálculo do nível de risco é baseado no produto entre a **Probabilidade (P)** e o **Impacto (I)**, adotando uma escala de 1 a 5 para cada critério.

*   **Cálculo:** `Nível de Risco = Probabilidade x Impacto`
*   **Classificação do Risco:**
    *   **1 a 5:** Baixo (Aceitável)
    *   **6 a 12:** Médio (Requer monitoramento)
    *   **15 a 25:** Alto/Crítico (Exige mitigação imediata)

---

## 2. Matriz de Riscos Prática (Tabela de Ativos e Ameaças)

Abaixo estão identificados cenários de risco fictícios para uma infraestrutura corporativa e suas respectivas ações corretivas:

| Ativo Afetado | Ameaça Identificada | P (1-5) | I (1-5) | Nível (P x I) | Impacto Principal (CIA) | Plano de Mitigação / Resposta ao Risco |
| :--- | :--- | :---: | :---: | :---: | :--- | :--- |
| **Banco de Dados de Clientes** | Ataque de Ransomware com sequestro de dados lógicos. | 3 | 5 | **15 (Alto)** | Quebra de Disponibilidade e Integridade. | Implementação de política de backup offline (3-2-1), testes de restauração mensais e proteção de endpoint. |
| **Dispositivos dos Usuários** | Vazamento de credenciais via engenharia social (Phishing). | 4 | 4 | **16 (Alto)** | Quebra de Confidencialidade e Acesso Indevido. | Ativação obrigatória de MFA (Autenticação de Múltiplos Fatores) e treinamentos periódicos de conscientização em segurança. |
| **Estações de Trabalho** | Acesso físico não autorizado a computadores desbloqueados. | 3 | 3 | **9 (Médio)** | Quebra de Confidencialidade. | Configuração de GPO para bloqueio automático de tela por inatividade em 5 minutos (aplicando as diretrizes de Hardening). |
| **Links de Internet da Empresa** | Queda generalizada do provedor principal de conectividade. | 3 | 3 | **9 (Médio)** | Quebra de Disponibilidade do Sistema. | Contratação de um link de internet redundante de operadoras diferentes com failover automático configurado no firewall. |

---

## 3. Monitoramento Contínuo
Os riscos mapeados nesta matriz devem ser revisados trimestralmente ou sempre que houver mudanças significativas na infraestrutura de tecnologia e nos processos organizacionais da instituição.
