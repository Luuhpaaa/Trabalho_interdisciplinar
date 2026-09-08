# User Flow e Wireframes
 
## 1. User Flow
 
### Fluxo 01 — Monitoramento, Metas e Alertas
 
**Objetivo do usuário:**

Acompanhar em tempo real o tempo de uso diário, definir metas de tempo, receber alertas visuais.

 
**Ator:**

Usuário
 
**Histórias de Usuário relacionadas:**
- HU01 Exibição de Tempo: O usuário visualizará o tempo acumulado do dia para ter clareza sobre o consumo total.
- HU02 Configuração de Limites: O usuário cadastra o limite diário.
 
**Diagrama:**

graph TD
    Start([Início]) --> LoadDash[Carregar Dashboard]
    LoadDash --> DisplayTime[Exibir Tempo Acumulado do Dia em cada aplicativo]
    
    DisplayTime --> ActionChoice{Deseja definir meta?}
    
    ActionChoice -- Sim --> InputLimit[Inserir ou Alterar Limite Diário em Horas]
    InputLimit --> SaveLimit[Salvar Limite]

    
**### Fluxo 02 - Análise de Desempenho e Saúde Digital**

**Objetivo do usuário:**

Analisar gráficos semanais de consumo de internet para identificar padrões de uso e receber sugestões práticas de atividades offline após atingir a meta diária.

 
**Ator:**

Usuário
 
**Histórias de Usuário relacionadas:**
- HU02 Alerta: O usuário recebe um alerta visual ao atingir o tempo definido anteriormente.
- HU03 Histórico e Relatórios Comparativos: Exibir gráfico dos últimos 7 dias.
- HU04 Sugestão de Desconexão: Apresentar dicas de atividades offline no momento do alerta de limite.
   
**Diagrama:**
 flowchart TB
    SaveLimit["SaveLimit"] --> CheckLimit["CheckLimit"]
    CheckLimit -- Sim --> TriggerAlert["Disparar Notificação"]
    StartAlert(["Notificação de Limite Atingido"]) --> DisplayTip["Dica Prática de Atividade Offline"]
    DisplayTip --> UserOption{"Deseja ver histórico?"}
    UserOption -- Sim --> NavReports["Navegar para Tela de Histórico"]
    UserOption -- Não --> End(["Encerrar ou Continuar"])
    NavReports --> LoadChart["Carregar Gráfico de Consumo dos Últimos 7 Dias"]
    LoadChart --> ShowStats["Exibir Comparativo"]
    ShowStats --> End
    CheckLimit -- Não --> End
    TriggerAlert --> StartAlert
