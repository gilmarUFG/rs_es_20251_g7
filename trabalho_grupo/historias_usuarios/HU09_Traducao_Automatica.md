## **HU09 — Tradução Automática de Mensagens**

**Como** usuário da plataforma,  
**quero** que as mensagens enviadas em idiomas diferentes sejam automaticamente traduzidas,  
**para que** eu possa entender e responder sem barreiras linguísticas.

### Critérios de Aceitação:

-   O idioma de destino deve respeitar as configurações do usuário receptor.
    
-   A mensagem original deve poder ser acessada junto da tradução.
    
-   Traduções devem ocorrer em tempo real ou com atraso máximo de 3 segundos.
    

### Fluxo Principal:

1.  Um usuário envia mensagem em idioma X.
    
2.  O sistema detecta o idioma e traduz para o idioma do receptor.
    
3.  A mensagem traduzida aparece no chat com opção de visualizar o texto original.
    

### Fluxo Alternativo:

-   Se o receptor fala o idioma original, ele pode optar por desativar a tradução automática.
    

### Tratamento de Erros:

-   Caso a tradução falhe, exibir: “Falha ao traduzir. Clique para visualizar mensagem original.”
    

### Rastreabilidade:

-   Relacionado à RF10 (ChatBot pode explicar como alterar o idioma).
    
