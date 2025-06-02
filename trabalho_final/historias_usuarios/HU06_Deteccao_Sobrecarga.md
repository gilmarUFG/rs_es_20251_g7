## **HU06 — Detecção de sobrecarga de trabalho em colaboradores**

**Como** gestor de equipe,  
**quero** receber alertas da IA quando um colaborador estiver sobrecarregado,  
**para que** eu possa redistribuir tarefas de forma mais justa e eficiente.

### Critérios de Aceitação:

-   A IA deve analisar tempo de execução, número de tarefas e performance recente.
    
-   O sistema deve notificar o gestor apenas se a sobrecarga for acima de um limiar.
    
-   A IA deve sugerir colaboradores elegíveis para receber parte da carga.
    

### Fluxo Principal:

1.  A IA monitora métricas de trabalho dos colaboradores em tempo real.
    
2.  Ao detectar sobrecarga, envia alerta ao gestor com sugestão de redistribuição.
    
3.  O gestor aprova, edita ou ignora a sugestão.
    

### Fluxo Alternativo:

-   Caso a IA não identifique colaboradores disponíveis para redistribuição, o alerta informa apenas a situação de sobrecarga.
    

### Tratamento de Erros:

-   Caso não haja dados suficientes (ex: novo colaborador), exibir mensagem: “Dados insuficientes para análise de carga de trabalho.”
    

### Rastreabilidade:

-   Relacionado à história RF10 (ChatBot pode explicar como funciona a análise de sobrecarga).
    
