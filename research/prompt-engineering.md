# Engenharia de Prompts

## 1. Objetivo

Uma das etapas do projeto foi investigar como a estrutura dos prompts influencia a qualidade e a confiabilidade das respostas produzidas por modelos de linguagem.

A estratégia adotada foi evoluir de perguntas genéricas para prompts estruturados com:

- papel;
- contexto;
- objetivo;
- restrições;
- fontes;
- critérios de validação;
- tratamento de incerteza;
- supervisão humana.

---

## 2. Prompt inicial

### Prompt

> Explique como a Inteligência Artificial pode melhorar o processo produtivo de uma fábrica.

### Características

O prompt apresenta uma pergunta ampla e pouco restritiva.

### Limitações observadas

Esse tipo de consulta pode produzir respostas:

- genéricas;
- pouco contextualizadas;
- excessivamente otimistas;
- sem referências específicas;
- sem consideração das restrições físicas do ambiente industrial.

---

## 3. Prompt intermediário — RAG

### Prompt

> Com base estritamente no manual de manutenção do compressor X e no histórico de ordens de serviço indexados na base RAG, identifique as três causas prováveis para o aumento de temperatura registrado pelo sensor IoT e sugira o procedimento de reparo correto.

### Evolução

O prompt passou a:

- restringir as fontes;
- especificar o equipamento;
- utilizar dados históricos;
- solicitar causas prováveis;
- exigir relação com procedimentos existentes.

### Benefício

A utilização de RAG permite ancorar a resposta em informações externas específicas, reduzindo a dependência do conhecimento geral do modelo.

---

## 4. Prompt avançado — restrições de engenharia

### Prompt

> Você é um Agente de Design para Manufaturabilidade (DfM) operando sob as restrições da Indústria 5.0.
>
> Desenvolva um script OpenSCAD paramétrico para um suporte de dispositivo eletrônico industrial.
>
> O projeto deve considerar:
>
> 1. Inclinação de 60 graus.
> 2. Canal para passagem de cabo.
> 3. Folga vertical de 15 mm.
> 4. Redução do volume de material.
> 5. Sustentabilidade.
> 6. Ergonomia do operador.
>
> Não gere o código antes de verificar as restrições geométricas e de montagem.

### Evolução

O prompt incorpora:

- papel especializado;
- contexto industrial;
- requisitos funcionais;
- requisitos ergonômicos;
- sustentabilidade;
- restrições geométricas.

---

## 5. Princípios identificados

A evolução dos prompts demonstrou que respostas mais úteis podem ser obtidas quando o prompt especifica claramente:

### Contexto

Qual é o ambiente em que a IA está operando?

### Papel

Qual especialista a IA deve simular?

### Dados

Quais informações devem ser consideradas?

### Restrições

Quais condições não podem ser violadas?

### Evidências

Quais fontes sustentam a resposta?

### Incerteza

O que deve acontecer quando os dados forem insuficientes?

### Validação

Quem deve verificar a recomendação?

---

## 6. Resultado

A engenharia de prompts passou a ser tratada como uma camada de controle da interação entre o usuário e o modelo.

Em aplicações industriais, um prompt bem estruturado não substitui sistemas de segurança ou validação técnica, mas pode reduzir ambiguidades e tornar as respostas mais auditáveis.
