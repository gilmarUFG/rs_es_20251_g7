# Técnicas para Especificação de Requisitos

## JAD (Joint Application Development)

JAD é uma metodologia que envolve a participação direta do cliente e usuários finais durante o processo de desenvolvimento de aplicações. Através de workshops e sessões estruturadas, os participantes colaboram para definir requisitos do sistema de forma conjunta e eficiente.

**Cenários aplicáveis:**

- Projetos novos ou melhorias de produtos existentes
- Projetos envolvendo grupos de usuários ou responsabilidades interdepartamentais
- Projetos considerados críticos para o sucesso da organização
- Organizações com histórico problemático entre produtos e usuários finais
- Quando é necessário consolidar reuniões, e-mails e telefonemas em sessões estruturadas

**Vantagens:**

- Melhora o tempo de entrega devido à abordagem coordenada
- Redução de custos por meio de análise acelerada dos requisitos
- Simplifica o processo identificando participantes, usuários e problemas rapidamente
- Clarifica os requisitos de forma unânime
- Satisfaz o cliente por envolvê-lo no desenvolvimento do sistema
- Elimina elementos de risco através do trabalho em equipe

**Desvantagens:**

- Pode ser muito caro se o tamanho do projeto não justificar o processo
- Requer compromisso de tempo dos participantes
- Necessita de suporte adequado da gerência executiva
- Pode ser contraproducente sem participação adequada

## Prototipação

Técnica que consiste em criar versões iniciais do sistema baseadas nos resultados de coletas preliminares de requisitos para mostrar aos clientes uma solução viável. O cliente pode então fornecer mais requisitos ou refinar os existentes.

**Cenários aplicáveis:**

- Quando os requisitos são difíceis de articular
- Para sistemas com interfaces de usuário complexas
- Quando é essencial obter feedback do cliente nas fases iniciais
- Para validar conceitos antes do desenvolvimento completo
- Quando a documentação de um sistema existente está ausente

**Vantagens:**

- Permite visualização antecipada e validação de conceitos
- Facilita feedback do cliente no início do processo
- Ajuda a identificar requisitos ausentes ou pouco claros
- Reduz o risco de desenvolver a solução errada
- Ciclo contínuo de refinamento até atender às necessidades do cliente

**Desvantagens:**

- Pode consumir tempo criar múltiplos protótipos
- Clientes podem confundir um protótipo com o produto final
- Pode estabelecer expectativas irrealistas
- Pode levar a expansão de escopo se não for gerenciado adequadamente

## Requisito A: Sistema de Análise Inteligente de Reuniões (usando JAD)

**Documentação da Sessão JAD:**

**Participantes:**

- Gerente de Projeto (Facilitador)
- Arquiteto de Software
- Especialistas em IA (2)
- Designer de UI/UX
- Product Owner
- Representantes de usuários finais (4)
- Especialista em QA
- Analista de Negócios (Relator)

**Resultados da Sessão:**

1. **Requisitos do Sistema:**
   - O sistema deve transcrever automaticamente reuniões gravadas
   - O sistema deve gerar resumos concisos das discussões
   - O sistema deve identificar pontos de ação, responsáveis e prazos
   - Os resumos devem estar disponíveis em até 1 hora após o término da gravação
   - Os participantes devem poder editar/corrigir o resumo gerado
   - A precisão na identificação de pontos de ação deve ser de pelo menos 80%
2. **Fluxo de Interação:**
   - Após a conclusão da reunião, o sistema inicia automaticamente o processamento
   - O sistema notifica os participantes quando o resumo está disponível
   - Os participantes podem acessar o resumo através da página da reunião
   - Os participantes podem editar o resumo ou adicionar informações ausentes
   - O sistema permite exportar o resumo em diferentes formatos
3. **Integrações:**
   - Plataformas de videoconferência
   - Sistemas de gerenciamento de projetos
   - Ferramentas de calendário
   - Sistemas de notificação
4. **Requisitos de Privacidade:**
   - As gravações e transcrições devem ser armazenadas com segurança
   - O acesso aos resumos deve ser limitado aos participantes da reunião
   - O sistema deve respeitar as configurações de privacidade dos usuários

## Requisito B: Painel de Produtividade do Trabalho Remoto (usando Prototipação)

**Documentação de Prototipação:**

**Objetivos do Protótipo:**

- Visualizar um painel que monitora e otimiza a produtividade no trabalho remoto
- Obter feedback sobre métricas e visualizações relevantes
- Validar experiência do usuário para autogerenciamento

**Iterações de Protótipos:**

**Iteração 1: Wireframes de baixa fidelidade**

- Layout básico do painel
- Áreas para métricas chave
- Visualização simples de tempo produtivo vs. improdutivo
- Seção para sugestões de melhoria

**Feedback dos Stakeholders:**

- Necessidade de personalização de métricas
- Preocupações com privacidade na coleta de dados
- Desejo por comparações de tendências ao longo do tempo
- Solicitação de recursos de estabelecimento de metas

**Iteração 2: Mockup interativo de média fidelidade**

- Redesign com métricas personalizáveis
- Controles de privacidade aprimorados
- Gráficos de tendências ao longo do tempo
- Ferramenta de estabelecimento de metas

**Feedback dos Stakeholders:**

- Interface ainda muito complexa
- Desejo por sugestões baseadas em IA
- Necessidade de integrações com ferramentas existentes
- Solicitação de alertas para comportamentos não saudáveis

**Iteração 3: Protótipo funcional de alta fidelidade**

- Interface simplificada e intuitiva
- Assistente de IA para sugestões de produtividade
- Integrações com ferramentas populares
- Alertas configuráveis para comportamentos não saudáveis
- Modelo de privacidade "opt-in" para todas as métricas

**Requisitos Finais Baseados nos Testes de Protótipo:**

- Dashboard personalizável com métricas escolhidas pelo usuário
- Visualizações de dados claras e acionáveis
- Sugestões baseadas em IA para melhorar produtividade
- Controles de privacidade granulares para todas as métricas
- Integração com ferramentas de produtividade existentes
- Sistema de metas e celebração de conquistas
- Alertas para comportamentos de trabalho não saudáveis
