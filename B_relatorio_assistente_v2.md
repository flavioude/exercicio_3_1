# PESQUISA PARA CONSTRUÇÃO DE SERVICE BLUEPRINT AS-IS (V2.0)
## Serviço: Análise de Projeto de Segurança Contra Incêndio e Pânico (PSCIP) para fins de Habite-se, Licenciamento e Regularização no Distrito Federal
**Órgão Executor:** Corpo de Bombeiros Militar do Distrito Federal (CBMDF)  
**Unidade Operacional:** Diretoria de Serviços Técnicos (DESEG) / Divisão de Exame e Aprovação de Projetos (DIEAP)

---

## ETAPA 1 — MAPEAMENTO DA JORNADA DO CIDADÃO

A jornada do usuário (responsável técnico habilitado) ocorre de forma eletrônica através do sistema de retaguarda corporativa **SCIP/SCIPWeb** (DESEGWEB).

```
[ Fase 1: Entrada ] ──> [ Fase 2: Análise Prévia ] ──> [ Fase 3: Corte Técnico AGFP ] ──> [ Fase 4: Homologação / Conselho ]
```

### Fase 1: Preparação, Enquadramento e Peticionamento

#### 1. Consulta Normativa e Compilação Histórica
*   **Objetivo do Usuário:** Determinar os parâmetros de proteção contra incêndio exigidos para o edifício e coletar os antecedentes da área.
*   **Ação Realizada:** Download das Instruções Técnicas (ITs) do CBMDF e das NBRs aplicáveis; levantamento de projetos aprovados anteriormente, Habite-se anteriores ou alvarás antigos (caso o pedido seja de modificação/retificação).
*   **Canal Utilizado:** Portal Oficial do CBMDF (Área da DESEG).
*   **Informações Fornecidas / Documentos:** Consulta passiva realizada pelo usuário.
*   **Decisões / Dúvidas:** A edificação se enquadra em projeto novo, modificação, retificação ou apenas digitalização de prancha física antiga? Há direito a pedido de isenção de taxa (ex: órgãos públicos ou entidades assistenciais)?
*   **Tempo de Espera:** Imediato (autoatendimento).
*   **Dependências Externas:** Nenhuma.
*   **Entradas:** Demanda do cliente/proprietário; **Saídas:** Diagnóstico técnico inicial elaborado pelo profissional.
*   **Evidências Geradas:** Legislação e documentos históricos baixados.
*   **Emoções/Frustrações:** Insegurança em virtude da alta complexidade na interpretação cruzada de normas técnicas antigas e novas.

#### 2. Autenticação e Entrada de Dados no SCIPWeb
*   **Objetivo do Usuário:** Realizar a identificação formal do profissional e abrir o processo eletrônico de análise técnica.
*   **Ação Realizada:** Entrada no sistema informando credenciais locais e preenchimento detalhado dos dados da edificação (área construída, altura, ocupação, carga de incêndio).
*   **Canal Utilizado:** Interface do sistema SCIPWeb.
*   **Informações Fornecidas:** Dados de identificação do proprietário, endereço completo da obra, dados técnicos estruturais e indicação se há solicitação de isenção de taxas.
*   **Documentos Anexados:** Carteira do conselho de classe, e documentação comprobatória de imunidade/isenção de taxa (quando aplicável).
*   **Decisões / Dúvidas:** O sistema processará corretamente o preenchimento sem apresentar erros de timeout?
*   **Tempo de Espera:** **[PENDENTE/EM ABERTO]** Validar o tempo exato necessário para a homologação de novos cadastros de profissionais no SCIPWeb.
*   **Dependências Externas:** Análise humana da administração do sistema para a liberação de novos perfis.
*   **Entradas:** Dados do profissional e do imóvel; **Saídas:** Tela de cadastro inicial preenchida.
*   **Evidências Geradas:** Dados gravados em tela no formulário do SCIPWeb.
*   **Emoções/Frustrações:** Insatisfação devido à rigidez no preenchimento dos formulários eletrônicos.

#### 3. Upload de Projetos, Memoriais e Protocolo Final
*   **Objetivo do Usuário:** Transmitir formalmente todas as peças do PSCIP para avaliação da corporação.
*   **Ação Realizada:** Upload do arquivo técnico de projeto e dos memoriais complementares; emissão e anexação do comprovante de pagamento da taxa de análise (salvo nos casos deferidos de isenção).
*   **Canal Utilizado:** Módulo de Peticionamento e Upload do SCIPWeb.
*   **Informações Fornecidas:** Metadados das pranchas de projeto e declaração de responsabilidade pelas informações prestadas.
*   **Documentos Anexados:** **Arquivo único em formato DWF (limite estrito de 10 MB)** contendo o projeto arquitetônico de incêndio com as notas obrigatórias exigidas por portaria; Anotação de Responsabilidade Técnica (ART/CREA), Registro de Responsabilidade Técnica (RRT/CAU) ou Termo de Responsabilidade Técnica (TRT/CFT); Memorial Descritivo e Memoriais de Cálculo específicos (Cálculo populacional/saídas, dimensionamento hidráulico de hidrantes/chuveiros automáticos, e pressurização de escadas).
*   **Decisões / Dúvidas:** O arquivo DWF ultrapassará o limite de tamanho do sistema? Os memoriais contêm todas as variáveis exigidas pelas NBRs específicas?
*   **Tempo de Espera:** Tempo de processamento do upload e processamento da taxa de análise pelo banco.
*   **Dependências Externas:** Compensação da rede bancária do Distrito Federal.
*   **Entradas:** Arquivos técnicos em formato digital (.dwf, .pdf); **Saídas:** Geração do número de processo eletrônico e emissão do Comprovante de Protocolo.
*   **Evidências Geradas:** Recibo de Protocolo com número de controle sequencial.
*   **Emoções/Frustrações:** Temor de rejeição sumária do arquivo por problemas de formatação digital ou tamanho.

---

### Fase 2: Interação e Resposta a Exigências

#### 4. Acompanhamento de Prazos e Retorno de Pendências
*   **Objetivo do Usuário:** Sanar as inconformidades apontadas pelo CBMDF e evitar o cancelamento ou arquivamento do pedido.
*   **Ação Realizada:** Monitoramento do painel eletrônico. Em caso de emissão de exigências (seja na Análise Prévia ou no exame do AGFP), o usuário acessa o relatório, corrige os arquivos originais e faz o reenvio (re-upload) dos documentos modificados.
*   **Canal Utilizado:** Central de Notificações do SCIPWeb / E-mail cadastrado.
*   **Informações Fornecidas:** Justificativas técnicas de alteração e notas de revisão no projeto.
*   **Documentos Anexados:** Novo arquivo único DWF revisado e memoriais retificados.
*   **Decisões / Dúvidas:** O prazo legal de resposta será suficiente para alterar os projetos executivos? A fundamentação do analista é passível de recurso ao Conselho Técnico?
*   **Tempo de Espera:** **30 dias corridos** é o prazo máximo legal concedido ao requerente para responder a qualquer exigência, sob pena de cancelamento do processo.
*   **Dependências Externas:** Nenhuma.
*   **Entradas:** Relatório de Exigências / Notificação de Comunique-se; **Saídas:** Resposta de exigência protocolada no sistema.
*   **Evidências Geradas:** Histórico de trâmites com registro de reenvio de documentos.
*   **Emoções/Frustrações:** Elevada frustração e retrabalho quando as exigências são interpretadas como excessivamente detalhistas ou repetitivas.

---

### Fase 3: Recebimento do Resultado Técnico

#### 5. Coleta do Parecer Técnico e Certificação Visual
*   **Objetivo do Usuário:** Obter a aprovação formal do PSCIP para dar andamento ao processo de Habite-se nas Administrações Regionais do GDF.
*   **Ação Realizada:** Download dos arquivos finais validados pelo CBMDF.
*   **Canal Utilizado:** Módulo de Certidões e Encerramento do SCIPWeb.
*   **Informações Fornecidas:** Nenhuma (etapa de download).
*   **Documentos Anexados:** Nenhum.
*   **Decisões / Dúvidas:** O documento emitido possui alguma incorreção gráfica no nome das partes ou endereço que inviabilize o Habite-se no órgão distrital?
*   **Tempo de Espera:** Imediato após a assinatura digital da autoridade competente da DIEAP.
*   **Dependências Externas:** Sistemas de validação de assinaturas eletrônicas.
*   **Entradas:** Despacho favorável do chefe da seção; **Saídas:** Parecer Técnico de Aprovação emitido e pranchas homologadas.
*   **Evidências Geradas:** Parecer Técnico Digital e pranchas em formato chancelado contendo QR Code institucional impresso para verificação de autenticidade.
*   **Emoções/Frustrações:** Alívio e satisfação com a conclusão do trâmite técnico de segurança.

---

## ETAPA 2 — PROCESSOS DE BASTIDOR (BACKSTAGE)

O fluxo interno de trabalho na DIEAP/DESEG é rigidamente balizado por competências legais e prazos peremptórios, operando por meio dos seguintes passos sequenciais:

```
[ Protocolo ] ──> [ Análise Prévia (3 dias úteis) ] ──> [ Distribuição ao AGFP ] ──> [ Exame Técnico (15 dias úteis) ] ──> [ Homologação ou Conselho ]
```

### 1. Triagem e Fluxo de Isenção de Taxas
*   **Responsável:** Setor Administrativo / Protocolo da DIEAP.
*   **Objetivo:** Validar a regularidade inicial do processo, operando a conferência da compensação bancária ou o exame do pedido de isenção de taxas.
*   **Sistemas Utilizados:** Retaguarda do DESEGWEB.
*   **Regras Aplicadas / Critérios:** Em caso de pedido de isenção, o processo é desviado para análise do fundamento legal apresentado pela entidade pública ou filantrópica. Se ausente o comprovante ou o direito à isenção, ocorre a rejeição administrativa imediata.

### 2. Etapa Formal de Análise Prévia
*   **Responsável:** Triador Técnico / Agente designado da DIEAP.
*   **Objetivo:** Executar o exame formal inicial para assegurar que o processo contém os elements mínimos indispensáveis para o corte técnico.
*   **Sistemas Utilizados:** Módulo de Triagem do DESEGWEB.
*   **Regras Aplicadas / Critérios:** Aplicação estrita da **Lista de Verificação do SCIP**. O agente avalia se o arquivo está no formato DWF correto, se possui tamanho máximo de 10 MB, se as ARTs/RRTs/TRTs de projeto e os memoriais descritivos/cálculos foram anexados de forma legível.
*   **Prazos e Fluxo de Retorno:** Esta etapa possui o prazo legal improrrogável de **3 dias úteis**. Caso falte qualquer item da lista de verificação, o processo não avança para os analistas; ele é imediatamente devolvido ao requerente com o status de "Exigência na Análise Prévia", interrompendo o fluxo até a regularização.

### 3. Exame Detalhado pelo Agente Fiscalizador de Projetos (AGFP)
*   **Responsável:** Agente Fiscalizador de Projetos (AGFP) da DIEAP.
*   **Objetivo:** Realizar a verificação técnica aprofundada dos sistemas de segurança contra incêndio projetados para a edificação.
*   **Sistemas Utilizados:** DESEGWEB, ferramentas corporativas de medição em ambiente DWF e planilhas de cálculo normativo.
*   **Regras Aplicadas e Critérios de Exame:** O AGFP confronta os memoriais e pranchas com os parâmetros das Instruções Técnicas do CBMDF e das normas reguladoras brasileiras, avaliando detalhadamente:
    *   *NBR 9077:* Dimensionamento de saídas de emergência, larguras de escadas, rotas de fuga e cálculo de lotação da edificação.
    *   *NBR 13714:* Dimensionamento hidráulico, posicionamento de abrigos, mangotinhos e hidrantes.
    *   *ITs Específicas:* Dimensionamento de sistemas de pressurização de escadas e chuveiros automáticos.
*   **Prazos Regimentais:** O AGFP dispõe do prazo de **15 dias úteis** para concluir o exame, sendo admitida uma prorrogação por mais **15 dias úteis** mediante justificativa fundamentada da chefia em virtude da alta complexidade estrutural do edifício.

### 4. Instância Contraditória: O Conselho Técnico da DIEAP
*   **Responsável:** Colegiado do Conselho Técnico (Presidente e Oficiais Membros).
*   **Objetivo:** Dirimir divergências de interpretação normativa entre o AGFP e o responsável técnico do projeto, atuando como instância recursal de bastidor.
*   **Sistemas Utilizados:** Sistema de Gestão de Recursos do DESEGWEB / Gravação de Atas de Reunião Colegiada.
*   **Regras Aplicadas / Prazos:** Quando provocado formalmente por recurso do requerente contra uma exigência considerada indevida, o Conselho Técnico possui o prazo de **10 dias úteis** para emitir parecer deliberativo colegiado. Se o Conselho mantiver a exigência com ajustes, o interessado terá o prazo de **15 dias úteis** para efetuar a correção estrita nas pranchas e memoriais de cálculo.

### 5. Homologação Final e Assinatura Digital
*   **Responsável:** Chefe da DIEAP / Diretor da DESEG.
*   **Objetivo:** Conceder validade jurídica institucional ao ato de aprovação do projeto de segurança.
*   **Sistemas Utilizados:** Módulo Assinador Digital integrado com criptografia e chaves públicas reconhecidas.
*   **Automação vs. Ação Humana:**
    *   *Processo Automatizado:* Inserção eletrônica do selo/carimbo do CBMDF em todas as páginas do arquivo único DWF e a geração do QR Code exclusivo de rastreabilidade.
    *   *Análise Humana:* O julgamento técnico de conformidade dos cálculos de engenharia permanece 100% dependente do AGFP humano.

---

## ETAPA 3 — EVIDÊNCIAS FÍSICAS E DIGITAIS

| Evidência Digital / Física | Etapa de Aparição | Quem Gera | Finalidade Operacional | Valor Percebido pelo Usuário |
| :--- | :--- | :--- | :--- | :--- |
| **Interface de Preenchimento do SCIPWeb** | Cadastro e Acesso | Sistema (Automático) | Capturar os dados primários da edificação para fins estatísticos e de controle fiscal. | Registro inicial da demanda no ecossistema público. |
| **Recibo de Protocolo Eletrônico** | Upload de Projetos | Sistema (Automático) | Garantir a comprovação jurídica do peticionamento tempestivo dos projetos pelo usuário. | Comprovação legal de entrega e contagem de prazos administrativos. |
| **Lista de Verificação do SCIP** | Análise Prévia | Triador Técnico da DIEAP | Registrar o cumprimento ou ausência dos requisitos formais mínimos do DWF e das taxas. | Transparência imediata sobre a regularidade formal do lote enviado. |
| **Relatório de Exigências do AGFP** | Exame Técnico / Correção | Agente Fiscalizador (AGFP) | Enumerar as falhas técnicas de projeto apontando explicitamente o item normativo violado. | Roteiro objetivo para correções, reduzindo a margem de erro. |
| **Ata de Deliberação do Conselho Técnico** | Recurso Administrativo | Colegiado da DIEAP | Formalizar a decisão sobre divergências interpretativas de normas ou ITs. | Segurança jurídica e possibilidade de defesa técnica contra decisões monocráticas. |
| **Parecer Técnico Conclusivo e DWF Chancelado** | Finalização do Serviço | Chefe da DIEAP via Sistema | Certificar que o edifício cumpre os parâmetros preventivos, liberando a emissão do Habite-se. | Documento de fé pública essencial para a entrega das chaves da obra. |
| **Selo Digital com QR Code Institucional** | Finalização do Serviço | Sistema de Emissão da DESEG | Permitir a validação imediata da autenticidade do projeto impresso por fiscais externos. | Praticidade e segurança contra fraudes ou adulterações de projetos. |

---

## ETAPA 4 — LEVANTAMENTO NORMATIVO

O serviço é estruturado sobre o seguinte ordenamento jurídico e técnico:

### 1. Legislação de Governança e Processo Eletrônico
*   **Lei Federal nº 14.129/2021 (Lei do Governo Digital):** Estabelece os parâmetros de modernização e prestação digital de serviços públicos, fundamentando a obrigatoriedade da tramitação sem papel.
*   **Lei Federal nº 13.874/2019 (Lei da Liberdade Econômica):** Fixa as garantias de livre mercado e os prazos máximos para manifestação da administração pública nos atos de liberação de atividade econômica.

### 2. Normativos e Regulamentos do Distrito Federal
*   **Decreto Distrital nº 42.502/2021 (Regulamenta o RSIP-DF):** Regulamenta o Regulamento de Segurança Contra Incêndio e Pânico do Distrito Federal, fixando as atribuições fiscalizatórias e de exame de projetos conferidas à DESEG.
*   **Lei Distrital nº 6.138/2018 (Código de Obras do Distrito Federal):** Dispõe sobre as regras construtivas do DF, condicionando a concessão de Carta de Habite-se pelas Administrações Regionais à aprovação do PSCIP pelo CBMDF.

### 3. Atos Normativos Específicos do CBMDF
*   **Portaria de Análise Digital do CBMDF (IT de Análise Digital vigente):** Normativo que disciplina as regras de envio eletrônico de projetos, instituindo a obrigatoriedade do arquivo único em formato **DWF com tamanho máximo de 10 MB**, além de fixar a estrutura obrigatória de notas e legendas nas pranchas.
*   **Regulamento Interno da DESEG / DIEAP:** **[PENDENTE/EM ABERTO]** Solicitar à Assessoria Técnico a especificação do número e data de publicação do ato regulamentar vigente que detalha a estrutura interna das seções de exame de projetos da DIEAP.

### 4. Normas Técnicas de Engenharia Aplicadas ao Exame de Projetos
*   **ABNT NBR 9077 (Saídas de Emergência em Edifícios):** Fixa os critérios mínimos para o dimensionamento de escadas, rampas, rotas de fuga, portas corta-fogo e cálculo de capacidade de população das áreas.
*   **ABNT NBR 13714 (Sistemas de Hidrantes e de Mangotinhos para Combate a Incêndio):** Estabelece as regras de vazão, pressão, diâmetro de tubulações e reserva técnica de incêndio para os sistemas hidráulicos sob comando.

---

## ETAPA 5 — FAIL POINTS (PONTOS DE FALHA)

Mapeamento abrangente de vulnerabilidades na jornada, atualizado de acordo com as regras operacionais da corporação.

### 1. Falhas do Usuário (Requerente Técnico)
*   **Envio de prancha em formato incorreto (ex: PDF comum) ou arquivo DWF acima de 10 MB:**
    *   *Causa Raiz:* Falha na leitura das diretrizes contidas na Portaria de Análise Digital do CBMDF.
    *   *Consequência:* Bloqueio mecânico de upload no sistema ou rejeição sumária do processo na fase de Análise Prévia.
*   **Classificação incorreta do risco ou da natureza do serviço solicitado (ex: marcar projeto novo quando se trata de retificação):**
    *   *Causa Raiz:* Erro de enquadramento técnico por parte do profissional do setor privado.
    *   *Consequência:* Cancelamento do processo administrativo por inconsistência de dados cadastrais, gerando perda das taxas recolhidas.
*   **Ausência de documentos históricos obrigatórios (Projetos antigos/Habite-se anterior) em casos de modificação:**
    *   *Causa Raiz:* Falta de saneamento prévio e pesquisa documental do arquivo do edifício pelo projetista.
    *   *Consequência:* Emissão de exigência na Análise Prévia, paralisando o andamento do processo.
*   **Omissão de memoriais de cálculo específicos (Hidrantes, População, Escada Pressurizada) ou ausência de TRT/ART/RRT:**
    *   *Causa Raiz:* Negligência técnica na compilação do lote de arquivos de engenharia.
    *   *Consequência:* Devolução do processo antes de ingressar na fila do AGFP.

### 2. Falhas Sistêmicas (Infraestrutura de TI)
*   **Lentidão extrema e erros de interrupção de upload (Timeout) nos servidores locais da DESEGWEB:**
    *   *Causa Raiz:* Sobrecarga nos servidores corporativos do CBMDF nos horários de encerramento de prazos.
    *   *Consequência:* Perda dos dados preenchidos nos formulários e necessidade de reiniciar o peticionamento do zero.
*   **Indisponibilidade de visualização de arquivos DWF assinados eletronicamente:**
    *   *Causa Raiz:* Bugs de atualização nos plugins de renderização de imagem do sistema SCIPWeb.
    *   *Consequência:* Impossibilidade de o AGFP prosseguir com o exame, provocando atrasos operacionais.

### 3. Falhas Operacionais e de Bastidor
*   **Não atendimento reiterado das exigências técnicas dentro dos prazos regulamentares:**
    *   *Causa Raiz:* Falta de capacidade técnica do projetista privado em sanar os erros apontados ou perda de prazos internos.
    *   *Consequência:* **Cancelamento definitivo do serviço** por abandono/decurso de prazo após o encerramento dos 30 dias corridos.
*   **Erros ou ausência de fundamentação legal na justificativa de exigências emitidas pelo AGFP:**
    *   *Causa Raiz:* Falta de clareza do agente ou erro material na indicação do item infringido da IT ou NBR.
    *   *Consequência:* Indução do usuário ao erro, gerando retrabalho crônico e a necessidade de abertura de recurso ao Conselho Técnico.

---

## ETAPA 6 — SISTEMAS E INTEGRAÇÕES

O ecossistema computacional é composto pelas seguintes ferramentas de operação:

1.  **SCIPWeb / DESEGWEB:** Portal centralizador que gerencia o fluxo de processos (Workflow) e controla as cargas de distribuição de pastas de projetos na DIEAP.
2.  **Módulo de Triagem Eletrônica:** Interface que apresenta a Lista de Verificação do SCIP para o preenchimento obrigatório pelo triador na fase de Análise Prévia.
3.  **Ferramenta de Medição e Visualização DWF:** Software interno integrado que possibilita ao AGFP conferir escalas, raios de cobertura de hidrantes e caminhos de fuga nas pranchas digitais.
4.  **Sistema Assinador Digital Corporativo:** Infraestrutura de criptografia responsável por autenticar o Parecer Técnico e aplicar o selo digital com o QR Code de segurança sobre as pranchas chanceladas.

---

## ETAPA 7 — MATRIZ SERVICE BLUEPRINT (AS-IS V2.0)

| Etapa da Jornada | Ação do Usuário | Frontstage (Interações Visíveis) | Linha de Visibilidade | Backstage (Processos Internos) | Sistemas Envolvidos | Evidência Física/Digital | Normativos Aplicáveis | Tempo de Espera Regulamentar | Fail Points Críticos |
| :--- | :--- | :--- | :---: | :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Preparação Histórica** | Compila normas e busca projetos anteriores e certidões de alvarás antigos da edificação. | Consulta passiva à seção de normas e acervos do CBMDF. | ────── | Atualização e upload das normas no portal pelo setor técnico. | Portal do CBMDF (DESEG) | PDFs das ITs e NBRs baixados; plantas antigas da área. | Decreto Distrital 42.502/2021 | Autoatendimento (Imediato) | **Ausência de documentos históricos da edificação** nos casos de modificação. |
| **2. Peticionamento** | Insere dados do imóvel, indica pedido de isenção de taxa e anexa os registros profissionais. | Tela de abertura de processo e formulários do SCIPWeb. | ────── | **[PENDENTE]** Triagem humana dos dados cadastrais do profissional de engenharia/arquitetura. | SCIPWeb (Módulo Cadastro) | Campos validados e gravados em tela. | Lei do Governo Digital (14.129/2021) | **[PENDENTE]** Validar prazo de liberação de cadastro. | Erros de timeout e perda de dados por queda de conexão nos servidores locais. |
| **3. Protocolo e Envio** | Faz upload do arquivo único DWF e dos memoriais, anexando o comprovante da taxa. | Upload concluído e recebimento do número de controle do processo. | ────── | Direcionamento automático do lote de documentos para a caixa de triagem inicial da DIEAP. | SCIPWeb (Módulo Peticionamento) | Recibo de Protocolo Eletrônico emitido. | Código de Obras do DF e Portaria de Análise Digital | Variável (Processamento técnico) | **Arquivo acima de 10 MB** ou em formato comum (PDF); **Ausência de guias de pagamento**. |
| **4. Análise Prévia** | Aguarda a validação formal da documentação submetida. | Visualização do status do processo: "Em Análise Prévia". | ────── | Verificação obrigatória através da **Lista de Verificação do SCIP** (Formato, taxas e assinaturas). | Módulo de Triagem do DESEGWEB | Lista de Verificação preenchida salva no histórico. | Portaria de Análise Digital do CBMDF | **Até 3 dias úteis** (Taxativo) | Rejeição imediata por **omissão de memoriais de cálculo** ou erros formais. |
| **5. Exame Técnico** | Acompanha a avaliação minuciosa das instalações preventivas. | Visualização do status do processo: "Em Análise pelo AGFP". | ────── | O **Agente Fiscalizador de Projetos (AGFP)** confere cálculos hidráulicos, lotação e rotas de fuga no DWF. | DESEGWEB e Visualizador DWF de Engenharia | Registro eletrônico do AGFP responsável vinculado ao processo. | ABNT NBR 9077, NBR 13714 e ITs do CBMDF | **15 dias úteis** (Prorrogável por +15 dias) | **Subjetividade ou divergência de interpretação** normativa entre AGPFs; Erros nas justificativas das exigências. |
| **6. Rota de Escape (Recurso)** | Interpõe recurso formal contra exigência considerada indevida pelo projetista. | Tela de peticionamento de recurso e acompanhamento de pauta. | ────── | Avaliação e deliberação técnica colegiada pelo **Conselho Técnico da DIEAP**. | Módulo de Recursos do DESEGWEB | Ata de Deliberação do Conselho Técnico em PDF. | Regimento Interno da DIEAP / DESEG | **Até 10 dias úteis** para julgamento colegiado | **Erros na condução do recurso** por falhas na fundamentação da contestação do usuário. |
| **7. Correção de Projeto** | Corrige as pranchas em DWF e os memoriais de cálculo e faz o reenvio dos arquivos. | Download do relatório de comunique-se e re-upload dos arquivos revisados. | ────── | Recebimento dos arquivos modificados e checagem do cumprimento estrito dos itens apontados. | SCIPWeb, DESEGWEB | Relatório de Exigências Técnicas emitido com assinatura digital. | Lei de Processo Administrativo | **Até 30 dias corridos** para o usuário responder; **15 dias úteis** se pós-Conselho | **Cancelamento definitivo do serviço** por não atendimento reiterado ou decurso de prazo. |
| **8. Emissão e Conclusão** | Efetua o download dos documentos de aprovação certificados com segurança digital. | Links de download habilitados no painel do usuário do SCIPWeb. | ────── | Homologação final pela chefia da DIEAP e aplicação automática de assinaturas e marcas. | Sistema Assinador e Emissor de QR Code da DESEG | Parecer Técnico Conclusivo e Pranchas com Selo Digital e QR Code. | Lei da Liberdade Econômica (13.874/2019) | Imediato após a liberação da chefia | Falha eletrônica na renderização do QR Code ou quebra na assinatura digital do arquivo. |

---

## ETAPA 8 — GRAU DE CONFIANÇA E VALIDAÇÃO DA PESQUISA

Para garantir a precisão metodológica necessária na transposição desta pesquisa para o modelo visual do blueprint, os níveis de certeza das informações coletadas foram recalibrados:

*   **Prazos Legais, Formato DWF e Etapa de Análise Prévia (Alta Confiança):** Informações totalmente alinhadas à Portaria de Análise Digital do CBMDF e à Carta de Serviços oficiais do órgão. Fatos administrativos consolidados.
*   **Fluxo de Isenção de Taxas e Recursos do Conselho Técnico (Média Confiança):** Estrutura procedimental amparada na legislação, mas que necessita de validação qualitativa em campo para mapear como os desvios de fluxo afetam a velocidade de processamento interna.
*   **Tempos Reais de Homologação de Cadastro e Homologação de Chefias (Baixa Confiança / Hipótese a Validar):** Marcados explicitamente como lacuna de dados. Demanda a realização de uma entrevista estruturada com o chefe da DIEAP e equipe de suporte de TI da DESEG para precisar a volumetria e gargalos humanos de liberação de perfis.
