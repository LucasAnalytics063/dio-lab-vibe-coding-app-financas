# App de Finanças Pessoais - Prototipagem Conversacional com IA

> Conceito de produto financeiro construído com Vibe Coding: da ideia ao MVP funcional usando IA como parceira de desenvolvimento.

## Visão Geral

A maioria dos aplicativos de controle financeiro falha pelo mesmo motivo: atrito excessivo na entrada de dados. O usuário abandona antes de criar o hábito.

Este projeto explora uma abordagem diferente **controle financeiro por conversação** onde o usuário interage com um agente de IA em linguagem natural, sem formulários, sem categorias manuais, sem fricção.

O desenvolvimento foi conduzido integralmente via **Vibe Coding**: uma metodologia de prototipagem onde a comunicação estruturada com a IA substitui a escrita linha a linha de código. O resultado é um MVP funcional, validável e extensível produzido sem um ciclo tradicional de engenharia.

## O Problema

Aplicativos financeiros convencionais exigem disciplina antes de entregar valor. O usuário precisa categorizar, orçar e configurar antes de ver qualquer resultado o que gera abandono precoce, especialmente em perfis iniciantes.

A hipótese central deste projeto: **se o registro financeiro acontecer dentro de uma conversa, a barreira de entrada cai e o engajamento sobe.**


## Metodologia — Vibe Coding

Vibe Coding não é sobre escrever menos código. É sobre **deslocar o esforço cognitivo da sintaxe para a estratégia**.

Na prática, isso significa:
- Definir o problema com precisão antes de qualquer prompt
- Estruturar a comunicação com a IA como um briefing técnico, não como um pedido casual
- Iterar sobre outputs com critérios claros de aceitação
- Tratar a IA como um membro sênior do time — ela executa melhor quando recebe contexto, não apenas comandos

> A qualidade do output é função direta da qualidade do input. Prompts vagos geram protótipos vagos.

## Etapas de Desenvolvimento

### 1. Engenharia de Prompt e PRD

Antes de qualquer geração de interface, o esforço foi concentrado na construção de um **PRD (Product Requirements Document)** via IA definindo escopo, persona, fluxo conversacional e critérios de MVP.

Os prompts utilizados nessa fase estabeleceram:
- Comportamento e tom de voz do agente financeiro
- Funcionalidades prioritárias do MVP
- Restrições de escopo para evitar bloat

*Prints do processo de engenharia de prompt:*

<img width="537" height="562" alt="Prompt - Fase 1" src="https://github.com/user-attachments/assets/f70ad15b-8f70-42ec-9e97-e8d6efc06300" />
<img width="533" height="573" alt="Prompt - Fase 2" src="https://github.com/user-attachments/assets/f98649f0-13a7-45c5-bca1-e47cb2a033f9" />
<img width="535" height="380" alt="Prompt - Fase 3" src="https://github.com/user-attachments/assets/6c1a4742-fdcb-4435-9803-c4ae5800a7b7" />

### 2. Prototipagem no Lovable

Com o PRD validado, a geração do MVP foi executada no **Lovable**, priorizando três entregas:

**Agente Financeiro**  Definição de comportamento, tom e intenções suportadas pelo assistente conversacional

**Fluxo de Telas**  Arquitetura de navegação gerada a partir das funcionalidades do PRD, simulando interação real por conversa

**Plano de MVP**  5 funcionalidades centrais, recursos necessários e métricas de validação inicial

> Restrição operacional: o plano gratuito do Lovable limita a 5 interações diárias — o que forçou precisão nas instruções e eliminou desperdício de iterações.


### 3. Análise Crítica do MVP

*Tela Home do aplicativo gerado:*

![Home](https://github.com/user-attachments/assets/f2611cb9-5778-4146-a54a-d87f5201b375)

**Arquitetura da interface:**
- Header com identificação do assistente e saldo mensal consolidado
- Área central de chat como ponto de entrada único
- Ações rápidas: registrar gasto, registrar receita, metas, resumo mensal
- Navegação inferior: Chat / Metas / Relatórios / Ajustes

**O que funcionou:**
- Interface com baixo ruído visual — curva de aprendizado mínima
- Paleta coerente com o domínio financeiro
- Hierarquia de ações bem definida — o usuário sabe o que fazer sem instrução

**O que não funcionou e por quê:**
- Chat iniciando vazio transmite inatividade — a ausência de uma mensagem de boas-vindas do agente quebra o contrato conversacional esperado pelo usuário
- Distância entre botões de ação e campo de input reduz fluidez — a interação deveria ser contínua, não fragmentada
- O agente não interpretou intenções relacionadas a metas — limitação de escopo do treinamento, não da interface

## Aprendizados Técnicos

|               Decisão                  |             Resultado               |                      Ajuste Identificado                       |
|----------------------------------------|-------------------------------------|----------------------------------------------------------------|
| PRD antes do protótipo                 | Reduziu retrabalho e manteve escopo | Adicionar critérios de aceitação por funcionalidade            |
| Prompts descritivos e contextualizados | Outputs mais alinhados ao produto   | Incluir restrições explícitas para evitar features fora do MVP |
| Lovable como motor de geração          | MVP funcional em poucas iterações   | Mapear intenções do agente antes da geração de interface       |


## Acesso ao Protótipo

[**Acessar MVP — FinSpeak Flow**](https://fin-speak-flow.lovable.app)


## Conclusão

O projeto validou a hipótese central: é possível construir um assistente financeiro funcional e com baixo atrito usando prototipagem conversacional com IA. O MVP entrega o fluxo essencial registro e acompanhamento — com uma interface que não intimida o usuário iniciante.

Os gaps identificados mensagem inicial do agente, proximidade das ações, suporte a intenções de metas são ajustes de produto, não limitações estruturais. A base está sólida para uma segunda iteração com escopo expandido e agente mais robusto.

O maior aprendizado do processo não foi técnico: foi constatar que **a disciplina na construção do prompt é o equivalente ao design de arquitetura no desenvolvimento tradicional**. Quem domina essa etapa entrega produtos melhores, mais rápido.

## Autor
**Lucas Beserra Ribeiro** 
Analista de Business Intelligence | Sicoob Tocantins 
[GitHub: LucasAnalytics063](https://github.com/LucasAnalytics063)

## Licença

MIT — Uso, fork e adaptação livres. Créditos são apreciados.
