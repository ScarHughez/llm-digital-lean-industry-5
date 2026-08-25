# Limitações, Riscos e "Cicatrizes"

## 1. Alucinações

LLMs podem produzir informações tecnicamente plausíveis, mas incorretas.

Em ambientes industriais, esse comportamento representa um risco significativo.

Uma resposta não deve ser considerada válida apenas porque parece coerente.

---

## 2. Raciocínio espacial

Modelos de linguagem podem apresentar limitações em tarefas envolvendo:

- geometria;
- cinemática;
- montagem;
- tolerâncias;
- interferências;
- relações espaciais tridimensionais.

Isso limita a utilização de LLMs isolados para projetos mecânicos críticos.

---

## 3. Mismatch semântico-estrutural

LLMs trabalham principalmente com representações probabilísticas e linguagem.

Sistemas industriais trabalham com requisitos determinísticos.

Essa diferença cria um problema importante:

> Uma resposta linguisticamente correta pode não ser fisicamente executável.

Por isso, recomendações geradas por IA precisam passar por validação adequada antes de qualquer execução.

---

## 4. Model Collapse

A utilização de dados sintéticos gerados por IA pode introduzir riscos quando esses dados são utilizados recursivamente para treinar novos modelos.

A perda progressiva de diversidade e fidelidade dos dados pode comprometer a qualidade dos modelos.

Em aplicações industriais, dados reais continuam sendo fundamentais.

---

## 5. Propriedade intelectual

Ambientes industriais possuem informações potencialmente sensíveis:

- projetos;
- processos;
- patentes;
- parâmetros;
- documentação;
- códigos;
- dados de produção.

O envio dessas informações para serviços externos de IA pode gerar riscos relacionados à propriedade intelectual e governança de dados.

---

## 6. Segurança

Uma IA generativa não deve ser considerada automaticamente um sistema de segurança.

Recomendações relacionadas a:

- máquinas;
- robôs;
- CNC;
- CLPs;
- manutenção;
- energia;
- processos críticos

devem permanecer submetidas aos mecanismos formais de segurança e validação da organização.

---

## 7. Dependência das fontes

Sistemas RAG melhoram o acesso ao conhecimento, mas não corrigem automaticamente:

- documentos incorretos;
- informações desatualizadas;
- dados incompletos;
- conflitos entre documentos.

A qualidade da resposta continua dependente da qualidade da base de conhecimento.

---

## 8. Limitações da pesquisa

Este projeto apresenta uma investigação conceitual e exploratória.

O framework proposto não representa uma implementação industrial validada em ambiente de produção.

Portanto, não devem ser interpretados como resultados de desempenho industrial real os benefícios potenciais discutidos na pesquisa.

---

## 9. Principal aprendizado

Uma das principais "cicatrizes" do projeto foi perceber que utilizar IA não significa simplesmente fazer perguntas melhores.

Em aplicações industriais, é necessário construir um sistema no qual a resposta possa ser:

1. contextualizada;
2. fundamentada;
3. auditada;
4. validada;
5. rejeitada quando necessário.

Essa conclusão levou à proposta de uma arquitetura baseada em inteligência híbrida e supervisão humana.
