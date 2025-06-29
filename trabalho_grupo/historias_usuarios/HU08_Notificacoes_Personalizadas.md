
## **HU08 — Notificações Personalizadas**

**Como** colaborador,  
**quero** receber sugestões baseadas no meu comportamento,  
**para que** eu possa melhorar minha rotina e bem-estar.

### Critérios de Aceitação:

-   Notificações devem considerar tempo contínuo de atividade, ausência de pausas, entre outros fatores.
    
-   As mensagens devem ser discretas, com linguagem amigável.
    
-   O usuário pode optar por não receber esse tipo de notificação.
    

### Fluxo Principal:

1.  O sistema detecta atividade contínua por mais de 90 minutos.
    
2.  Envia uma notificação sugerindo uma pausa.
    
3.  O usuário pode aceitar, ignorar ou adiar a sugestão.
    

### Fluxo Alternativo:

-   O sistema pode sugerir diferentes ações, como alongamentos, pausas de foco, etc.
    

### Tratamento de Erros:

-   Caso a IA falhe na análise de comportamento, o sistema não envia notificações naquele período.
    

### Rastreabilidade:

-   Relacionado à RF06 (IA usa os mesmos dados para detectar sobrecarga).
    