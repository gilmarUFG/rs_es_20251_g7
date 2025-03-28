# Especificação do Requisito Funcional

## Sistema de Reserva de Hotéis

### Requisitos Elicitados

Durante o processo de elicitação de requisitos, utilizamos diversas técnicas para garantir um entendimento completo das necessidades dos stakeholders. Através de entrevistas com clientes e equipe de atendimento, workshops colaborativos e análise de cenários de uso, refinamos os seguintes requisitos para o sistema:

#### **1. Envio de E-mails de Confirmação de Reserva (RF4)**

O sistema deve enviar automaticamente um e-mail de confirmação para o hóspede assim que uma reserva for concluída com sucesso. O e-mail deve conter todas as informações relevantes da reserva, incluindo:

- Nome do hóspede
- Datas de check-in e check-out
- Tipo de acomodação
- Número da reserva
- Valor total da hospedagem e forma de pagamento
- Políticas de cancelamento e contato do hotel

Com base na análise de falhas em versões anteriores e benchmarking com concorrentes, estabelecemos um fluxo de tentativa de reenvio automático até três vezes em caso de erro. Caso todas as tentativas falhem, o sistema notificará a equipe de suporte para ação manual.

##### **Questionário de Elicitação - RF4**
- **Por quê?**: Por que é essencial enviar um e-mail de confirmação de reserva?
- **O quê?**: O que o e-mail de confirmação deve conter para ser útil ao hóspede?
- **Como?**: Como o sistema deve processar e garantir o envio correto dos e-mails?
- **Onde?**: Onde o hóspede pode acessar essa confirmação?
- **Quando?**: Quando o sistema deve reenviar a confirmação em caso de falha?
- **Quem?**: Quem deve ser notificado caso ocorra um erro no envio?

#### **2. Notificações de Lembrete de Check-in (Novo Requisito - RF5)**

Com base nas entrevistas realizadas com hóspedes frequentes e na observação do comportamento dos usuários, identificamos a necessidade de um lembrete automático antes da data do check-in. O sistema deve:

- Enviar uma notificação por e-mail e/ou SMS 24 horas antes do check-in.
- Incluir um link para informações adicionais, como horário de entrada e opções de early check-in.
- Permitir que o hóspede confirme a chegada prevista para melhorar a organização da recepção.

##### **Questionário de Elicitação - RF5**
- **Por quê?**: Por que um lembrete de check-in é útil para o hóspede e para o hotel?
- **O quê?**: O que a notificação deve conter para ser informativa e útil?
- **Como?**: Como o sistema deve determinar quais hóspedes devem receber o lembrete?
- **Onde?**: Onde essa notificação será exibida para o hóspede?
- **Quando?**: Quando a notificação deve ser enviada para ter maior eficácia?
- **Quem?**: Quem deve receber essa notificação e quem deve ser alertado sobre confirmações de chegada?

#### **3. Opção de Reenvio de Confirmação pelo Hóspede (Novo Requisito - RF6)**

Com base em questionários e análise de suporte técnico, identificamos que muitos hóspedes perdem o e-mail de confirmação ou inserem um endereço incorreto. Para mitigar esse problema, o sistema deve:

- Permitir que o hóspede solicite o reenvio da confirmação de reserva diretamente pelo site ou aplicativo.
- Verificar e permitir a alteração do e-mail cadastrado antes do reenvio.
- Notificar a equipe de suporte caso a solicitação ocorra mais de uma vez para o mesmo hóspede.

##### **Questionário de Elicitação - RF6**
- **Por quê?**: Por que é importante permitir o reenvio da confirmação de reserva?
- **O quê?**: O que deve ser validado antes de reenviar a confirmação?
- **Como?**: Como o hóspede pode solicitar um novo envio de forma intuitiva?
- **Onde?**: Onde o hóspede pode acessar essa funcionalidade no site ou aplicativo?
- **Quando?**: Quando o sistema deve permitir essa solicitação e há um limite de tentativas?
- **Quem?**: Quem deve ser notificado caso um hóspede faça múltiplas solicitações de reenvio?
#### **4. Identificação das Fontes dos Requisitos**

As principais fontes de requisitos incluem:

- **Clientes/Hóspedes**: Necessitam de uma confirmação oficial da reserva para referência e garantia do serviço contratado.
- **Equipe de Atendimento do Hotel**: Precisa garantir que os hóspedes recebam a confirmação corretamente para evitar problemas no check-in.
- **Departamento de TI**: Deve garantir que o envio de e-mails ocorra de forma automatizada e confiável, com um mecanismo de monitoramento de falhas.
- **Equipe de Suporte de Produto de Primeiro Nível**: Responsável por resolver problemas técnicos relacionados ao envio de e-mails.
- **Agências Reguladoras e Órgãos Profissionais**: Garantem que padrões e regulamentos sejam seguidos no envio de comunicações eletrônicas.
- **Desenvolvedores e Equipe de Operações**: Trabalham para implementar e manter o sistema funcionando corretamente.

Outras fontes de requisitos incluem:

- Versões anteriores do sistema;
- Banco de dados de rastreamento de defeitos;
- Sistemas que interagem com o sistema em desenvolvimento;
- Benchmarking competitivo;
- Pesquisa bibliográfica;
- Normas como ISO/IEC 25010.

#### **5. Fluxos de Execução**

##### **Fluxo Principal**

1. O usuário realiza uma reserva pelo site ou aplicativo do hotel.
2. O sistema valida os dados da reserva e confirma a disponibilidade.
3. A reserva é confirmada e registrada no banco de dados.
4. O sistema gera um e-mail de confirmação com os detalhes da reserva.
5. O e-mail é enviado automaticamente para o endereço cadastrado pelo hóspede.
6. O hóspede recebe o e-mail e pode acessá-lo para verificar as informações.

##### **Fluxo Alternativo – Falha no Envio**

1. Caso ocorra um erro no envio do e-mail, o sistema tenta reenviar automaticamente até três vezes.
2. Se todas as tentativas falharem, o sistema gera um alerta para a equipe de suporte.
3. A equipe de suporte pode reenviar manualmente ou entrar em contato com o hóspede para confirmar a reserva.

#### **6. Perfis de Usuários com Permissão de Execução**

- **Sistema Automatizado**: Responsável pelo envio dos e-mails de confirmação sem necessidade de intervenção manual.
- **Equipe de Suporte/Atendimento**: Pode acessar registros de e-mails enviados, reenviar confirmações manualmente e corrigir eventuais problemas.
- **Hóspede**: Apenas recebe o e-mail de confirmação, sem acesso direto ao sistema de envio.

#### **7. Elicitação de Requisitos**

A elicitação de requisitos envolve o levantamento detalhado das necessidades do sistema. Algumas técnicas utilizadas incluem:

- **Entrevistas com stakeholders**: Consiste na realização de perguntas diretas para coletar informações sobre as necessidades e expectativas dos envolvidos no projeto.
- **Workshops (JAD, JRP)**: Sessões colaborativas onde diferentes stakeholders discutem e refinam os requisitos juntos, promovendo alinhamento entre as partes interessadas.
- **Análise de protocolos e observação do trabalho em campo**: Acompanhar a execução das tarefas no ambiente real permite identificar requisitos tácitos que não seriam facilmente mencionados em entrevistas.
- **Prototipação e design thinking**: Criar versões iniciais e interativas do sistema para coletar feedback antecipado dos usuários, garantindo que o produto final atenda às necessidades.
- **Mapeamento de histórias de usuários**: Técnica que descreve as interações dos usuários com o sistema de forma narrativa, ajudando a compreender melhor suas necessidades e expectativas.
- **ISO/IEC 25010 e regulamentos aplicáveis**: Utilização de normas de qualidade e segurança para garantir que o sistema atenda a padrões reconhecidos no setor.

##### **Modelo de Questionário para Entrevista**

Para garantir uma elicitação eficaz, utilizamos um modelo de questionário baseado em diferentes categorias de perguntas. Essa abordagem busca compreender melhor os requisitos do sistema, verificando aspectos essenciais como funcionalidade, usabilidade e impacto nos usuários.

- **"Como"**: Perguntas que ajudam a entender a execução do requisito e seus impactos. Exemplo: "Como você vai usar esse recurso?" ou "Como saberemos que isso está completo?".
- **"Onde"**: Identifica o contexto de uso do recurso. Exemplo: "Onde o usuário acessaria esse recurso?" ou "Onde os resultados seriam visíveis?".
- **"Quando"**: Define os momentos em que o recurso será acionado e sua importância temporal. Exemplo: "Quando esse recurso será usado?" ou "Quando o recurso falhará?".
- **"Quem"**: Identifica os principais usuários e partes interessadas. Exemplo: "Quem vai usar esse recurso?" ou "Quem entregará as entradas para o recurso?".
- **"O Que"**: Explora detalhes específicos da funcionalidade. Exemplo: "O que esse recurso precisa fazer?" ou "O que precisa acontecer antes e depois?".
- **"Por Quê"**: Avalia a justificativa do requisito e sua relevância. Exemplo: "Qual o benefício do recurso?" ou "Existe alguma outra maneira de conseguir isso?".

---

**Documento atualizado conforme as novas técnicas e conceitos discutidos na aula de 27/03/2025.**

