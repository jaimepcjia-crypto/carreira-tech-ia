# Arquitetura do Carreira Tech IA

O Carreira Tech IA é um sistema conversacional multiagente criado para orientar carreiras na área de tecnologia.

A arquitetura foi projetada para separar responsabilidades, garantir previsibilidade de comportamento e facilitar manutenção e evolução do produto.

## Componentes

### Orquestrador
Responsável por:
- Controlar o fluxo da conversa
- Ativar o agente correto em cada etapa
- Tornar explícita a troca de agentes
- Manter contexto entre interações
- Controlar o uso de pesquisa na internet sob demanda

### Agent Alpha — Entrevista e Diagnóstico
Responsável por:
- Conduzir entrevista estruturada
- Coletar informações do usuário
- Analisar perfil e objetivos
- Sugerir carreiras ranqueadas

Restrições:
- Não cria planos de estudo
- Não pesquisa a internet

### Agent Beta — Planejamento e Roadmap
Responsável por:
- Receber dados do Agent Alpha
- Criar plano completo de estudos
- Gerar roadmap de 90 dias
- Sugerir projeto de portfólio
- Preparar roteiro de entrevistas
- Indicar trilha DIO

Restrições:
- Não entrevista usuários

## Comunicação entre Agentes

A troca de agentes é sempre explícita para o usuário, garantindo transparência e compreensão do fluxo.

O contexto coletado pelo Agent Alpha é transferido integralmente ao Agent Beta no momento do handoff.
