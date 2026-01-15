---
title: "Cultura de Qualidade e Testes"
permalink: /cases/quality-culture/
layout: single
---

# Cultura de Qualidade e Testes

**De dependência de QA a autonomia das squads**

## Contexto

Squads dependiam de ciclos longos de testes manuais, QA era gargalo operacional e bugs chegavam à produção com frequência. Não havia cultura de testes — código era entregue "pronto", validação era tarefa de terceiros. Resultado: tempo longo de ciclo, falta de propriedade dos times e qualidade reativa.

## Problema

- Testes tardios (após desenvolvimento concluído)
- Dependência de equipe central de QA
- Baixa cobertura de testes automáticos
- Cultura de "QA valida, dev entrega" — sem propriedade compartilhada
- Bugs recorrentes em produção

## Decisão de Produto

Transformar qualidade de burocracia central em responsabilidade compartilhada das squads, via mudança cultural sistemática: **shift-left testing, empoderamento de desenvolvedores, e alinhamento entre planejamento e qualidade**.

## Abordagem

- **Planejamento incluindo testes desde o início** — user stories com critérios de aceita explícitos e exemplos de testes
- **TDD como prática aliada** — não obrigatório, mas incentivado e facilitado com workshops
- **Shift-left testing** — testes unitários e integrados por feature, antes de QA centralizado
- **Code review como mecanismo de visão independente** — padronização de boas práticas e detecção de falhas
- **Empoderamento de desenvolvedores** — investimento em ferramentas, capacitação e autonomia

## Métricas Usadas

- Cobertura de testes por feature (% linha)
- Taxa de bugs em novas funcionalidades (bugs/1k LOC)
- Tempo médio de resolução de bugs críticos em produção (horas)
- Adoção de TDD pelos times (% features com testes desde o início)

## Impacto Sistêmico

- Redução de bugs críticos em 65%
- Cobertura de testes aumentada de 30% para 85%
- Squads com autonomia de validação (redução de 3 semanas de ciclo)
- Cultura de propriedade compartilhada consolidada

## Resultado-chave

Qualidade deixou de ser responsabilidade de QA centralizado e virou capacidade distribuída das squads. Squads passaram de reativas (corrigir bugs) a preventivas (estruturar qualidade no design). Impacto direto: ciclos mais curtos, confiança maior e menos rework em produção.
