# Especificação do Requisito Funcional 
## Sistema de reserva de hotéis
### Requisito escolhido:  RF4. O sistema deve enviar e-mails de confirmação de reserva.

#### **1. Descrição Detalhada do Requisito**

O sistema de reservas de hotéis deve enviar automaticamente um e-mail de confirmação para o hóspede assim que uma reserva for concluída com sucesso. O e-mail deve conter todas as informações relevantes da reserva, incluindo:

-   Nome do hóspede
-   Datas de check-in e check-out
-   Tipo de acomodação
-   Número da reserva
-   Valor total da hospedagem e forma de pagamento
-   Políticas de cancelamento e contato do hotel

O envio do e-mail deve ocorrer imediatamente após a confirmação da reserva. Em caso de falha no envio, o sistema deve tentar reenviar automaticamente até três vezes antes de registrar o erro e notificar a equipe responsável.

#### **2. Identificação das Fontes dos Requisitos**

-   **Clientes/Hóspedes**: Necessitam de uma confirmação oficial da reserva para referência e garantia do serviço contratado.
-   **Equipe de Atendimento do Hotel**: Precisa garantir que os hóspedes recebam a confirmação corretamente para evitar problemas no check-in.
-   **Departamento de TI**: Deve garantir que o envio de e-mails ocorra de forma automatizada e confiável, com um mecanismo de monitoramento de falhas.

#### **3. Fluxos de Execução**

##### **Fluxo Principal**

1.  O usuário realiza uma reserva pelo site ou aplicativo do hotel.
2.  O sistema valida os dados da reserva e confirma a disponibilidade.
3.  A reserva é confirmada e registrada no banco de dados.
4.  O sistema gera um e-mail de confirmação com os detalhes da reserva.
5.  O e-mail é enviado automaticamente para o endereço cadastrado pelo hóspede.
6.  O hóspede recebe o e-mail e pode acessá-lo para verificar as informações.

##### **Fluxo Alternativo – Falha no Envio**

1.  Caso ocorra um erro no envio do e-mail, o sistema tenta reenviar automaticamente até três vezes.
2.  Se todas as tentativas falharem, o sistema gera um alerta para a equipe de suporte.
3.  A equipe de suporte pode reenviar manualmente ou entrar em contato com o hóspede para confirmar a reserva.

#### **4. Perfis de Usuários com Permissão de Execução**

-   **Sistema Automatizado**: Responsável pelo envio dos e-mails de confirmação sem necessidade de intervenção manual.
-   **Equipe de Suporte/Atendimento**: Pode acessar registros de e-mails enviados, reenviar confirmações manualmente e corrigir eventuais problemas.
-   **Hóspede**: Apenas recebe o e-mail de confirmação, sem acesso direto ao sistema de envio.
