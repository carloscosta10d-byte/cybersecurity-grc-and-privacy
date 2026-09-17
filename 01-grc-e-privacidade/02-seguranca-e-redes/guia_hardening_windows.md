# Guia Prático de Hardening - Estações de Trabalho Windows 11

Este guia técnico documenta os passos necessários para aplicar as diretrizes da Política de Segurança da Informação nas máquinas dos colaboradores.

## 1. Configuração de Bloqueio de Tela por Inatividade
Para garantir que a tela bloqueie em 5 minutos:
1. Abrir o menu Iniciar e buscar por `Opções de Proteção de Tela`.
2. Alterar o tempo de **Aguardar** para `5` minutes.
3. Marcar a opção `Ao reiniciar, exibir tela de logon`.

## 2. Desativação de Contas de Administrador Local
Para mitigar riscos de privilégios excessivos:
1. Abrir o `Executar` (Win + R) e digitar `lusrmgr.msc`.
2. Ir em **Usuários** e clicar duas vezes na conta `Administrador`.
3. Marcar a caixa `Conta desativada` e clicar em Aplicar.

## 3. Gerenciamento de Atualizações (Windows Update)
1. Ir em **Configurações** > **Windows Update**.
2. Garantir que a opção `Obtenha as atualizações mais recentes assim que elas estiverem disponíveis` esteja ativada.
