# Sistema de Reserva de Hotéis

## Requisitos Funcionais:

- RF1. O sistema deve permitir que os usuários pesquisem hotéis por localização e datas.
- RF2. O sistema deve permitir que os usuários se cadastrem antes de realizar uma reserva online, incluindo a coleta de informações como nome, e-mail, telefone e dados de pagamento.
- RF3. O sistema deve permitir que os usuários visualizem detalhes do quarto e do hotel.
- RF4. O sistema deve enviar e-mails de confirmação de reserva.
- RF5. O sistema deve permitir que os usuários efetuem o cancelamento de reservas.
- RF6. O sistema deve permitir que os usuários visualizem, alterem ou cancelem suas reservas diretamente em sua conta após o login.
- RF7. O sistema deve oferecer múltiplas opções de pagamento, como cartão de crédito, boleto bancário e pagamento via carteira digital, durante o processo de reserva.
- RF8. O sistema deve permitir que os usuários deixem avaliações e comentários sobre o hotel e o quarto após o check-out, e visualizem as avaliações de outros hóspedes ao fazerem a reserva.

## Requisitos Não Funcionais:

- RNF1. O sistema deve ser rápido, com tempo de resposta inferior a 2 segundos para pesquisa de hotéis.
- RNF2. O sistema deve estar disponível 24/7 e ser resistente a falhas.
- RNF3. O sistema deve ser seguro, utilizando criptografia para transações de pagamento.
- RNF4. O sistema deve ser compatível com dispositivos móveis e navegadores modernos.
- RNF5. O sistema deve ser capaz de lidar com até 10.000 reservas simultâneas.
- RNF6. O sistema deve realizar backups diários dos dados dos usuários e das reservas para garantir a recuperação em caso de falha.
- RNF7. O sistema deve ser projetado de forma modular e documentada para facilitar futuras atualizações e manutenção, garantindo que qualquer correção ou melhoria possa ser implementada rapidamente sem impactar a disponibilidade do serviço.
- RNF8. O sistema deve ser acessível por meio de aplicativos móveis (iOS e Android) e navegadores web modernos, proporcionando uma experiência consistente e responsiva em todas as plataformas.

## Regras de Negócio:

- RN1. **Disponibilidade de Quarto**
   - **Descrição**: Um quarto só pode ser reservado se ele estiver disponível para as datas solicitadas.
   - **Exemplo**: Se um usuário tenta reservar um quarto de 1º a 5 de junho, o sistema deve verificar se o quarto está livre durante todo o período. Caso contrário, o sistema deve informar ao cliente que não há disponibilidade.

- RN2. **Pagamento**
   - **Descrição**: A reserva só será confirmada após o pagamento integral ou o pagamento parcial de 50% do valor na hora da reserva.
   - **Exemplo**: A política do hotel exige o pagamento de 50% na hora da reserva e o restante até 7 dias antes do check-in, o sistema deve bloquear a reserva até que o pagamento inicial seja confirmado.

- RN3. **Cancelamento**
   - **Descrição**: O cliente pode cancelar a reserva sem penalidades até uma determinada data, após a qual será cobrada uma taxa de cancelamento.
   - **Exemplo**: Se o cliente cancelou a reserva com até 48 horas de antecedência, ele não será cobrado. Após esse prazo, o sistema deve aplicar uma taxa de cancelamento de 20% do valor total da reserva.

- RN4. **Acompanhante**
   - **Descrição**: O número de acompanhantes permitidos por quarto é limitado de acordo com a capacidade do quarto.
   - **Exemplo**: Se um quarto tem capacidade para até 2 adultos e 2 crianças, o sistema deve impedir a reserva de 3 ou mais adultos para o mesmo quarto, ou oferecer a opção de reservar um quarto adicional.

- RN5. **Data de Check-in/Check-out**
   - **Descrição**: O horário de check-in e check-out deve ser respeitado. O check-in pode ocorrer apenas após o horário estabelecido, e o check-out deve ocorrer até o horário limite do dia da saída.
   - **Exemplo**: Se o check-in está disponível a partir das 14:00 e o check-out deve ser feito até às 12:00, o sistema deve garantir que essas regras sejam aplicadas e notificar os hóspedes sobre o horário de entrada e saída.

- RN6. **Limite de Reservas por Usuário**
   - **Descrição**: O sistema deve permitir que cada usuário faça um número máximo de 3 reservas simultâneas, a menos que haja uma solicitação especial e aprovação do hotel.
   - **Exemplo**: Um usuário tentará reservar 4 quartos simultaneamente para diferentes datas, mas o sistema só permitirá 3 reservas ao mesmo tempo sem a aprovação do hotel.

- RN7. **Política de Crianças e Acomodações**
   - **Descrição**: Crianças de até 5 anos devem ser acomodadas sem custo adicional se compartilharem o quarto com os pais. Crianças maiores de 5 anos devem pagar uma taxa adicional.
   - **Exemplo**: Se um hóspede reserva um quarto para dois adultos e uma criança de 4 anos, a criança ficará sem custo. Porém, se a criança tiver 6 anos, será cobrada uma taxa adicional.

- RN8. **Desconto para Reservas Antecipadas**
   - **Descrição**: O sistema deve aplicar um desconto de 10% em reservas feitas com mais de 30 dias de antecedência para incentivar reservas antecipadas.
   - **Exemplo**: Se um hóspede fizer uma reserva em 1º de dezembro para o mês de janeiro, ele receberá 10% de desconto no valor total da reserva.

