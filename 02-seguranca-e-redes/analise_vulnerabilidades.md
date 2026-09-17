# Relatório Técnico: Análise de Vulnerabilidades e Plano de Mitigação

## 1. Escopo e Cenário da Análise
*   **Ambiente Analisado:** Servidor Web Fictício (Ambiente de Homologação)
*   **Sistema Operacional:** Linux Ubuntu Server 20.04 LTS
*   **Ferramenta Utilizada:** Tenable Nessus (Scanner de Vulnerabilidades)
*   **Objetivo:** Identificar brechas de segurança críticas na infraestrutura de rede e propor correções imediatas de acordo com a Tríade CIA.

---

## 2. Vulnerabilidades Identificadas

### 🚨 Vulnerabilidade 1: CVE-2021-44228 (Log4j / Log4Shell)
*   **Severidade:** Crítica (CVSS 10.0)
*   **Descrição:** Brecha de Execução Remota de Código (RCE) encontrada na biblioteca de log do Apache (Log4j). Permite que um atacante execute comandos arbitrários no servidor sem autenticação.
*   **Impacto:** Quebra total de Confidencialidade, Integridade e Disponibilidade.

### ⚠️ Vulnerabilidade 2: Protocolo SSH com Criptografia Fraca (Weak Ciphers)
*   **Severidade:** Média (CVSS 5.3)
*   **Descrição:** O serviço SSH está configurado para aceitar algoritmos de criptografia antigos e considerados fracos (como 3DES e RC4).
*   **Impacto:** Risco de interceptação de tráfego e ataques de Man-in-the-Middle (MitM) na rede.

---

## 3. Plano de Ação e Mitigação (Remediação)

Abaixo estão os procedimentos recomendados para sanar os problemas identificados no ambiente corporativo:

| ID | Vulnerabilidade | Ação de Correção (Remediação) | Status Esperado |
| :--- | :--- | :--- | :--- |
| 01 | Log4j (Log4Shell) | Atualizar a biblioteca Java Log4j para a versão estável mais recente (`Log4j 2.17.1` ou superior). | **Corrigido** |
| 02 | SSH Weak Ciphers | Editar o arquivo `/etc/ssh/sshd_config` para desativar as cifras fracas e forçar o uso de algoritmos robustos (como AES-GCM). | **Corrigido** |
| 03 | Geral | Executar um novo escaneamento de credenciais (Rescan) para validar a eficácia das correções aplicadas. | **Validado** |
