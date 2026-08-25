# Prompt — Auditoria de Respostas de IA

## Objetivo

Avaliar a confiabilidade de uma resposta produzida por um Large Language Model em um contexto industrial.

O objetivo é identificar alucinações, afirmações sem evidência, inconsistências técnicas e informações que exigem validação humana.

---

## Problema

LLMs podem produzir respostas linguisticamente convincentes mesmo quando:

- não possuem informação suficiente;
- interpretam incorretamente uma fonte;
- combinam informações incompatíveis;
- inventam valores técnicos;
- apresentam hipóteses como fatos.

Em ambientes industriais, esse comportamento pode representar riscos operacionais.

---

## Prompt

> **Papel:** Você é um auditor técnico responsável por avaliar a confiabilidade de uma resposta produzida por um sistema de Inteligência Artificial Generativa.
>
> **Entrada:**
>
> ### Fontes disponíveis
>
> [Inserir documentos utilizados]
>
> ### Resposta gerada pela IA
>
> [Inserir resposta]
>
> ---
>
> **Tarefa:**
>
> Audite a resposta considerando os seguintes critérios:
>
> ### 1. Grounding
>
> Verifique quais afirmações podem ser diretamente sustentadas pelas fontes fornecidas.
>
> ### 2. Informações não suportadas
>
> Identifique afirmações que não possuem evidência suficiente.
>
> ### 3. Alucinações
>
> Procure:
>
> - dados inventados;
> - referências inexistentes;
> - valores técnicos sem fonte;
> - procedimentos não encontrados na documentação;
> - conclusões apresentadas como fatos.
>
> ### 4. Consistência técnica
>
> Verifique se existem contradições entre a resposta e os princípios técnicos presentes nas fontes.
>
> ### 5. Nível de confiança
>
> Classifique cada afirmação como:
>
> - **Alta confiança:** diretamente sustentada pelas fontes.
> - **Média confiança:** interpretação plausível, mas requer confirmação.
> - **Baixa confiança:** hipótese ou informação insuficientemente sustentada.
> - **Não suportada:** não há evidência disponível.
>
> ### 6. Risco operacional
>
> Classifique o potencial risco da informação:
>
> - Baixo
> - Moderado
> - Alto
> - Crítico
>
> ---
>
> **Formato da auditoria:**
>
> | Afirmação | Evidência na fonte | Confiança | Risco | Problema identificado |
> |---|---|---|---|---|
> | Afirmação 1 | Fonte/página | Alta | Baixo | Nenhum |
> | Afirmação 2 | Não encontrada | Baixa | Alto | Sem evidência |
>
> ---
>
> **Conclusão da auditoria**
>
> Responda:
>
> **A resposta pode ser utilizada sem revisão humana?**
>
> **Sim / Não**
>
> Explique o motivo.
>
> Em seguida apresente:
>
> **Principais problemas:**  
> **Informações confiáveis:**  
> **Informações que precisam ser verificadas:**  
> **Riscos identificados:**  
> **Recomendação para o operador humano:**

---

## Conceitos aplicados

- AI auditing
- Grounding
- Hallucination detection
- Uncertainty management
- Human-in-the-Loop
- AI governance
- Industrial safety

---

## Importância para o framework

Este prompt representa uma camada fundamental do framework proposto:

**LLM → Resposta → Auditoria → Validação → Decisão Humana**

A IA não deve ser considerada automaticamente confiável apenas porque apresenta uma resposta coerente.

Em aplicações industriais, a confiabilidade deve ser tratada como uma propriedade verificável do sistema.
