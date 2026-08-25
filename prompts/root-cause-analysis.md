# Prompt — Análise de Causa Raiz Industrial

## Objetivo

Utilizar IA Generativa para estruturar uma investigação de causa raiz em processos industriais, relacionando variáveis de processo, defeitos e possíveis mecanismos físicos.

O modelo deve atuar como ferramenta de apoio à investigação, e não como autoridade definitiva sobre a causa do problema.

---

## Cenário

Foi identificado um defeito em um processo de usinagem.

### Defeito observado

Microfissuras em uma superfície usinada.

### Variáveis disponíveis

- Temperatura do processo
- Velocidade de corte
- Rotação do spindle
- Desgaste da ferramenta
- Tempo de operação
- Histórico de lotes
- Registros de manutenção

---

## Prompt

> **Papel:** Você é um especialista em análise de causa raiz, controle de qualidade e engenharia de processos.
>
> **Objetivo:** Investigar possíveis causas de um defeito industrial utilizando as evidências disponíveis na base de conhecimento.
>
> **Etapa 1 — Definição do problema**
>
> Descreva claramente:
>
> - qual é o defeito;
> - onde ocorre;
> - quando ocorre;
> - qual processo está associado;
> - quais variáveis podem estar relacionadas.
>
> **Etapa 2 — Levantamento de hipóteses**
>
> Gere hipóteses de causa raiz utilizando:
>
> - evidências encontradas nas fontes;
> - relações entre variáveis;
> - princípios de engenharia;
> - histórico de ocorrências semelhantes.
>
> **Etapa 3 — Relação causal**
>
> Para cada hipótese, explique:
>
> `Variável → mecanismo físico → consequência → defeito`
>
> **Etapa 4 — Evidências**
>
> Para cada hipótese, indique:
>
> - evidências favoráveis;
> - evidências contrárias;
> - informações ausentes;
> - nível de confiança.
>
> **Etapa 5 — Investigação**
>
> Sugira quais medições, inspeções ou experimentos poderiam confirmar ou descartar cada hipótese.
>
> **Regras:**
>
> - Não apresente uma hipótese como fato.
> - Não invente dados.
> - Diferencie evidência de inferência.
> - Informe quando a base de conhecimento não possuir dados suficientes.
> - Priorize explicações fisicamente plausíveis.
> - Recomendações envolvendo intervenção física devem ser submetidas à validação de um profissional qualificado.
>
> **Formato final:**
>
> | Hipótese | Evidências | Evidências contrárias | Confiança | Teste de confirmação |
> |---|---|---|---|---|
> | Causa 1 | ... | ... | Alta/Média/Baixa | ... |
> | Causa 2 | ... | ... | Alta/Média/Baixa | ... |
>
> Finalize com:
>
> **Causa mais provável:**  
> **Evidência principal:**  
> **Incertezas:**  
> **Próximo passo recomendado:**  
> **Validação humana necessária:**

---

## Conceitos aplicados

- Root Cause Analysis
- Causal reasoning
- Quality Engineering
- Process monitoring
- Knowledge Graphs
- Human-in-the-Loop
- Uncertainty Management

---

## Valor profissional

O diferencial deste prompt é que ele não solicita simplesmente que a IA "descubra a causa".

Ele estrutura o raciocínio investigativo em uma sequência:

**Problema → Hipóteses → Evidências → Relações causais → Testes → Validação**

Essa abordagem reduz o risco de transformar uma resposta probabilística do LLM em uma falsa conclusão técnica.
