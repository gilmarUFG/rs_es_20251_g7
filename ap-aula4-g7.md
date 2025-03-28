# Especificação do Requisito Funcional

## Sistema de Reserva de Hotéis

### Requisito Escolhido: RF4. O sistema deve enviar e-mails de confirmação de reserva.

#### **1. Descrição Detalhada do Requisito**

O sistema de reservas de hotéis deve enviar automaticamente um e-mail de confirmação para o hóspede assim que uma reserva for concluída com sucesso. O e-mail deve conter todas as informações relevantes da reserva, incluindo:

- Nome do hóspede
- Datas de check-in e check-out
- Tipo de acomodação
- Número da reserva
- Valor total da hospedagem e forma de pagamento
- Políticas de cancelamento e contato do hotel

O envio do e-mail deve ocorrer imediatamente após a confirmação da reserva. Em caso de falha no envio, o sistema deve tentar reenviar automaticamente até três vezes antes de registrar o erro e notificar a equipe responsável.

#### **2. Identificação das Fontes dos Requisitos**

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

#### **3. Fluxos de Execução**

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

#### **4. Perfis de Usuários com Permissão de Execução**

- **Sistema Automatizado**: Responsável pelo envio dos e-mails de confirmação sem necessidade de intervenção manual.
- **Equipe de Suporte/Atendimento**: Pode acessar registros de e-mails enviados, reenviar confirmações manualmente e corrigir eventuais problemas.
- **Hóspede**: Apenas recebe o e-mail de confirmação, sem acesso direto ao sistema de envio.

#### **5. Elicitação de Requisitos**

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

