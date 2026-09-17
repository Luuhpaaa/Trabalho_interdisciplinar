# Protótipo de Alta Fidelidade

## 1. Acesso ao Protótipo

https://www.figma.com/board/a8csoUfeBWn1GRACxXFC51/05-prototipo?node-id=0-1&t=Q1E1WeZGAWusGQhu-1

## 2. Identidade visual

**Cores principais:**
- #2B4C3F — cor primária (navegação ativa, botões principais)
- #D98A3D — cor de destaque (tempo, alarmes, progresso)
- #B14B3D — ações destrutivas
- #F3F5EF — fundo da aplicação
- #1E2620 — texto principal
- #5B6459 — texto secundário

**Tipografia:**
- Space Grotesk — títulos, botões e números de destaque
- Inter — texto de corpo, formulários e dados

## 3. Telas

### Tela 01 — Painel

**Wireframe relacionado:**
- Tela XX

**User Flows relacionados:**
- Fluxo 01

**Histórias de Usuário relacionadas:**
- HU01
- HU02

**Protótipo:**
![Tela 01 — Painel](tela-01-painel.png)

---

### Tela 02 — Alarmes

**Wireframe relacionado:**
- Tela XX

**User Flows relacionados:**
- Fluxo 02

**Histórias de Usuário relacionadas:**
- HU02
- HU04

**Protótipo:**
![Tela 02 — Alarmes](tela-02-alarmes.png)

---

### Tela 03 — Histórico

**Wireframe relacionado:**
- Tela XX

**User Flows relacionados:**
- Fluxo 02

**Histórias de Usuário relacionadas:**
- HU03

**Protótipo:**
![Tela 03 — Histórico](tela-03-historico.png)

## 4. Alterações em relação aos Wireframes

- Alarmes por horário no lugar de um limite diário único com alerta automático (HU02): o usuário cadastra horários específicos (ex.: 21h30) com mensagem ou dica associada, em vez de definir um teto de horas. Justificativa: permite lembretes em múltiplos momentos do dia e evita depender de cálculo de tempo acumulado em tempo real.
- Dica de desconexão (HU04) integrada ao cadastro do alarme, em vez de um pop-up reativo no momento do alerta. Justificativa: mantém o objetivo da história sem depender de notificações do sistema operacional.
- Filtros de rede e período na tela de Histórico, além do gráfico fixo de 7 dias previsto na HU03. Justificativa: o dado já estava disponível na aplicação e o filtro amplia a análise sem custo relevante de implementação.
- Seção "Você sabia?" no Painel, não prevista nas histórias originais, com curiosidades sobre uso de redes sociais. Justificativa: reforça o objetivo de autoconsciência digital do produto.
