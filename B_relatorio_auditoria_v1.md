# AUDITORIA RIGOROSA – PESQUISA SOBRE A OPERAÇÃO DO SERVIÇO PÚBLICO "SOLICITAÇÃO DE ANÁLISE DE PROJETOS DE NOVOS EDIFÍCIOS PARA HABITE-SE NO DISTRITO FEDERAL (CBMDF)"

## Documento auditado

Pesquisa intitulada *"Service Blueprint AS-IS – Solicitação de Análise de Projetos de Novos Edifícios para Habite-se no Distrito Federal (CBMDF)"*.

---

# RESUMO EXECUTIVO

A pesquisa apresenta uma estrutura coerente de jornada do usuário e Service Blueprint, porém contém diversas falhas relevantes de natureza factual, operacional e normativa.

As principais deficiências identificadas foram:

* Descrição imprecisa do serviço efetivamente prestado pelo CBMDF;
* Inclusão de funcionalidades e integrações sem comprovação documental;
* Omissão de etapas formais previstas na Carta de Serviços;
* Omissão de atores relevantes do fluxo operacional;
* Omissão de documentos obrigatórios;
* Omissão de fail points críticos previstos normativamente;
* Utilização de hipóteses apresentadas como fatos;
* Grau de confiança declarado incompatível com as evidências apresentadas.

## Quadro-síntese dos achados da auditoria v1

| # | Achado | Tipo | Como deveria ser na v2 |
| --- | --- | --- | --- |
| 1 | Descrição imprecisa do serviço ("Análise para Habite-se") | Erro factual | Corrigir para **PSCIP — Análise de Projeto de Segurança Contra Incêndio e Pânico**; Habite-se é consequência posterior, não o objeto. |
| 2 | Formato do projeto informado como **PDF** | Erro factual | Corrigir para **DWF** (arquivo único, limite de 10 MB), conforme a Portaria/Anexo II de Análise Digital. |
| 3 | Integração com **Gov.br** afirmada sem fonte | Inferência não sustentada | Remover ou marcar como hipótese a validar. |
| 4 | Integração automática com **APIs CREA/CAU** | Inferência não comprovada | Remover ou marcar como hipótese a validar. |
| 5 | **Assinador ICP-Brasil / QR Code** como fato | Hipótese como fato | Marcar como [PENDENTE] até validação com a DESEG/DIEAP. |
| 6 | Omissão da etapa formal de **Análise Prévia** (3 dias úteis) | Omissão de etapa | Incluir na jornada, no backstage e na matriz. |
| 7 | Omissão do ator **AGFP** (Agente Fiscalizador de Projetos) | Omissão de ator | Incluir como ator técnico central do exame. |
| 8 | Omissão do **Conselho Técnico** (instância especializada) | Omissão de etapa/ator | Incluir como instância superior (casos omissos, medidas compensatórias). |
| 9 | Omissão de documentos: **TRT, Lista de Verificação do SCIP, memoriais de cálculo** | Omissão documental | Incluir todos como evidências/documentos obrigatórios. |
| 10 | Omissão de normativos: **Portaria de Análise Digital**, competências da DIEAP, NBRs específicas | Omissão normativa | Citar nominalmente os normativos que regem cada etapa. |
| 11 | Prazos oficiais substituídos por estimativas vagas | Imprecisão | Usar os prazos da Carta de Serviços (3, 15, +15, 10, 15 dias úteis; 30 corridos). |
| 12 | Fail point de **cancelamento por reincidência** ausente | Omissão de fail point | Registrar a regra dos dois retornos da mesma exigência. |
| 13 | Grau de confiança superestimado | Inconsistência | Recalibrar separando fato, inferência e hipótese. |

---

# 1. ERROS FACTUAIS

## 1.1 Serviço descrito de forma imprecisa

### Trecho auditado

> "Solicitação de Análise de Projetos de Novos Edifícios para Habite-se"

### Problema

O serviço oficial do CBMDF é a **Análise de Projeto de Segurança Contra Incêndio e Pânico (PSCIP)**.

O Habite-se é consequência administrativa posterior e não o objeto principal do serviço.

### Justificativa

A Carta de Serviços do CBMDF descreve o serviço como PSCIP para fins de Habite-se, Licença de Funcionamento e Regularização.

---

## 1.2 Formato principal dos projetos informado incorretamente

### Trecho auditado

> "upload das pranchas em PDF assinado digitalmente"

### Problema

A documentação oficial estabelece que o projeto deve ser protocolado em formato **DWF**, não PDF.

### Justificativa

A Portaria de Análise Digital exige:

* Arquivo único;
* Extensão .DWF;
* Limite de 10 MB.

---

# 2. INFERÊNCIAS MAL-SUPORTADAS

## 2.1 Integração com Gov.br

### Trecho auditado

> "Login utilizando credenciais cadastradas ou integração com Gov.br"

### Problema

Não foi encontrada evidência normativa ou documental que confirme integração do SCIPWeb com Gov.br.

### Classificação

Inferência não sustentada.

---

## 2.2 Integração automática com CREA/CAU

### Trecho auditado

> "APIs de conselhos de classe (CREA/CAU)"

### Problema

A pesquisa afirma a existência de integrações automáticas sem apresentar qualquer evidência.

### Classificação

Inferência não comprovada.

---

## 2.3 Assinador ICP-Brasil e QR Code

### Trecho auditado

> "QR Code exclusivo de validação"

> "Assinatura ICP-Brasil"

### Problema

A pesquisa apresenta essas funcionalidades como fatos sem indicar documentação oficial que as confirme.

### Classificação

Hipótese apresentada como fato.

---

## 2.4 Armazenamento em nuvem

### Trecho auditado

> "armazenamento em nuvem/servidor"

### Problema

Não há evidência de utilização de infraestrutura em nuvem.

### Classificação

Inferência sem fonte.

---

# 3. ETAPAS DE BASTIDOR (BACKSTAGE) OMITIDAS

## 3.1 Análise Prévia

### Problema

O fluxo oficial prevê etapa formal de Análise Prévia.

### Impacto

Altera significativamente a modelagem do Service Blueprint.

---

## 3.2 Retorno da Análise Prévia

### Problema

A pesquisa ignora o fluxo de retorno ao requerente após a análise prévia.

### Impacto

O ciclo de interação usuário-CBMDF fica incompleto.

---

## 3.3 Atuação do Agente Fiscalizador de Projetos (AGFP)

### Problema

O ator operacional principal não foi identificado.

### Impacto

Perda de precisão na representação do processo.

---

## 3.4 Conselho Técnico

### Problema

O fluxo de recurso e análise especializada foi omitido.

### Impacto

O blueprint não contempla o tratamento formal de divergências técnicas.

---

## 3.5 Fluxo de isenção de taxa

### Problema

A pesquisa não contempla o processo administrativo de análise de isenção.

---

## 3.6 Tratamento de modificações e retificações

### Problema

Projetos de modificação, retificação e digitalização possuem tratamento específico e não aparecem no fluxo.

---

# 4. DOCUMENTOS E EVIDÊNCIAS FÍSICAS OMITIDOS

## 4.1 TRT (Termo de Responsabilidade Técnica)

### Trecho auditado

> "ART/RRT"

### Problema

O TRT não foi incluído.

---

## 4.2 Lista de Verificação do SCIP

### Problema

Não aparece em nenhuma etapa da jornada.

### Impacto

Foi omitida uma das principais evidências digitais utilizadas no serviço.

---

## 4.3 Memoriais de cálculo

### Problema

Não foram considerados.

### Exemplos

* Hidrantes;
* Chuveiros automáticos;
* Escadas pressurizadas.

---

## 4.4 Documentação para isenção

### Problema

Não aparece no levantamento documental.

---

## 4.5 Histórico de processos anteriores

### Problema

Omissão dos documentos necessários para casos de modificação ou retificação.

---

## 4.6 Notas obrigatórias previstas na Portaria

### Problema

A pesquisa não identifica exigências documentais relativas:

* Histórico da edificação;
* Projetos aprovados anteriormente;
* Habite-se anterior;
* Alvarás anteriores.

---

# 5. NORMATIVOS RELEVANTES AUSENTES OU INSUFICIENTES

## 5.1 Conselho Técnico

### Problema

O fluxo normativo de submissão ao Conselho Técnico não foi citado.

---

## 5.2 Portaria de Análise Digital

### Problema

Normativo central para o serviço foi omitido.

---

## 5.3 Procedimentos específicos do SCIP

### Problema

As regras operacionais do sistema não aparecem no levantamento normativo.

---

## 5.4 Competências da DIEAP

### Problema

As atribuições formais da unidade foram pouco exploradas.

---

## 5.5 Referências normativas genéricas

### Trecho auditado

> "ABNT"

### Problema

Norma citada genericamente sem indicar quais NBRs efetivamente impactam a etapa.

---

## 5.6 Regulamento Interno da DESEG

### Trecho auditado

> "Regulamento Interno da DESEG"

### Problema

Normativo citado sem identificação formal.

---

# 6. FAIL POINTS NÃO IDENTIFICADOS

## 6.1 Limite máximo do arquivo DWF

### Problema

Não aparece entre os riscos operacionais.

---

## 6.2 Arquivo em formato incorreto

### Problema

Fail point ausente.

---

## 6.3 Ausência de comprovante de pagamento

### Problema

Fail point não identificado.

---

## 6.4 Ausência de documentos obrigatórios

### Problema

Não aparece como ponto de falha.

---

## 6.5 Não atendimento reiterado das exigências

### Problema

O serviço pode ser cancelado após reincidência.

### Impacto

É um fail point muito mais relevante que o chamado "comunique-se infinito".

---

## 6.6 Classificação incorreta do serviço solicitado

### Problema

Não aparece no levantamento.

---

## 6.7 Pedido de isenção incompleto

### Problema

Não identificado.

---

## 6.8 Erros na justificativa de exigências

### Problema

Não aparece entre os riscos operacionais.

---

## 6.9 Ausência de documentos históricos da edificação

### Problema

Não identificado.

---

# 7. PRAZOS OFICIAIS IGNORADOS

## Trechos auditados

> "dias a semanas"

> "1 a 5 dias úteis"

> "até 48h"

### Problema

A pesquisa substitui prazos normativos por estimativas.

### Prazos previstos oficialmente

| Etapa                  | Prazo            |
| ---------------------- | ---------------- |
| Análise Prévia         | 3 dias úteis     |
| Retorno do interessado | 30 dias corridos |
| Análise do Projeto     | 15 dias úteis    |
| Prorrogação            | +15 dias úteis   |
| Conselho Técnico       | 10 dias úteis    |
| Correção após Conselho | 15 dias úteis    |

---

# 8. PROBLEMAS NO GRAU DE CONFIANÇA DECLARADO

## Trecho auditado

> "Fluxo do SCIPWeb e mecanismos de upload (Alta Confiança)"

### Problema

A própria pesquisa contém diversos elementos incompatíveis com os documentos oficiais.

### Exemplos

* PDF em vez de DWF;
* Gov.br;
* APIs CREA/CAU;
* Prazos divergentes;
* Omissão da análise prévia.

### Conclusão

O grau de confiança declarado é superestimado.

---

# CONCLUSÃO FINAL

A pesquisa apresenta boa estrutura conceitual para um primeiro esboço de Service Blueprint, porém ainda não pode ser considerada uma representação fiel da operação AS-IS do serviço.

As principais limitações são:

1. Omissão de etapas formais previstas na Carta de Serviços;
2. Omissão de atores institucionais relevantes;
3. Falta de aderência à Portaria de Análise Digital;
4. Inclusão de integrações não comprovadas;
5. Fail points insuficientes;
6. Documentação obrigatória incompleta;
7. Uso de hipóteses como fatos;
8. Superestimação do grau de confiança.

Em sua forma atual, o documento é útil como levantamento preliminar, mas exige revisão substancial antes de ser utilizado como base para desenho de processos, Service Blueprint oficial ou iniciativas de transformação de serviços.
