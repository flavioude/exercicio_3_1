## Diagrama AS-IS — Análise de PSCIP (Obra Inicial) para Habite-se no DF

```mermaid
flowchart LR
  subgraph Cidadao [Cidadão / Responsável Técnico]
    C1[1. Consulta ITs e classifica risco]
    C2[2. Cadastro e dados da edificação]
    C3[3. Upload DWF + ART/RRT/TRT + taxa]
    C7[7. Corrige e reenvia projeto]
    C8[8. Baixa Parecer e pranchas certificadas]
  end

  subgraph SCIPWeb [SCIPWeb - Frontstage]
    S2[Formulário de cadastro]
    S3[Protocolo eletrônico]
    S5[Painel de status]
    S8[Módulo de Downloads/Certidões]
  end

  subgraph DIEAP [DIEAP / DESEG - Backstage]
    B4[4. Análise Prévia - Lista de Verificação]
    B5[5. Exame técnico do AGFP]
    B7[Recepção da correção e checagem de itens]
    B8[Homologação e chancela ICP-Brasil/QR Code]
  end

  subgraph CTDSCI [CTDSCI - instância condicional]
    B6[6. Deliberação do Colegiado]
  end

  subgraph Suporte [Processos de Suporte]
    Sup1[(DESEGWEB)]
    Sup2[(Assinador ICP-Brasil / QR Code)]
  end

  C1 --> C2 --> S2 --> C3 --> S3 --> B4

  B4 -->|conforme| B5
  B4 -.->|⚠ Fail point: DWF fora do padrão / ART-RRT ausente| C7

  B5 -->|aprovado| B8
  B5 -.->|exigência técnica| C7
  B5 -.->|caso omisso / solução alternativa| B6

  B6 -->|deferido c/ condicionantes| C7
  B6 -.->|⚠ Fail point: indeferido| F6[/Retorno ao fluxo padrão sem flexibilização/]

  C7 -.->|reenvio - revalida| B4
  C7 -.->|reenvio - revalida| B5
  C7 -.->|⚠ Fail point: reincidência em 2 retornos| F7[/Cancelamento definitivo do processo/]

  B8 --> S8 --> C8
  S5 -.-> C2
  S5 -.-> C3

  B4 -.-> Sup1
  B5 -.-> Sup1
  B8 -.-> Sup2

  classDef failpoint fill:#fdd,stroke:#c00,color:#900,stroke-width:1px;
  classDef condicional stroke-dasharray: 4 2;
  class F6,F7 failpoint;
  class CTDSCI condicional;
```

**Legenda:**
- Setas sólidas (`-->`): fluxo principal da jornada (1 → 2 → 3 → 4 → 5 → 8).
- Setas tracejadas (`-.->`): fluxos condicionais/iterativos (correção, encaminhamento ao CTDSCI) e interações com sistemas de suporte/painel de status.
- Nós vermelhos (`⚠`): fail points que interrompem ou revertem a jornada (devolução, indeferimento, cancelamento).
- *Subgraphs*: representam os atores/camadas — Cidadão (Ações do Cidadão), SCIPWeb (Frontstage), DIEAP/DESEG (Backstage), CTDSCI (instância condicional) e Processos de Suporte.
