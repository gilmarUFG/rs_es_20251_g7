# Técnicas para Especificação de Requisitos

## Técnica 1: Casos de Uso (Use Cases)

### Descrição:

A técnica de **Casos de Uso** descreve as interações entre os usuários (atores) e o sistema para atingir um objetivo específico. Utiliza uma linguagem natural estruturada e pode ser complementada com diagramas UML.

### Cenários de Aplicação:

-   Projetos com forte interação entre usuários e o sistema;
    
-   Aplicações orientadas a serviços ou funcionalidades;
    
-   Ideal para captar requisitos funcionais em sistemas interativos.
    

### Vantagens:

-   Facilidade de compreensão por usuários não técnicos;
    
-   Fornece uma visão centrada no usuário;
    
-   Ajuda na identificação de funcionalidades principais.
    

### Desvantagens:

-   Pode se tornar extenso em sistemas muito complexos;
    
-   Nem sempre é adequado para capturar requisitos não funcionais;
    
-   Pode omitir detalhes técnicos importantes.
    

----------

## Técnica 2: Especificação baseada em Requisitos Funcionais (Estilo Shall)

### Descrição:

Essa técnica usa sentenças formais e padronizadas para descrever o que o sistema **deve fazer**. Usa-se a palavra-chave **“shall”** para indicar obrigações.

### Cenários de Aplicação:

-   Projetos com requisitos formais ou contratuais;
    
-   Sistemas críticos ou regulados (ex: aeroespacial, bancário);
    
-   Quando é necessário verificar os requisitos de forma objetiva.
    

### Vantagens:

-   Clareza e precisão;
    
-   Fácil verificação e validação;
    
-   Permite rastreabilidade com testes.
    

### Desvantagens:

-   Pouco intuitivo para usuários finais;
    
-   Pode dificultar a visualização do fluxo de interação;
    
-   Foco limitado na experiência do usuário.
    

----------

# Especificação de Requisitos para o Cenário: Plataforma com IA para Produtividade no Trabalho Remoto

## Requisito A – Especificado com a Técnica de Casos de Uso

### Caso de Uso: Recomendação de Tarefas Automatizadas

**Ator Principal**: Usuário remoto  
**Pré-condição**: O usuário está autenticado na plataforma  
**Fluxo principal**:

1.  O usuário acessa o painel da plataforma;
    
2.  O sistema analisa o histórico de atividades e dados contextuais;
    
3.  O sistema exibe uma lista de tarefas recomendadas com base na prioridade e urgência;
    
4.  O usuário pode aceitar ou rejeitar as recomendações.
    

**Pós-condição**: As tarefas aceitas são adicionadas automaticamente à agenda do usuário.

----------

## Requisito B – Especificado com Requisito Funcional (Estilo Shall)

> **ID**: RF-002  
> **Descrição**: O sistema **shall** permitir que os usuários iniciem sessões de brainstorming com suporte de IA, gerando ideias automaticamente com base nos tópicos digitados, em até 5 segundos após a entrada do usuário.
