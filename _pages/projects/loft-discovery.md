---
title: "Case: Product Discovery – Loft"
layout: single
permalink: /projects/loft-discovery/
author_profile: true
---
# Case: Product Discovery – Loft

Este case documenta um processo de Product Discovery conduzido para aumentar a conversão de agendamentos de visita em anúncios de imóveis da Loft. A narrativa foca em decisões, trade‑offs e impacto — seguindo o padrão: Contexto → Problema → Objetivos & Métricas → Requisitos → Decisões & Trade‑offs → Execução → Resultados & Aprendizados.

---

## Contexto do sistema

- Produto: plataforma de anúncios imobiliários com alto tráfego de usuários interessados em compra/visita.  
- Stakeholders: growth, produto, engenharia frontend/back-end, UX, operações de atendimento e times comerciais.  
- Escala e constraints: grande volume de listagens com variação substancial de qualidade de conteúdo (fotos, descrição) e integração com calendários/contato via WhatsApp.

## Problema (cliente, negócio, técnico)

- Cliente: muitos usuários encontram anúncios mas desistem antes de agendar visita — perda de funnel no ponto de conversão.  
- Negócio: baixa taxa de agendamento reduz receita de transação e limita indicadores de aquisição/engajamento.  
- Técnico: processo de agendamento fragmentado e pouca instrumentação para medir pontos de queda; inconsistência de conteúdo por listagem.

## Objetivos e métricas de sucesso

- Objetivo primário: aumentar a taxa de agendamento de visita (visita agendada / visitas à página do anúncio).  
- Métricas principais: taxa de conversão para agendamento, taxa de clique no CTA (agendar/WhatsApp), lift em testes A/B, taxa de sucesso de agendamento (completo vs. abandonado).  
- Guardrails: não reduzir a qualidade da experiência; manter latência de página e SLA de integrações dentro de limites operacionais.

## Requisitos funcionais e não funcionais

- Requisitos funcionais: simplificar fluxo de agendamento, incluir CTA direto (ex.: WhatsApp), melhorar copy e imagens em listagens prioritárias; instrumentar eventos para cada etapa do fluxo.  
- Requisitos não funcionais: testes A/B com segmentação, sistema de monitoração de erros e alertas, suporte a alta concorrência em integrações de contato.

## Decisões e trade‑offs

1. Priorizar experimentos incrementais (A/B) antes de uma reescrita completa do fluxo: menor custo inicial e aprendizado rápido vs. possibilidade de ganhos maiores com reformulação.  
2. Implementar CTA via WhatsApp como experiência de baixo atrito — trade‑off: menor controle de dados no início vs. potencial de aumentar conversão rapidamente.  
3. Investir em testes de conteúdo (descrição/fotos) em listagens de maior tráfego antes de globalizar mudanças — trade‑off entre rapidez no experimento e representatividade estatística.  
4. Adotar testes de formulário simplificado com métricas definidas (conversão, abandono, qualidade do lead) e rollback criteria claros em caso de queda de qualidade de lead.

Cada decisão foi documentada em specs que listavam cenário, hipóteses, métricas de sucesso, critérios de parada e plano de rollout incremental.

## Execução (papel do PM e uso de specs)

- Papel do PM: liderar descoberta (entrevistas e análise quantitativa), definir hipóteses e priorização, escrever specs e critérios de aceitação, coordenar com engenheiros e UX, definir metodologia de A/B e plan de rollout.  
- Uso de specs: documentos curtos (Contexto → Hipótese → Métricas → Critérios de sucesso → Plano de rollout) serviram como contrato entre produto e engenharia, reduzindo ambiguidade e acelerando implementação de experimentos.  
- Instrumentação e medição: eventos de funnel e monitoramento foram implementados para identificar abandono em cada etapa e permitir decisão baseada em dados em tempo real.

## Resultado, impacto e aprendizados

- Resultado experimental: os experimentos de copy e simplificação de formulário mostraram lift positivo em conversão nos segmentos testados (detalhes numéricos a serem inseridos conforme dados de análise).  
- Impacto operacional: introdução de CTA via WhatsApp permitiu testar alternativas de contato com baixo custo de desenvolvimento; exigiu acompanhamento de qualidade de lead.  
- Aprendizados principais:  
	- Priorizar experimentos de menor custo que possibilitem aprendizado rápido e validação de hipóteses.  
	- Instrumentação antecipada é crítica para interpretar resultados e evitar decisões precipitadas.  
	- Especificações curtas e orientadas a métricas facilitam alinhamento cross‑functional e reduzem retrabalho.

---

### Próximos passos recomendados

1. Consolidar métricas e publicar dashboard com os resultados por experimento (incluir lift, p-value e tamanho do efeito).  
2. Automatizar rollback e monitoramento de qualidade de lead para CTAs externos (WhatsApp).  
3. Expandir experimentos bem‑sucedidos de listagens de alto tráfego para mais segmentos, mantendo critérios de segurança operacional.

---

_Nota:_ se quiser, eu insiro os números reais de lift e estatísticas dos testes (se disponíveis) e adiciono gráficos/visualizações para evidenciar impacto em linha com o posicionamento do portfólio.
