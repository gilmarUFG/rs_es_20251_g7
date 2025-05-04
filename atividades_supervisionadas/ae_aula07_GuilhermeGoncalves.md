# Técnicas para Especificação de Requisitos

## 1. Casos de Uso

**Descrição:**  
Casos de uso descrevem como um usuário (ou outro sistema) interage com o sistema para atingir um objetivo específico. Focam nas interações e fluxos de eventos entre o ator e o sistema.

**Aplicabilidade:**  
São especialmente úteis em sistemas interativos com múltiplos tipos de usuários, como plataformas online, apps e sistemas corporativos.

**Vantagens:**
- Linguagem próxima da forma como os usuários pensam.
- Permite visualizar o comportamento do sistema em diferentes situações.
- Ajuda a identificar fluxos alternativos e exceções.

**Desvantagens:**
- Pode não detalhar requisitos técnicos.
- Pode gerar documentos longos e difíceis de manter se o sistema tiver muitos casos.

---

## 2. Histórias de Usuário
**Descrição:**  
As histórias de usuário são uma técnica ágil que descreve funcionalidades do ponto de vista do usuário. Têm uma estrutura simples:  
**Como [tipo de usuário], eu quero [ação] para que [benefício].**

**Aplicabilidade:**  
Muito utilizadas em metodologias ágeis como Scrum e Kanban. São ideais quando se deseja entregar valor de forma incremental e iterativa.

**Vantagens:**
- Linguagem simples, fácil para todos os envolvidos entenderem.
- Facilitam a priorização e planejamento de entregas.
- Focam no valor entregue ao usuário final.

**Desvantagens:**
- Pouco detalhadas sozinhas — precisam de critérios de aceitação ou complementos técnicos.
- Podem gerar ambiguidades se mal escritas ou sem validação.

---

# Especificação de Requisitos do Cenário 

## Requisito A — Técnica: Casos de Uso

**Título do Caso de Uso:** *Geração de Relatórios de Produtividade com IA*

**Ator Principal:** Gestor de Projetos

**Descrição:**  
O gestor acessa a plataforma e gera um relatório de produtividade da equipe, baseado em dados processados por IA (tempo em tarefas, foco, pausas, interações). O sistema apresenta o resultado com gráficos e insights.

**Fluxo Principal:**
1. O gestor faz login na plataforma.
2. Acessa o menu “Relatórios”.
3. Seleciona o período desejado.
4. A IA processa os dados da equipe.
5. O sistema apresenta gráficos e recomendações.
6. O gestor pode exportar o relatório.

**Fluxos Alternativos:**
- Se não houver dados suficientes, a IA avisa e sugere aguardar mais tempo de uso da plataforma.

---

## Requisito B — Técnica: História de Usuário

**ID:** HU-004

**História:**  
**Como** colaborador da empresa,  
**quero** integrar meu calendário do Google com a plataforma,  
**para que** eu possa agendar e visualizar minhas reuniões sem sair do sistema.

**Critérios de Aceitação:**
- O usuário deve poder conectar sua conta Google via OAuth.
- A plataforma deve exibir todos os eventos agendados no painel de controle.
- O usuário deve poder criar eventos na plataforma que sejam refletidos automaticamente no Google Agenda.
- A sincronização deve ocorrer em tempo real ou a cada 5 minutos.
