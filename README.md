# Carreira Tech IA

Carreira Tech IA é um GPT multiagente criado para orientar pessoas na escolha e no planejamento de carreira na área de tecnologia.

O projeto funciona como um sistema conversacional que combina entrevista estruturada, análise de perfil e geração de um plano completo de estudos, tudo via chat.

---

## 🎯 Objetivo

Criar um orientador de carreira em tecnologia que:
- Entenda o perfil do usuário por meio de perguntas guiadas
- Sugira carreiras alinhadas a interesses, objetivos e disponibilidade
- Gere um roadmap de estudos claro e acionável
- Utilize arquitetura multiagente com responsabilidades bem definidas

---

## 🧠 Arquitetura Multiagente

O sistema é composto por três partes:

### Orquestrador — Carreira Tech IA
Responsável por:
- Controlar o fluxo da conversa
- Ativar o agente correto
- Tornar explícita a troca de agentes
- Manter contexto entre etapas
- Controlar pesquisa na internet sob demanda

### Agent Alpha — Entrevista e Diagnóstico
- Conduz entrevista estruturada de 7 perguntas
- Analisa perfil e objetivos
- Sugere 3 carreiras ranqueadas
- Transfere dados para o Agent Beta

### Agent Beta — Planejamento e Roadmap
- Recebe os dados do Agent Alpha
- Gera plano completo de estudos
- Cria roadmap de 90 dias
- Sugere projeto de portfólio
- Prepara roteiro de entrevistas
- Indica trilha DIO

---

## 🔄 Fluxo de Funcionamento

1. Início com Agent Alpha  
2. Entrevista (7 perguntas, uma por vez)  
3. Sugestão de 3 carreiras  
4. Escolha do usuário  
5. Troca explícita para Agent Beta  
6. Geração do plano completo  
7. Ajustes ou retorno ao diagnóstico  

---

## 🌐 Pesquisa na Internet

O GPT não pesquisa a internet por padrão.

A pesquisa só ocorre quando:
- O usuário faz uma pergunta que depende de dados atualizados
- O GPT pede confirmação explícita antes de consultar a web

---

## 📁 Estrutura do Repositório

carreira-tech-ia/
├── README.md
├── prompts/
│ ├── orquestrador.md
│ ├── agent-alpha.md
│ └── agent-beta.md
├── docs/
│ ├── arquitetura.md
│ └── fluxo.md
└── exemplos/
└── conversa-exemplo.md

yaml
Copiar código

---

## 🚀 Como Reproduzir

1. Criar um GPT personalizado no ChatGPT  
2. Colar o prompt do arquivo `prompts/orquestrador.md`  
3. Ativar navegação na web (opcional)  
4. Testar o fluxo completo  

---

## 🏁 Status

✅ Projeto finalizado

Criado por **Jaime**
📄 prompts/orquestrador.md
md
Copiar código
# Carreira Tech IA — Prompt Orquestrador

Este arquivo contém o prompt principal do GPT Carreira Tech IA.

Ele define:
- Regras de orquestração
- Troca explícita de agentes
- Separação de responsabilidades
- Uso de pesquisa na internet sob demanda

[COLE AQUI O PROMPT ÚNICO FINAL DO GPT]
📄 prompts/agent-alpha.md
md
Copiar código
# Agent Alpha — Entrevista e Diagnóstico de Carreira

[COLE AQUI O PROMPT 1 INTEGRAL]
📄 prompts/agent-beta.md
md
Copiar código
# Agent Beta — Planejamento e Roadmap de Carreira

[COLE AQUI O PROMPT 2 INTEGRAL]
📄 docs/arquitetura.md
md
Copiar código
# Arquitetura do Carreira Tech IA

O Carreira Tech IA é um sistema conversacional multiagente composto por:

- Um orquestrador central
- Dois agentes especializados
- Regras rígidas de separação de responsabilidades

O orquestrador controla o estado da conversa e define qual agente está ativo em cada momento.
📄 docs/fluxo.md
md
Copiar código
# Fluxo do GPT

1. GPT inicia com Agent Alpha
2. Entrevista estruturada em 7 perguntas
3. Análise e sugestão de carreiras
4. Escolha do usuário
5. Troca explícita para Agent Beta
6. Geração do plano completo
7. Possibilidade de ajustes ou retorno ao diagnóstico
📄 exemplos/conversa-exemplo.md
md
Copiar código
# Exemplo de Conversa

Usuário: Quero orientação de carreira em tecnologia.

Agent Alpha:
Pergunta 1: O que mais te atrai em tecnologia?

[...]

Agent Alpha:
Sugestão de carreiras

Usuário:
Escolho a carreira X

Agent Beta:
Geração do plano completo de estudos
