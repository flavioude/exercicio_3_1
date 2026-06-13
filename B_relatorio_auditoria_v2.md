# SEGUNDA AUDITORIA RIGOROSA – PESQUISA SERVICE BLUEPRINT AS-IS V2.0

## Serviço auditado

**Análise de Projeto de Segurança Contra Incêndio e Pânico (PSCIP) para fins de Habite-se, Licenciamento e Regularização no Distrito Federal — CBMDF/DESEG/DIEAP.**

## Objetivo da segunda auditoria

Verificar:

1. se cada falha apontada na auditoria anterior foi de fato endereçada na V2;
2. se a V2 introduziu novas falhas;
3. se ainda restam pontos abertos relevantes.

## Fontes de referência utilizadas

- Pesquisa V2 enviada pelo usuário: `pesquisa_service_blueprint_final_v2.md`.
- Carta de Serviços do CBMDF — Análise de Projeto de Segurança Contra Incêndio e Pânico (PSCIP).
- IN nº 01/2021-DESEG/CBMDF — Procedimentos Normativos para Prestação de Serviços de Segurança Contra Incêndio e Pânico.
- Anexo II da IN nº 01/2021-DESEG/CBMDF — Requisitos de apresentação de projeto em formato eletrônico.

---

# 1. Síntese executiva

A V2 corrige parte significativa das falhas da versão anterior. Houve melhora real nos seguintes pontos:

- correção do nome do serviço para PSCIP;
- inclusão do formato DWF;
- inclusão do limite de 10 MB;
- retirada da afirmação de login via Gov.br;
- retirada da afirmação de APIs CREA/CAU;
- inclusão de ART/RRT/TRT;
- inclusão da Análise Prévia;
- inclusão do AGFP;
- inclusão do Conselho Técnico;
- inclusão de prazos oficiais;
- inclusão de Lista de Verificação;
- inclusão de fail points documentais e técnicos.

Apesar disso, a V2 ainda **não pode ser considerada plenamente confiável** como representação AS-IS. Ela continua misturando informações oficiais, inferências plausíveis e suposições operacionais não comprovadas. Além disso, introduz novas falhas, especialmente ao transformar hipóteses técnicas de sistema em fatos, citar normas de forma inadequada e descrever o Conselho Técnico como se fosse uma instância recursal ordinária da DIEAP.

## Quadro-síntese dos pontos ainda abertos na v2 (a corrigir na v3)

| # | Achado residual da v2 | Categoria | Correção exigida para a v3 |
| --- | --- | --- | --- |
| 1 | Sistemas não comprovados: **DESEGWEB, módulo de triagem, módulo de recursos, visualizador DWF integrado, assinador ICP-Brasil, emissor de QR Code** | Validação de sistemas | Marcar todos como **[PENDENTE]** até validação com a TI/DESEG; não tratar como fato. |
| 2 | Base normativa: **Decreto nº 42.502/2021** tratado como regulamento do RSIP-DF sem demonstrar a relação | Correção normativa | Referenciar o **Decreto nº 21.361/2000** (RSIP-DF citado pela IN nº 01/2021) ou justificar o dispositivo do 42.502/2021. |
| 3 | **CTDSCI** descrito como "Conselho Técnico da DIEAP" / instância recursal ordinária | Correção institucional | Reescrever como Conselho Técnico do DSCI, instância superior para casos omissos, medidas compensatórias e dispensa de exigências. |
| 4 | **DIEAP** grafada como "Divisão de Exame e Aprovação de Projetos" | Erro factual | Corrigir para **Diretoria de Estudos e Análise de Projetos**. |
| 5 | Documentos e fail points não estruturados **por modalidade** de PSCIP | Detalhamento | Distinguir obra inicial, existente, modificação, bem tombado, área não regularizada, retificação, cópia digital. |
| 6 | Fronteira com a **vistoria para Habite-se** mal delimitada | Delimitação de escopo | Inserir seção "Fronteira do serviço": PSCIP encerra no parecer; vistoria (DIVIS) é handoff posterior. |
| 7 | Prazo da Análise Prévia classificado como **"improrrogável/taxativo"** | Excesso interpretativo | Remover a qualificação jurídica não comprovada; manter apenas "3 dias úteis". |
| 8 | Regra de cancelamento genérica ("não atendimento reiterado") | Imprecisão | Registrar a **regra dos dois retornos** da mesma exigência. |
| 9 | Regra dos **10 MB** apresentada como rígida | Imprecisão | Admitir subdivisão do DWF quando exceder o limite, conforme o Anexo II. |

---

# 2. Verificação das falhas do audit_v1

## 2.1 Serviço descrito de forma imprecisa

### Status

**Endereçado.**

### Trecho da V2

> “Serviço: Análise de Projeto de Segurança Contra Incêndio e Pânico (PSCIP) para fins de Habite-se, Licenciamento e Regularização no Distrito Federal.”

### Avaliação

A V2 corrige adequadamente a denominação do serviço e abandona a formulação anterior excessivamente centrada em “novos edifícios para Habite-se”.

### Ponto residual

Ainda há momentos em que a conclusão do serviço é redigida como se “liberasse a emissão do Habite-se” de forma direta, quando a aprovação do PSCIP é etapa anterior e não substitui a vistoria ou os demais atos administrativos.

---

## 2.2 Erro sobre formato dos arquivos

### Status

**Endereçado parcialmente.**

### Trecho da V2

> “Arquivo único em formato DWF (limite estrito de 10 MB).”

### Avaliação

A V2 corrigiu a falha principal: o projeto deixa de ser tratado como PDF e passa a ser corretamente tratado como DWF.

### Falha residual

A V2 afirma “limite estrito de 10 MB” de forma absoluta. O Anexo II estabelece que o arquivo deve ser único até o limite de 10 MB, mas também prevê subdivisão em dois ou mais arquivos quando a quantidade de folhas acarretar tamanho superior a 10 MB. Portanto, o texto está rígido demais.

### Correção recomendada

Substituir por:

> “As pranchas devem ser apresentadas em arquivo DWF único sempre que possível, respeitado o limite de 10 MB; caso a quantidade de folhas gere arquivo superior a esse limite, admite-se subdivisão conforme o Anexo II da IN nº 01/2021-DESEG/CBMDF.”

---

## 2.3 Integração Gov.br afirmada sem base

### Status

**Endereçado.**

### Avaliação

A V2 removeu a afirmação de integração com Gov.br e passou a falar em “credenciais locais”.

### Ponto aberto

Permanece pendente a validação do fluxo real de cadastro e homologação de perfis no SCIPWeb, que a própria V2 marcou corretamente como lacuna.

---

## 2.4 APIs CREA/CAU inventadas ou não sustentadas

### Status

**Endereçado.**

### Avaliação

A V2 removeu a afirmação de integração automática com CREA/CAU.

### Ponto aberto

A V2 ainda menciona “carteira do conselho de classe” como documento anexado no cadastro, mas isso deveria ser validado operacionalmente. A fonte oficial enfatiza ART/RRT/TRT e documentos do processo, não necessariamente carteira profissional como anexo obrigatório em todas as situações.

---

## 2.5 Omissão do TRT/CRT

### Status

**Endereçado.**

### Trecho da V2

> “ART/CREA, RRT/CAU ou TRT/CFT.”

### Avaliação

A V2 incorporou corretamente o TRT/CFT.

---

## 2.6 Omissão da Análise Prévia

### Status

**Endereçado.**

### Trecho da V2

> “Análise Prévia (3 dias úteis).”

### Avaliação

A etapa foi inserida na jornada, no backstage e na matriz do blueprint.

### Ponto de atenção

A V2 chama a Análise Prévia de “prazo legal improrrogável” e “taxativo”. Essa qualificação é mais forte do que a fonte oficial normalmente permite concluir. O documento oficial informa prazo de 3 dias úteis; a caracterização como “improrrogável” ou “taxativo” deveria ser removida, salvo fonte específica.

---

## 2.7 Omissão do AGFP

### Status

**Endereçado.**

### Trecho da V2

> “Agente Fiscalizador de Projetos (AGFP).”

### Avaliação

A V2 passou a identificar corretamente o ator técnico central.

### Falha nova relacionada

Na matriz, aparece “AGPFs”, com inversão da sigla. Isso não é apenas cosmético se o documento for usado institucionalmente, porque introduz inconsistência terminológica em ator formal do processo.

---

## 2.8 Prazos oficiais substituídos por estimativas vagas

### Status

**Endereçado em grande parte.**

### Trecho da V2

> “3 dias úteis”, “15 dias úteis”, “30 dias corridos”, “10 dias úteis”, “15 dias úteis se pós-Conselho”.

### Avaliação

A V2 incorporou os prazos centrais da Carta de Serviços.

### Falhas residuais

A V2 ainda deixa “Tempo de Espera: variável” no protocolo e “imediato após assinatura” na emissão final. Isso é aceitável como hipótese, mas deveria ser marcado como pendente quando não houver dado real do sistema.

Também faltou distinguir claramente o prazo de retorno para saneamento documental, valor de taxa ou cumprimento de exigência, que é tratado de modo mais amplo na Carta de Serviços.

---

## 2.9 Fail point de cancelamento por reincidência

### Status

**Endereçado parcialmente.**

### Trecho da V2

> “Cancelamento definitivo do serviço por não atendimento reiterado ou decurso de prazo.”

### Avaliação

A V2 passou a reconhecer o cancelamento.

### Falha residual

A fonte oficial é mais específica: o processo pode ser reprovado e cancelado caso persista reincidência do não cumprimento de uma mesma exigência em dois retornos. A V2 fala genericamente em “não atendimento reiterado”, sem registrar a regra dos dois retornos.

### Correção recomendada

Inserir expressamente:

> “O processo poderá ser reprovado e cancelado se persistir a reincidência do não cumprimento de uma mesma exigência em dois retornos.”

---

## 2.10 Omissão do Conselho Técnico

### Status

**Endereçado, mas com distorção.**

### Trecho da V2

> “Instância Contraditória: O Conselho Técnico da DIEAP.”

### Avaliação

A V2 incluiu o Conselho Técnico, mas o descreveu de forma problemática.

### Falha nova

O Conselho Técnico não deve ser tratado simplesmente como “Conselho Técnico da DIEAP” nem como “instância recursal de bastidor” ordinária. A IN nº 01/2021 trata o Conselho Técnico do Departamento de Segurança Contra Incêndio como instância superior de decisão sobre assuntos relacionados à SCIP e como instância do Sistema de Engenharia Contra Incêndio e Pânico. A V2 reduz e localiza indevidamente essa instância como se fosse apenas colegiado interno da DIEAP.

### Correção recomendada

Trocar por:

> “Conselho Técnico do Departamento de Segurança Contra Incêndio (CTDSCI), instância superior de decisão em matérias de segurança contra incêndio e pânico, acionada em hipóteses específicas, como casos omissos, medidas compensatórias, dispensa ou substituição de exigências e demandas técnicas justificadas.”

---

## 2.11 Backstage de taxa incompleto

### Status

**Parcialmente endereçado.**

### Trecho da V2

> “emissão e anexação do comprovante de pagamento da taxa de análise (salvo nos casos deferidos de isenção).”

### Avaliação

A V2 incluiu isenção e comprovante de pagamento.

### Falhas residuais

O texto não detalha adequadamente a base de cálculo da taxa, a dependência do tipo de projeto e dos sistemas/medidas, nem a diferença entre taxa gerada pelo sistema e pagamento externo quando aplicável. Além disso, “rede bancária do Distrito Federal” é expressão vaga e possivelmente imprecisa.

---

## 2.12 Documentos obrigatórios incompletos

### Status

**Parcialmente endereçado.**

### Avaliação

A V2 incluiu ART/RRT/TRT, memoriais e documentos históricos.

### Falhas residuais

Ainda faltam elementos documentais importantes para casos específicos, por exemplo:

- comprovante de lotação do responsável técnico no caso de órgão público;
- contrato com o responsável técnico no caso de entidade filantrópica;
- comprovação de entidade filantrópica;
- carta ao analista nos casos de demanda ao Conselho Técnico;
- documentação específica exigida para soluções alternativas, substituição ou dispensa de exigências.

---

## 2.13 Omissão da Lista de Verificação do SCIP

### Status

**Endereçado.**

### Trecho da V2

> “Lista de Verificação do SCIP.”

### Avaliação

A V2 incorporou a evidência na etapa de Análise Prévia e na matriz.

### Ponto aberto

A V2 afirma que a Lista é preenchida pelo “triador técnico” e salva no histórico. Isso pode ser operacionalmente verdadeiro, mas não foi comprovado pela pesquisa. Deve ser validado com usuários internos.

---

## 2.14 Omissão de notas obrigatórias no projeto

### Status

**Parcialmente endereçado.**

### Trecho da V2

> “notas obrigatórias exigidas por portaria.”

### Avaliação

A V2 menciona a existência das notas, mas não lista quais são nem vincula as notas aos casos em que se aplicam.

### Ponto aberto

Ainda falta detalhar as notas obrigatórias previstas no Anexo II e distinguir exigências para PSCIP, PARQ, modificação, galpões, depósitos, indústrias ou histórico da edificação.

---

## 2.15 Normativo central citado de forma problemática

### Status

**Não endereçado.**

### Trecho da V2

> “Decreto Distrital nº 42.502/2021 (Regulamenta o RSIP-DF).”

### Problema

A V2 manteve um ponto sensível da V1. A IN nº 01/2021-DESEG/CBMDF referencia expressamente o RSIP-DF aprovado pelo Decreto nº 21.361/2000. A pesquisa continua tratando o Decreto nº 42.502/2021 como regulamento do RSIP-DF sem demonstrar essa relação normativa.

### Correção recomendada

Revisar a base normativa e, no mínimo, inserir:

> “Decreto nº 21.361/2000 — aprova o Regulamento de Segurança Contra Incêndio e Pânico do Distrito Federal, referenciado pela IN nº 01/2021-DESEG/CBMDF.”

Se o Decreto nº 42.502/2021 for mantido, deve ser explicado exatamente qual dispositivo dele incide sobre o serviço.

---

## 2.16 Competência da DIEAP tratada parcialmente

### Status

**Parcialmente endereçado.**

### Avaliação

A V2 identifica a DIEAP como unidade operacional e descreve seu papel geral.

### Ponto aberto

Ainda falta explicitar competências formais da DIEAP e de suas estruturas internas, especialmente análise e aprovação de projetos, emissão de pareceres, organização da rotina de análise, padronização e interface com Conselho Técnico. A V2 marca o regulamento interno como pendente, o que é correto.

---

## 2.17 Conexão com Habite-se simplificada demais

### Status

**Parcialmente endereçado.**

### Trecho da V2

> “Obter a aprovação formal do PSCIP para dar andamento ao processo de Habite-se.”

### Avaliação

Melhorou em relação à V1, pois agora fala em “dar andamento”.

### Falha residual

A matriz ainda afirma:

> “liberando a emissão do Habite-se.”

Isso continua forte demais. A aprovação do PSCIP não “libera” automaticamente o Habite-se; ela compõe uma cadeia que ainda envolve vistoria e demais exigências administrativas.

---

## 2.18 Vistoria para Habite-se fora do encadeamento

### Status

**Não endereçado adequadamente.**

### Problema

A V2 continua encerrando o fluxo no parecer técnico e DWF chancelado, sem explicitar a interface posterior com a vistoria para emissão do Laudo para Habite-se.

### Avaliação

Como o serviço analisado é o PSCIP, não é necessário mapear toda a vistoria como etapa interna do mesmo serviço. Porém, como o documento usa “para fins de Habite-se”, a vistoria deveria aparecer como dependência posterior, handoff, evidência de transição ou limite do escopo.

### Correção recomendada

Inserir uma seção “Fronteira do serviço”:

> “A aprovação do PSCIP encerra o serviço de análise de projeto. A etapa posterior de vistoria para emissão de laudo para Habite-se pertence a outro serviço da DESEG/DIVIS, mas constitui dependência relevante da jornada ampliada do usuário.”

---

## 2.19 Assinatura ICP-Brasil, QR Code e chancela sem comprovação

### Status

**Não endereçado; a falha foi agravada.**

### Trecho da V2

> “Sistema Assinador Digital Corporativo.”

> “QR Code exclusivo de rastreabilidade.”

> “Inserção eletrônica do selo/carimbo do CBMDF em todas as páginas do arquivo único DWF.”

### Problema

A V2 mantém e amplia a afirmação sem apresentar fonte. Pode ser operacionalmente verdadeiro, mas não foi demonstrado no documento.

### Classificação

Inferência tratada como fato.

### Correção recomendada

Marcar como hipótese:

> “[PENDENTE] Validar com a DIEAP/DESEG se a emissão final envolve QR Code, assinatura eletrônica, selo/carimbo em DWF e qual sistema realiza essas operações.”

---

## 2.20 Armazenamento em nuvem/servidor sem fonte

### Status

**Endereçado.**

### Avaliação

A V2 removeu a referência a armazenamento em nuvem.

---

## 2.21 “Regulamento Interno da DESEG” sem identificação

### Status

**Endereçado parcialmente.**

### Trecho da V2

> “Regulamento Interno da DESEG / DIEAP: [PENDENTE/EM ABERTO].”

### Avaliação

A V2 fez o correto ao marcar como pendente.

### Falha residual

Apesar de marcar como pendente no levantamento normativo, a matriz usa “Regimento Interno da DIEAP / DESEG” como normativo aplicável ao recurso. Isso é contraditório: o documento não pode declarar como base aplicável algo que ele próprio diz ainda não ter identificado.

---

## 2.22 ABNT citada genericamente

### Status

**Parcialmente endereçado, mas com novas fragilidades.**

### Trecho da V2

> “ABNT NBR 9077” e “ABNT NBR 13714”.

### Avaliação

A V2 deixou de citar ABNT genericamente e passou a indicar normas específicas.

### Falhas novas

A V2 faz afirmações técnicas amplas sobre as NBRs sem demonstrar que elas são as normas vigentes ou aplicáveis em todos os casos citados. Além disso, reduz o exame técnico praticamente a NBR 9077, NBR 13714 e algumas ITs, omitindo que a aplicação normativa depende da classificação, ocupação, área, altura, risco, medidas de segurança e legislação específica.

### Correção recomendada

Reescrever como:

> “Normas ABNT e ITs específicas podem ser aplicáveis conforme o sistema de segurança, a ocupação e as características da edificação, devendo ser listadas caso a caso.”

---

## 2.23 Fail points tecnológicos importantes omitidos

### Status

**Parcialmente endereçado.**

### Avaliação

A V2 incluiu formato incorreto, DWF acima de 10 MB, ausência de pagamento, ausência de memoriais e documentos históricos.

### Falhas residuais

Ainda faltam fail points relevantes já apontados no audit_v1:

- fragmentação indevida de pranchas;
- layers incorretos ou ausência de layers por medida de segurança;
- problemas de legibilidade no zoom máximo;
- não retorno do processo ao Protocolo da DIEAP;
- uso inadequado da carta ao analista ou da aba de justificativa para Conselho Técnico;
- apresentação de prancha de modificação sem respeito à numeração do projeto anterior.

---

## 2.24 Fail points administrativos omitidos

### Status

**Parcialmente endereçado.**

### Avaliação

A V2 inclui isenção, documentos históricos e classificação incorreta.

### Falhas residuais

Ainda faltam:

- indeferimento de isenção por ausência de comprovação específica;
- ausência de comprovante de lotação ou contrato do responsável técnico;
- erro na comprovação de entidade filantrópica;
- ausência de parecer de aprovação anterior em PSCIP de modificação;
- erro material em endereço, área, medidas de segurança ou dados de processo.

---

## 2.25 Grau de confiança superestimado

### Status

**Melhorou, mas ainda há superestimação parcial.**

### Avaliação

A V2 recalibrou o grau de confiança e marcou algumas lacunas como pendentes.

### Falha residual

O documento classifica como “Alta Confiança” um conjunto amplo que inclui “Prazos Legais, Formato DWF e Etapa de Análise Prévia”. Essa parte é aceitável. Porém, ao longo do documento, outros elementos seguem apresentados como fatos sem validação: QR Code, sistema assinador, módulo de recursos, gravação de atas, triador técnico, visualizador DWF integrado, servidores locais e timeout em horários de encerramento de prazos.

---

# 3. Novas falhas introduzidas pela V2

## 3.1 O termo “DESEGWEB” é usado como fato sem validação

### Trecho da V2

> “SCIP/SCIPWeb (DESEGWEB).”

### Problema

A V2 trata DESEGWEB como sistema formal equivalente ao SCIPWeb, mas não demonstra fonte. Se for nomenclatura interna, precisa de validação. Se não for, pode confundir canal, sistema e retaguarda.

---

## 3.2 “Sistema de Gestão de Recursos do DESEGWEB” foi inventado ou não comprovado

### Trecho da V2

> “Sistema de Gestão de Recursos do DESEGWEB / Gravação de Atas de Reunião Colegiada.”

### Problema

Não há fonte apresentada para a existência desse sistema ou dessa funcionalidade. A IN fala em formalização da demanda técnica e disponibilização do parecer pelo SCIP, não necessariamente em “Sistema de Gestão de Recursos” ou “gravação de atas”.

### Classificação

Inferência operacional não comprovada.

---

## 3.3 “Módulo de Triagem Eletrônica” como sistema específico não comprovado

### Trecho da V2

> “Módulo de Triagem Eletrônica.”

### Problema

A existência de uma triagem é plausível, mas o documento apresenta um módulo específico como se fosse ferramenta formal. Sem validação, deve ser tratado como hipótese.

---

## 3.4 “Ferramenta de medição e visualização DWF integrada” não comprovada

### Trecho da V2

> “Software interno integrado que possibilita ao AGFP conferir escalas...”

### Problema

O Anexo II recomenda visualização prévia no software gratuito Autodesk Design Review antes do envio do DWF. Isso não comprova existência de software interno integrado no CBMDF para medição no DESEGWEB.

---

## 3.5 “Servidores locais da DESEGWEB” é afirmação técnica sem fonte

### Trecho da V2

> “Sobrecarga nos servidores corporativos do CBMDF nos horários de encerramento de prazos.”

### Problema

Pode ser um fail point hipotético, mas não há evidência de infraestrutura local, padrão de sobrecarga, horário crítico ou histórico de timeout.

### Correção recomendada

Marcar como hipótese a validar com logs, GLPI, relatórios de indisponibilidade ou entrevistas.

---

## 3.6 Uso de “prazo legal improrrogável” e “taxativo” sem base explícita

### Trecho da V2

> “prazo legal improrrogável de 3 dias úteis.”

> “Até 3 dias úteis (Taxativo).”

### Problema

A fonte oficial informa o prazo, mas a V2 adiciona qualificação jurídica que não foi demonstrada.

---

## 3.7 Confusão entre Conselho Técnico e recurso administrativo ordinário

### Trecho da V2

> “Rota de Escape (Recurso).”

> “Instância recursal de bastidor.”

### Problema

A V2 transforma o Conselho Técnico em uma espécie de recurso administrativo ordinário contra exigência. A IN trata o CTDSCI como instância técnica superior para casos omissos, medidas compensatórias, dispensa ou substituição de exigências, casos especiais e demandas técnicas justificadas. A forma de acionamento é mais específica do que a V2 sugere.

---

## 3.8 “Entrega das chaves da obra” é extrapolação indevida

### Trecho da V2

> “Documento de fé pública essencial para a entrega das chaves da obra.”

### Problema

Isso foge do serviço público mapeado. Entrega de chaves é consequência contratual/imobiliária privada, não evidência ou objetivo operacional do serviço PSCIP.

---

## 3.9 “Obrigatoriedade da tramitação sem papel” atribuída à Lei do Governo Digital

### Trecho da V2

> “fundamentando a obrigatoriedade da tramitação sem papel.”

### Problema

A Lei nº 14.129/2021 estabelece princípios e regras de Governo Digital, mas a V2 usa a lei para sustentar uma obrigatoriedade específica do serviço sem demonstrar o dispositivo. No caso do PSCIP, a exigência operacional do formato eletrônico decorre de norma setorial do CBMDF/DESEG.

---

## 3.10 Lei da Liberdade Econômica como normativo de emissão e conclusão sem relação clara

### Trecho da V2

> “Normativos Aplicáveis: Lei da Liberdade Econômica (13.874/2019).”

### Problema

A lei pode ter relação geral com atos públicos de liberação econômica, mas o documento não demonstra sua aplicação direta à etapa de “Emissão e Conclusão” do PSCIP. A citação permanece genérica e mal amarrada.

---

## 3.11 Omissão da Lei nº 9.784/1999 e da Lei distrital que a recepciona

### Problema

A V2 cita genericamente “Lei de Processo Administrativo” na matriz, mas não identifica o diploma. A IN nº 01/2021 referencia a Lei nº 9.784/1999 e a Lei nº 2.834/2001, que recepciona a lei federal no DF. O documento deveria citar essas normas expressamente.

---

## 3.12 Omissão das normas de taxa efetivamente referenciadas na IN

### Problema

A V2 trata taxa de modo superficial. A IN nº 01/2021 referencia a Taxa de Segurança Contra Incêndio e Pânico, instituída por lei e regulamentada por decreto, além de atualização por portaria/índice. A V2 não incorpora essa base.

---

## 3.13 Erro de unidade/estrutura institucional: “DIEAP” como divisão

### Trecho da V2

> “Divisão de Exame e Aprovação de Projetos (DIEAP).”

### Problema

A própria IN nº 01/2021 menciona a DIEAP como **Diretoria de Estudos e Análise de Projetos**, não como “Divisão de Exame e Aprovação de Projetos”. Essa é uma falha factual relevante.

### Correção recomendada

Substituir por:

> “Diretoria de Estudos e Análise de Projetos (DIEAP).”

---

# 4. Pontos ainda abertos

## 4.1 Fluxo real de cadastro no SCIPWeb

A V2 marcou como pendente o prazo de liberação de cadastro. Isso deve permanecer em aberto até validação com suporte/DESEG.

## 4.2 Sistemas efetivamente usados no backstage

Precisam de validação:

- DESEGWEB;
- módulo de triagem;
- módulo de recursos;
- visualizador DWF integrado;
- assinador digital;
- emissor de QR Code;
- forma de registro de atas ou pareceres do CTDSCI.

## 4.3 Fronteira entre PSCIP e vistoria para Habite-se

A V2 ainda precisa delimitar melhor o fim do serviço de análise de projeto e o início da vistoria/Laudo para Habite-se.

## 4.4 Modalidades específicas de PSCIP

A V2 cita projeto novo, modificação, retificação e digitalização, mas não estrutura adequadamente as modalidades previstas na IN, como:

- PSCIP obra inicial ou existente;
- PSCIP de modificação;
- PSCIP de bem tombado;
- modificação de bem tombado;
- área não regularizada;
- retificação de dados;
- cópia digital;
- digitalização de processo aprovado.

## 4.5 Regras técnicas do DWF

Ainda faltam no blueprint:

- layers por medida de segurança;
- matriz do projeto arquitetônico com anuência/aprovação/visto anterior;
- cotas, escalas, legendas, notas, detalhes;
- recomendação de conferência no Autodesk Design Review;
- regra de subdivisão quando o arquivo exceder 10 MB;
- vedação de subdivisão quando não ultrapassar o limite.

## 4.6 Conselho Técnico

Precisa ser reescrito com base no CTDSCI, não como simples “Conselho Técnico da DIEAP”.

## 4.7 Taxas e isenções

A V2 precisa detalhar:

- regra de cobrança;
- base normativa;
- hipóteses de isenção;
- documentos comprobatórios;
- fail points de pagamento, ausência de comprovante e cálculo incorreto.

---

# 5. Veredito final

A V2 representa uma melhora substancial em relação à V1, mas ainda mistura três níveis de informação sem separação adequada:

1. fatos oficiais comprovados;
2. inferências plausíveis;
3. hipóteses operacionais não validadas.

A V2 endereçou bem as falhas mais evidentes da V1, especialmente nome do serviço, DWF, TRT, Análise Prévia, AGFP, Conselho Técnico, prazos e fail points documentais.

Entretanto, ainda restam falhas graves:

- manutenção de base normativa problemática sobre o Decreto nº 42.502/2021;
- uso incorreto da denominação da DIEAP;
- tratamento inadequado do CTDSCI como “Conselho Técnico da DIEAP”;
- afirmações não comprovadas sobre sistemas, módulos, QR Code, assinador e infraestrutura;
- rigidez excessiva na regra dos 10 MB;
- ausência da regra dos dois retornos para cancelamento;
- fronteira mal definida entre aprovação do PSCIP e vistoria para Habite-se;
- ausência de modalidades específicas previstas na IN nº 01/2021;
- citação superficial de taxas, processo administrativo e normas técnicas.

## Conclusão

A V2 é adequada como **rascunho avançado** para construção de blueprint, mas ainda não deve ser usada como representação AS-IS oficial sem validação com a DIEAP/DESEG e sem revisão normativa fina.

Para elevar o documento a nível institucional, recomenda-se:

1. separar fatos oficiais de hipóteses;
2. revisar a base normativa;
3. corrigir a denominação da DIEAP;
4. reescrever a seção do CTDSCI;
5. marcar sistemas não comprovados como pendentes;
6. inserir a regra completa do DWF;
7. delimitar claramente o fim do PSCIP e a transição para vistoria/Habite-se;
8. detalhar documentos e fail points por modalidade de serviço.
