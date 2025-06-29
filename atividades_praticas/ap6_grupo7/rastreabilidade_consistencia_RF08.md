# Rastreabilidade e Análise de Consistência  
## RF08 - Notificações Personalizadas

## Matriz de Rastreabilidade

| Requisito / User Story                  | Relacionado a                      | Descrição / Observações                                                               |
|-----------------------------------------|------------------------------------|----------------------------------------------------------------------------------------|
| RF08 — Notificações Personalizadas      | RF01 — Geração de Relatórios       | Usa métricas de produtividade para disparar notificações                              |
| RF08                                    | RF04 — Recomendação de Tarefas     | Alertas podem sugerir início de tarefas conforme prioridade gerada                     |
| RF08                                    | RF06 — Detecção de Sobrecarga      | Notificações de pausa acionadas ao detectar carga excessiva                           |

---

## Análise de Consistência

- [x] Notificações são baseadas em comportamento (ex.: longos períodos de atividade)?  
- [ ] Usuário pode configurar frequência e tipo de notificação?  
- [ ] Há personalização de canais (e-mail, Slack, push)?  
- [ ] Sistema previne envio excessivo (limitar número de alertas)?  
- [ ] Há fallback em caso de falha no canal de notificação?  

### Recomendações:

1. Permitir ao usuário definir limites e horários de notificação.  
2. Oferecer seleção de canal preferencial (e-mail, app móvel, Slack).  
3. Implementar lógica anti-spam para não sobrecarregar o colaborador.  
