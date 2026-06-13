# Pesquisa para Construção de Service Blueprint AS-IS
## Serviço: Solicitação de Análise de Projetos de Novos Edifícios para Habite-se no Distrito Federal (CBMDF)

---

## ETAPA 1 — MAPEAMENTO DA JORNADA DO CIDADÃO

A jornada do usuário (responsável técnico — engenheiro ou arquiteto) é realizada de forma digital por meio do sistema **SCIP / SCIPWeb** (Gerenciamento do Sistema de Segurança Contra Incêndio e Pânico da Diretoria de Serviços Técnicos - DIEAP/DESEG).

```
[ Jornada do Usuário: Habilitação/Acesso ] ──> [ Entrada do Processo/Upload ] ──> [ Análise Técnico/Correções ] ──> [ Emissão/Retirada do Parecer ]
```

### Fase 1: Preparação e Entrada

#### 1. Consulta de Requisitos e Normativas
* **Objetivo do Usuário:** Compreender quais critérios técnicos, taxas e documentos são necessários para aprovar o projeto da edificação específica.
* **Ação Realizada:** Acesso ao site oficial do CBMDF (DESEG), download de Instruções Técnicas (ITs), Normas Técnicas (NTs) e checagem de tabelas de classificação de risco.
* **Canal Utilizado:** Portal Web do CBMDF / Seção da DESEG.
* **Informações Fornecidas / Documentos:** Consulta pública; nenhuma informação é inserida nesta etapa.
* **Decisões / Dúvidas:** Qual a classificação de carga de incêndio da edificação? Quais medidas de segurança (hidrantes, chuveiros automáticos, saídas de emergência) são obrigatórias?
* **Tempo de Espera:** Imediato (autoatendimento).
* **Dependências Externas:** Nenhuma.
* **Entradas:** Necessidade do cliente; **Saídas:** Conhecimento técnico dos requisitos aplicáveis.
* **Evidências Geradas:** PDFs de normas baixados.
* **Emoções/Frustrações:** Ansiedade devido à complexidade interpretativa do arcabouço normativo do CBMDF.

#### 2. Autenticação e Cadastro no Sistema
* **Objetivo do Usuário:** Obter acesso seguro e personalizado ao sistema SCIPWeb.
* **Ação Realizada:** Login utilizando credenciais cadastradas ou integração com a plataforma Gov.br (padrão de Governo Digital).
* **Canal Utilizado:** Interface de Login do SCIPWeb / DESEGWEB.
* **Informações Fornecidas:** CPF/CNPJ, registro profissional (CREA/CAU), e-mail e senha.
* **Documentos Anexados:** Carteira do Conselho Profissional (em cadastros novos).
* **Decisões / Dúvidas:** O sistema reconhecerá o registro profissional ativo?
* **Tempo de Espera:** Instantâneo se cadastrado; até 48h úteis se necessitar de validação manual de perfil pela administração do sistema.
* **Dependências Externas:** Integração Gov.br e APIs de conselhos de classe (CREA/CAU) para validação de regularidade profissional.
* **Entradas:** Dados do profissional; **Saídas:** Perfil de usuário ativo.
* **Evidências Geradas:** Tela inicial do painel (Dashboard) do solicitante.
* **Emoções/Frustrações:** Frustração se houver lentidão na validação de tokens ou se o sistema apresentar indisponibilidade de banco de dados.

#### 3. Formalização da Solicitação e Upload de Projetos
* **Objetivo do Usuário:** Protocolar formalmente o projeto arquitetônico e de segurança contra incêndio para obter o Parecer Técnico.
* **Ação Realizada:** Preenchimento do formulário eletrônico de características da edificação (área construída, altura, ocupação), upload das pranchas de projeto em formato digital específico (geralmente PDF assinado digitalmente), e anexação de termos de responsabilidade.
* **Canal Utilizado:** Módulo de Peticionamento do SCIPWeb.
* **Informações Fornecidas:** Dados do proprietário, endereço da obra, parâmetros estruturais e técnicos.
* **Documentos Anexados:** Pranchas do Projeto de Incêndio (com convenções de cores normatizadas), Anotação/Registro de Responsabilidade Técnica (ART/RRT) de projeto, e comprovante de recolhimento de taxa (caso aplicável/gerada pelo sistema).
* **Decisões / Dúvidas:** Os arquivos estão no tamanho e formato corretos exigidos pelo sistema para não corromper o upload?
* **Tempo de Espera:** Tempo de processamento do upload dos arquivos pesados.
* **Dependências Externas:** Sistema bancário para compensação da taxa de análise (se houver ônus).
* **Entradas:** Arquivos digitais e metadados; **Saídas:** Número de Protocolo/Processo gerado.
* **Evidências Geradas:** Comprovante de Protocolo Eletrônico com número de controle/processo.
* **Emoções/Frustrações:** Medo de errar no preenchimento de campos rígidos que travem o andamento do processo.

---

### Fase 2: Tramitação e Avaliação

#### 4. Acompanhamento do Processo e Atendimento de Exigências
* **Objetivo do Usuário:** Monitorar o status da análise e corrigir eventuais inconformidades apontadas pelo analista do CBMDF.
* **Ação Realizada:** Consulta periódica ao painel do SCIPWeb para verificar se o status mudou de "Em Análise" para "Com Exigência" ou "Aprovado". Em caso de exigência, o usuário faz o download do relatório de comunique-se/notificação, corrige as pranchas ou documentos e realiza o reenvio.
* **Canal Utilizado:** Módulo de Acompanhamento do SCIPWeb; notificações via e-mail corporativo.
* **Informações Fornecidas:** Correções textuais e justificativas técnicas sobre os pontos contestados.
* **Documentos Anexados:** Pranchas de projeto revisadas e respostas formais aos itens da exigência.
* **Decisões / Dúvidas:** A interpretação do analista sobre a norma é idêntica à minha? Devo contestar formalmente a exigência?
* **Tempo de Espera:** Depende do prazo interno de análise da DIEAP (pode variar de dias a semanas a depender do volume de demanda). O usuário geralmente possui prazo fixo (ex: 30 dias) para responder sob pena de arquivamento.
* **Dependências Externas:** Nenhuma (interação direta Usuário-CBMDF).
* **Entradas:** Notificação de exigência; **Saídas:** Resposta de exigência protocolada.
* **Evidências Geradas:** Relatório de Exigências Técnicas (Comunique-se), Histórico de trâmite interno visível na tela.
* **Emoções/Frustrações:** Alto nível de estresse e irritação caso as exigências sejam consideradas subjetivas ou redundantes (retrabalho).

---

### Fase 3: Conclusão e Entrega

#### 5. Recebimento de Resultados e Emissão de Documentos
* **Objetivo do Usuário:** Obter as pranchas carimbadas digitalmente e o Parecer Técnico de Aprovação para subsidiar a emissão da Carta de Habite-se junto à Administração Regional correspondente.
* **Ação Realizada:** Download dos arquivos finais validados pelo CBMDF.
* **Canal Utilizado:** Módulo de Downloads / Certidões do SCIPWeb.
* **Informações Fornecidas:** Nenhuma (etapa de consumo).
* **Documentos Anexados:** Nenhum.
* **Decisões / Dúvidas:** O documento emitido possui todos os dados idênticos aos da Administração Regional para evitar entraves no Habite-se?
* **Tempo de Espera:** Imediato após a assinatura digital do chefe da seção/analista.
* **Dependências Externas:** Sistemas de validação de assinaturas digitais (ICP-Brasil / ITI).
* **Entradas:** Aprovação do sistema; **Saídas:** Parecer Técnico e Pranchas Certificadas com QR Code.
* **Evidências Geradas:** Parecer Técnico Conclusivo, Pranchas com chancela digital e QR Code impresso no corpo do documento.
* **Emoções/Frustrações:** Alívio, satisfação e sensação de segurança jurídica.

---

## ETAPA 2 — PROCESSOS DE BASTIDOR (BACKSTAGE)

O fluxo de trabalho interno do CBMDF ocorre fora da visão direta do cidadão, envolvendo triagem, distribuição, análise técnica detalhada e instâncias de controle de qualidade.

```
[ Entrada via SCIP ] ──> [ Triagem Administrativa ] ──> [ Distribuição por Complexidade ] ──> [ Análise Técnica (DIEAP) ] ──> [ Revisão/Chefia ] ──> [ Assinatura e Liberação ]
```

### 1. Triagem Administrativa e Distribuição Eletrônica
* **Responsável:** Setor Administrativo / Protocolo da DIEAP (Divisão de Exame e Aprovação de Projetos) da DESEG.
* **Objetivo:** Verificar a conformidade documental inicial (se a taxa foi compensada, se as ARTs estão assinadas, se os arquivos estão corrompidos) antes de enviar para a fila de análise técnica.
* **Sistemas Utilizados:** Retaguarda do SCIP / DESEGWEB.
* **Regras Aplicadas / Critérios:** O processo só avança se a documentação obrigatória mínima estiver presente. Se faltar documento essencial, o processo é rejeitado de plano (reprovação administrativa).
* **Encaminhamentos:** Distribuição automatizada ou manual por sorteio/complexidade para a carga dos analistas de projetos (oficiais ou praças habilitados).

### 2. Análise Técnica Qualificada (Corte Técnico)
* **Responsável:** Analista Técnico de Projetos (Engenheiro Militar / Técnico de Prevenção da DIEAP).
* **Objetivo:** Avaliar minuciosamente se os projetos arquitetônicos e de instalações preventivas cumprem rigorosamente as Normas Técnicas e regulamentos de segurança contra incêndio e pânico vigentes no DF.
* **Sistemas Utilizados:** Módulo de Análise do DESEGWEB, visualizadores de PDF avançados com ferramentas de medição e anotação digital.
* **Regras Aplicadas & Critérios de Aprovação/Reprovação:**
    * *Aprovação:* Total consonância com o Regulamento de Segurança Contra Incêndio e Pânico do DF (RSIP-DF) e Instruções Técnicas correspondentes (dimensionamento de saídas, rotas de fuga, pressurização de escadas, posicionamento de hidrantes).
    * *Reprovação/Exigência:* Divergência de cálculo de lotação, subdimensionamento de equipamentos, ausência de detalhes técnicos obrigatórios.
* **Controle de Qualidade:** O analista redige um relatório pormenorizado vinculando cada inconformidade ao respectivo item normativo violado (vedada a exigência puramente discricionária ou sem amparo legal).

### 3. Revisão de Chefia, Assinatura Digital e Certificação
* **Responsável:** Chefe da DIEAP / Diretor da DESEG.
* **Objetivo:** Homologar a análise executada pelo analista e aplicar a fé pública institucional ao ato administrativo de aprovação.
* **Sistemas Utilizados:** Módulo de Assinatura Digital do SCIPWeb integrado a certificados digitais padrão ICP-Brasil.
* **Regras Aplicadas:** Verificação de conformidade do parecer final. O chefe possui poder de avocação e revisão se provocado por recurso do usuário.
* **Automação vs. Ação Humana:**
    * *Automatizado:* Geração do QR Code exclusivo de validação, aplicação do carimbo digital padronizado em todas as folhas do projeto, disparo de e-mails automáticos de conclusão.
    * *Análise Humana:* A aferição técnica das distâncias de caminhamento, cálculos hidráulicos e locação de riscos é 100% dependente da capacidade cognitiva especializada do analista humano.
    * *Decisão Discricionária:* Reduzida ao mínimo. O serviço público de segurança contra incêndio é estritamente vinculado à legalidade estrita e normas de engenharia. A discricionariedade ocorre apenas na concessão de prazos adicionais ou na aceitação de soluções de engenharia alternativas (comissões técnicas) para prédio históricos ou de geometria complexa.

---

## ETAPA 3 — EVIDÊNCIAS FÍSICAS E DIGITAIS

| Evidência Digital / Física | Etapa de Aparição na Jornada | Quem Gera | Finalidade Operacional | Valor Percebido pelo Usuário |
| :--- | :--- | :--- | :--- | :--- |
| **Interface do Dashboard do SCIP** | Login e Acompanhamento | Sistema (Automático) | Centralizar solicitações e mostrar o status atualizado do processo. | Transparência e controle do andamento das demandas em tempo real. |
| **Comprovante de Protocolo e Número de Processo** | Upload de Projetos | Sistema (Automático) | Servir como recibo legal de que o cidadão protocolou o pedido na data X. | Segurança jurídica e comprovação de cumprimento de prazos. |
| **Relatório de Exigências Técnicas (Comunique-se)** | Atendimento de Exigências | Analista da DIEAP | Apontar erros no projeto e fundamentar legalmente o que deve ser corrigido. | Clareza sobre o que precisa ser alterado para obter a aprovação. |
| **Parecer Técnico Conclusivo de Aprovação** | Recebimento de Resultados | Chefe da DIEAP | Declarar formalmente que a edificação cumpre as normas de segurança. | Documento oficial essencial para obter o Habite-se com o GDF. |
| **Pranchas de Projeto com Chancela Digital e QR Code** | Recebimento de Resultados | Sistema integrado com Assinador | Autenticar cada página do projeto arquitetônico aprovado. | Garantia de intangibilidade do projeto; facilidade de verificação em campo via smartphone. |

---

## ETAPA 4 — LEVANTAMENTO NORMATIVO

O serviço é rigidamente regulado por um ecossistema normativo que vai da legislação de desburocratização digital às regras técnicas de engenharia de incêndio.

### 1. Legislação Federal e Governo Digital
* **Lei Federal nº 14.129/2021 (Lei do Governo Digital):** Dispõe sobre princípios, regras e instrumentos para o Governo Digital e para a eficiência pública, incentivando a desmaterialização de processos.
* **Lei Federal nº 13.874/2019 (Lei da Liberdade Econômica):** Estabelece garantias de livre mercado e a classificação de atividades de risco para fins de licenciamento.

### 2. Legislação do Distrito Federal
* **Decreto Distrital nº 42.502/2021 (Regulamenta o RSIP-DF):** Regulamenta a segurança contra incêndio e pânico no DF, definindo as competências do CBMDF no tocante à análise de projetos e vistorias para Habite-se.
* **Lei Distrital nº 6.138/2018 (Código de Obras do Distrito Federal):** Regula toda atividade de obras no DF, condicionando a Carta de Habite-se à anuência do CBMDF.

### 3. Normativos e Instruções Técnicas do CBMDF
* **Portarias da DESEG/CBMDF e Instruções Técnicas (ITs):** Conjunto de dezenas de instruções que detalham as especificidades técnicas por sistema (ex: IT 11 - Saídas de Emergência, IT 22 - Hidrantes, etc.).

---

## ETAPA 5 — FAIL POINTS (PONTOS DE FALHA)

Abaixo estão descritos os principais gargalos e vulnerabilidades operacionais identificados na prestação do serviço atual.

* **Falhas do Usuário:** Upload de arquivos fora dos padrões de nomenclatura ou tamanho; incompatibilidade geométrica ou erros de cálculo de dimensionamento normativo.
* **Falhas Sistêmicas:** Instabilidade de infraestrutura ou lentidão em horários de pico; falhas na integração com bases externas (Gov.br ou CREA/CAU).
* **Falhas Operacionais e Institucionais:** Subjetividade ou divergência interpretativa entre analistas da DIEAP, gerando múltiplas exigências contraditórias ("comunique-se infinito").

---

## ETAPA 6 — SISTEMAS E INTEGRAÇÕES

1.  **SCIPWeb / DESEGWEB:** Portal transacional de relacionamento com o cidadão e workflow interno dos militares da DESEG/DIEAP.
2.  **Módulo Assinador Digital do CBMDF:** Aplica chancelas eletrônicas criptográficas baseadas em certificados ICP-Brasil (A3/A1) nos pareceres e pranchas.
3.  **Gerador de QR Code Institucional:** Cria uma assinatura visual rastreável ligada à URL de autenticidade da DESEG.

---

## ETAPA 7 — MATRIZ SERVICE BLUEPRINT (AS-IS)

| Etapa da Jornada | Ação do Usuário | Frontstage (Interações Visíveis) | Linha de Visibilidade | Backstage (Processos Internos) | Sistemas Envolvidos | Evidência Física/Digital | Normativos Aplicáveis | Tempo de Espera Est. | Fail Points Críticos |
| :--- | :--- | :--- | :---: | :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Preparação** | Acessa o site e lê as normas técnicas de incêndio. | Consulta ao menu público da DESEG no portal. | ────── | Atualização e upload das normas no portal pelo setor técnico. | Portal do CBMDF / Servidor Web | PDFs das Instruções Técnicas (ITs). | Decreto Distrital 42.502/2021 | Imediato (Autoatendimento) | Dificuldade de localização de normas atualizadas. |
| **2. Cadastro e Acesso** | Realiza login via Gov.br e valida dados profissionais. | Tela de login do SCIPWeb e campos de perfil. | ────── | Validação automática ou manual de perfis pendentes de profissionais. | SCIPWeb, API Gov.br, Banco de Dados CREA/CAU | Dashboard inicial do usuário logado. | Lei do Governo Digital (14.129) | Instantâneo a 48h (se manual) | Erro na validação de tokens de segurança. |
| **3. Protocolização** | Preenche dados da edificação e faz upload do projeto. | Formulário eletrônico de peticionamento de análise. | ────── | Recepção digital do lote de arquivos e armazenamento em nuvem/servidor. | SCIPWeb (Módulo Peticionamento) | Comprovante de Protocolo Eletrônico com número. | Código de Obras do DF (Lei 6.138) | Variável | Queda de conexão com arquivos pesados; rejeição de formato. |
| **4. Triagem** | Aguarda movimentação do processo no sistema. | Visualização do status "Aguardando Distribuição". | ────── | Verificação de conformidade de documentos obrigatórios e taxas. | DESEGWEB (Módulo de Gestão Interna) | Histórico de trâmites atualizado na tela. | Regulamento Interno da DESEG | 1 a 5 dias úteis | Atraso na compensação bancária das taxas; erro de triagem. |
| **5. Avaliação Técnica** | Monitora o andamento do processo técnico. | Visualização do status "Em Análise Técnica". | ────── | Analista examina cálculos, layout de rotas de fuga e locação de equipamentos. | DESEGWEB, Ferramentas de Visualização de Pranchas | Registro do analista responsável atribuído ao caso. | Instruções Técnicas (ITs) do CBMDF e ABNT | Dias a semanas (conforme fila da DIEAP) | **Subjetividade / Divergência de interpretação** entre analistas. |
| **6. Correção (se houver)** | Baixa o relatório de exigências e reenvia o projeto corrigido. | Download do documento de Comunique-se; reenvio de arquivos. | ────── | Emissão das inconformidades e posterior checagem do reenvio. | SCIPWeb, DESEGWEB | Relatório de Exigências Técnicas em PDF. | Lei de Processo Administrativo | Prazo fixo concedido ao usuário (ex: 30 dias) | **"Comunique-se Infinito"**: Novas exigências feitas tardiamente. |
| **7. Finalização** | Faz o download dos documentos chancelados aprovados. | Clique no link de download do parecer e pranchas. | ────── | Homologação pela Chefia, aplicação automática do QR Code e assinatura ICP. | SCIPWeb, Assinador Digital, Gerador de QR Code | Parecer Técnico de Aprovação e Pranchas com QR Code. | Lei da Liberdade Econômica (13.874) | Imediato após assinatura final | Erro na renderização do QR Code ou corrupção do documento assinado. |

---

## ETAPA 8 — GRAU DE CONFIANÇA E VALIDAÇÃO

1. **Fluxo do SCIPWeb e Mecanismos de Upload (Alta Confiança):** Baseado nos manuais oficiais disponibilizados na página da DESEG/CBMDF.
2. **Tempo de Espera e Fila de Análise Técnica (Média Confiança / Hipótese a Validar):** Os tempos médios variam sazonalmente. Requer validação de dados históricos junto ao CBMDF.
3. **Divergências Interpretativas entre Analistas (Média Confiança / Hipótese a Validar):** Relatado frequentemente por engenheiros e arquitetos (dores do usuário). Deve ser confrontado em entrevista com os oficiais analistas da DIEAP.
