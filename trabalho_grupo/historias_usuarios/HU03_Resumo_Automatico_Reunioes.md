# HU-3: Resumo Automático de Reuniões Gravadas

**Como um** participante ou ausente de uma reunião,
**Eu quero** receber um resumo textual gerado automaticamente com os principais pontos discutidos, decisões tomadas e próximos passos definidos em reuniões virtuais gravadas, poucos minutos após o seu término,
**Para que** eu possa rapidamente me atualizar sobre o conteúdo da reunião, sem a necessidade de assistir à gravação completa, economizando tempo e garantindo que nenhuma informação importante seja perdida.

## Critérios de Aceitação

1. O sistema deve:
    - Transcrever o áudio da reunião gravada com precisão mínima de 95%
    - Identificar automaticamente diferentes falantes
    - Filtrar ruídos, conversas paralelas e conteúdo irrelevante
    - Processar reuniões em múltiplos idiomas (pelo menos inglês, português e espanhol)
2. O resumo gerado deve incluir:
    - Tópicos principais discutidos, em ordem cronológica
    - Decisões tomadas e seus responsáveis
    - Itens de ação definidos, com prazos (quando mencionados)
    - Pontos que ficaram pendentes para discussão futura
3. O usuário deve poder:
    - Receber o resumo por e-mail em até 15 minutos após o término da reunião
    - Acessar o resumo através da plataforma
    - Editar o resumo para adicionar informações ou corrigir imprecisões
    - Definir níveis de acesso ao resumo (público, restrito à equipe, confidencial)
    - Solicitar uma versão mais detalhada ou mais concisa do resumo
4. O sistema deve aprender e melhorar com o tempo:
    - Identificando termos técnicos específicos da empresa/equipe
    - Reconhecendo padrões de comunicação da equipe
    - Adaptando-se ao formato específico de diferentes tipos de reuniões (brainstorming, status report, etc.)
5. Deve haver integração com ferramentas populares de videoconferência (Zoom, Teams, Google Meet, etc.)

## Quando essa HU está pronta?

- O tempo médio de geração não ultrapassa 15 minutos após o término da reunião
- A taxa de precisão na identificação de decisões e itens de ação é de pelo menos 90%
