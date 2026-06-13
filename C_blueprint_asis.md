## Service Blueprint AS-IS — Análise de PSCIP (Obra Inicial) para Habite-se no DF

**Serviço:** Análise de Projeto de Segurança Contra Incêndio e Pânico (PSCIP) — modalidade **Obra Inicial** (edificações novas), realizada pelo CBMDF/DESEG/DIEAP via SCIPWeb.

**Escopo e fronteira do serviço:** este blueprint cobre exclusivamente a modalidade **PSCIP Obra Inicial**, das 7 modalidades previstas na IN nº 01/2021-DESEG/CBMDF (as demais — Edificação Existente, Modificação, Bem Tombado, Área Não Regularizada, Retificação e Cópia Digital — possuem fluxos AS-IS distintos e não são tratadas aqui). O serviço **encerra-se na emissão do Parecer Técnico de Aprovação e das pranchas chanceladas com QR Code** — a emissão da Carta de Habite-se em si é ato do GDF, fora do escopo desta jornada, e a vistoria predial (DIVIS) é um *handoff* posterior.

**Nota de fluxo:** o caminho principal da jornada é **1 → 2 → 3 → 4 → 5 → 8**. As etapas **6 (Demanda Superior/CTDSCI)** e **7 (Correção de Projeto)** são **desvios condicionais/iterativos**: a etapa 7 pode ocorrer entre 4→4, 5→5 ou após 6, repetindo-se até 2 vezes (na 3ª reincidência da mesma exigência, o processo é cancelado); a etapa 6 só ocorre em casos especiais (solução alternativa de engenharia, medida compensatória, dispensa de exigência ou caso omisso na norma), normalmente acionada a partir da etapa 5 ou 7.

Legenda: ⚠️ = informação não confirmada pela pesquisa documental (hipótese a validar com a equipe de TI/gestão da DESEG).

**As 5 camadas de Shostack representadas nas linhas desta matriz são:** (1) **Evidências Físicas**, (2) **Ações do Cidadão**, (3) **Frontstage** (visível), (4) **Backstage** (invisível) e (5) **Processos de Suporte** (retaguarda). Elas são separadas pelas 3 linhas divisórias — *Linha de Interação* (entre Ações do Cidadão e Frontstage), *Linha de Visibilidade* (entre Frontstage e Backstage) e *Linha de Interação Interna* (entre Backstage e Processos de Suporte). A linha **Prazos / Tempo de Espera** (topo) e a linha **⚠ Fail points** (base) são complementos transversais, não camadas de Shostack.

---

## Matriz do Blueprint (camadas × etapas)

| Camada \ Etapa | 1. Preparação | 2. Peticionamento | 3. Envio e Protocolo | 4. Análise Prévia | 5. Exame do AGFP | 6. Demanda Superior *(condicional — apenas casos especiais/CTDSCI)* | 7. Correção de Projeto *(iterativo — repete até 2x; 3ª reincidência = cancelamento)* | 8. Certificação |
|---|---|---|---|---|---|---|---|---|
| **Prazos / Tempo de Espera** | Autoatendimento (imediato) | ⚠️ tempo de homologação do cadastro profissional não documentado | ⚠️ tempo de processamento do protocolo/compensação bancária não documentado | Até **3 dias úteis** | **15 dias úteis** (prorrogável por +15 dias úteis em casos complexos) | **10 dias úteis** para deliberação; +15 dias úteis para adequação se deferido com condicionantes | **30 dias corridos** (usuário); **15 dias úteis** se pós-CTDSCI | ⚠️ tempo de disponibilização dos downloads pós-assinatura não documentado |
| **Evidências Físicas** | PDFs de Instruções Técnicas (ITs) baixados do portal DESEG | Tela de cadastro/login e formulário eletrônico de dados da edificação no SCIPWeb | Recibo de Protocolo Eletrônico com numeração sequencial | Lista de Verificação do SCIP preenchida (⚠️ visibilidade ao usuário não confirmada) | Status "Em Análise pelo AGFP" no painel; eventual Relatório de Exigências Técnicas | Ata de Deliberação do Colegiado do CTDSCI | Relatório de Exigências Técnicas ("Comunique-se") em PDF | Parecer Técnico de Aprovação (PDF) + pranchas DWF chanceladas com Selo Digital e QR Code |
| **Ações do Cidadão** | Consulta ITs e classifica o risco/carga de incêndio da edificação | Login/cadastro profissional; preenchimento de área, altura, ocupação e sistemas preventivos projetados | Upload do projeto em DWF único (ou subdividido conforme Anexo II, ≤10MB), ART/RRT/TRT e memoriais de cálculo; anexa comprovante de taxa | Aguarda; consulta status "Em Análise Prévia" | Aguarda; consulta status "Em Análise pelo AGFP" | Anexa "Carta ao Analista" justificando solução alternativa/medida compensatória/dispensa de exigência | Baixa o Comunique-se, corrige DWF e memoriais, reenvia o lote | Acessa aba de certidões e baixa parecer e pranchas chanceladas |
| — *Linha de Interação* — | | | | | | | | |
| **Frontstage** (visível) | Portal público da DESEG (conteúdo estático de autoatendimento, sem atendente) | Interface de cadastro/formulário do SCIPWeb | Módulo de Peticionamento/Upload do SCIPWeb | Painel de status do SCIPWeb ("Em Análise Prévia") | Painel de status do SCIPWeb ("Em Análise pelo AGFP") | Tela de envio de demandas/anexação ao CTDSCI | SCIPWeb/DESEGWEB — tela de reenvio de arquivos revisados | Módulo de Downloads/Certidões do SCIPWeb |
| — *Linha de Visibilidade* — | | | | | | | | |
| **Backstage** (invisível) | ⚠️ Manutenção/atualização das ITs e indexação do portal pela equipe da DESEG | ⚠️ Triagem/validação administrativa do cadastro do profissional (CREA/CAU) pelo suporte do CBMDF | Recepção eletrônica do lote e direcionamento à fila de triagem; checagem de compensação da taxa | Triador/Equipe Técnica da DIEAP aplica a Lista de Verificação do SCIP (formato DWF, ART/RRT/TRT, limite de 10MB, notas obrigatórias) | AGFP confronta pranchas e memoriais com NBR 9077, NBR 13714 e ITs (rotas de fuga, hidrantes, chuveiros automáticos, pressurização de escadas) | Colegiado do CTDSCI avalia casos omissos na norma, soluções de desempenho ou medidas compensatórias | Equipe da DIEAP recebe o reenvio e verifica o cumprimento exato dos itens notificados; controla a contagem de reincidências | Chefia da DIEAP/Diretor da DESEG homologa o parecer final do AGFP e aplica a chancela institucional |
| — *Linha de Interação Interna* — | | | | | | | | |
| **Processos de Suporte** | Manutenção normativa e publicação/indexação das ITs no portal (retaguarda da DESEG) | Sustentação e disponibilidade do sistema de cadastro (TI do CBMDF, sobre o SCIPWeb) | Conciliação e compensação bancária da taxa (arrecadação do GDF) + sustentação do peticionamento | ⚠️ Operação da rotina de triagem e da Lista de Verificação (retaguarda da DIEAP, sobre o DESEGWEB) | ⚠️ Suporte técnico de medição/visualização do DWF ao AGFP (DESEGWEB) | ⚠️ Secretariado do CTDSCI: pauta, deliberação e arquivo de atas | Versionamento e guarda do histórico de reenvios e exigências (SCIPWeb/DESEGWEB) | ⚠️ Processo de certificação digital: assinatura ICP-Brasil, selagem e geração de QR Code (retaguarda da DESEG) |
| **⚠ Fail points** | Risco/carga de incêndio mal classificado | Timeout do SCIPWeb em picos ⚠️ | **DWF fora do padrão (>10MB) ou ART/RRT/TRT ausente** | Devolução por DWF/memoriais incompletos | Divergência de interpretação entre AGFPs | Indeferimento por "Carta ao Analista" mal fundamentada | **Reincidência em 2 retornos = cancelamento** | QR Code/assinatura corrompidos ⚠️ |

---

## Fail Points por etapa

### 1. Preparação
- **Interpretação equivocada da classificação de risco/carga de incêndio da edificação.**
  - *Causa raiz:* complexidade interpretativa do arcabouço normativo (ITs, NBRs) sem orientação centralizada.
  - *Consequência:* enquadramento incorreto do projeto, gerando memoriais de cálculo incompatíveis já na etapa 3 (Envio e Protocolo).

**Normativos:** Decreto Distrital nº 21.361/2000 (RSIP-DF).

### 2. Peticionamento
- **Lentidão/timeout do SCIPWeb em períodos de pico de fechamento de prazos.** ⚠️ (hipótese a validar)
  - *Causa raiz:* possível sobrecarga da infraestrutura de servidores que sustentam o SCIPWeb.
  - *Consequência:* perda dos dados digitados no formulário, exigindo novo preenchimento.

**Normativos:** Lei Federal nº 9.784/1999 e Lei Distrital nº 2.834/2001 (prazos em dias úteis, motivação dos atos).

### 3. Envio e Protocolo
- **Transmissão do DWF fora do padrão ou fragmentação indevida (acima de 10MB sem seguir o Anexo II).**
  - *Causa raiz:* desconhecimento das regras de formatação/subdivisão do Anexo II da IN nº 01/2021.
  - *Consequência:* rejeição do lote já na Análise Prévia (etapa 4), sem avançar para o exame técnico.
- **Omissão de ART/RRT/TRT ou do comprovante de recolhimento da taxa.**
  - *Causa raiz:* falha na instrução documental obrigatória no momento do upload.
  - *Consequência:* rejeição administrativa imediata do protocolo.

**Normativos:** Anexo II da IN nº 01/2021-DESEG/CBMDF.

### 4. Análise Prévia
- **Devolução por omissão de memoriais de cálculo ou erros formais do DWF (legibilidade, *layers*, notas obrigatórias).**
  - *Causa raiz:* falha na revisão do arquivo vetorial antes do upload.
  - *Consequência:* processo devolvido ao Protocolo da DIEAP sob status "Exigência na Análise Prévia", reiniciando a contagem do prazo de 3 dias úteis.

**Normativos:** IN nº 01/2021-DESEG/CBMDF (Lista de Verificação do SCIP).

### 5. Exame do AGFP
- **Subjetividade/divergência de interpretação normativa entre diferentes AGFPs.**
  - *Causa raiz:* ausência de padronização interpretativa interna na DIEAP.
  - *Consequência:* exigências mal fundamentadas, induzindo o usuário ao erro e alimentando o "comunique-se infinito" (loop com a etapa 7).

**Normativos:** ABNT NBR 9077, ABNT NBR 13714 e ITs do CBMDF.

### 6. Demanda Superior (CTDSCI) — condicional
- **Erros de fundamentação na "Carta ao Analista" levam ao indeferimento pelo CTDSCI.**
  - *Causa raiz:* despreparo do requerente para justificar tecnicamente a solução alternativa ou medida compensatória.
  - *Consequência:* retorno ao fluxo padrão sem a flexibilização pretendida, com perda de até 10 dias úteis de tramitação.

**Normativos:** IN nº 01/2021-DESEG/CBMDF (regras de competência e prazos do CTDSCI).

### 7. Correção de Projeto — iterativo
- **Reincidência da mesma exigência técnica em 2 retornos consecutivos.**
  - *Causa raiz:* incapacidade do projetista de sanar a inconformidade, ou falta de clareza no Relatório de Exigências Técnicas emitido na etapa 5.
  - *Consequência:* **reprovação e cancelamento definitivo do processo, com perda da taxa paga**, obrigando o requerente a reiniciar todo o rito a partir da etapa 3.

**Normativos:** Lei Federal nº 9.784/1999 (prazos de resposta do administrado).

### 8. Certificação
- **Erro na gravação do QR Code ou corrupção da assinatura eletrônica do arquivo DWF.** ⚠️ (hipótese a validar)
  - *Causa raiz:* possível incompatibilidade entre plugins de visualização/assinatura e o sistema corporativo de certificação.
  - *Consequência:* documento final não confiável para uso no Habite-se ou em vistorias futuras, exigindo reemissão pela chefia da DIEAP.

**Normativos:** Lei Distrital nº 6.138/2018 (Código de Obras do DF); IN nº 01/2021-DESEG/CBMDF (certificação digital).
