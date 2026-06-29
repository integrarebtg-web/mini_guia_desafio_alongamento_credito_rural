# mini_guia_desafio_alongamento_credito_rural
# 🌾 Miniguia de Estudos: Alongamento de Dívidas Rurais com Inteligência Artificial
> **Projeto Prático - Desafio de Aprendizagem Ativa da Digital Innovation One (DIO)**

![Status do Projeto](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)
![Categoria](https://img.shields.io/badge/Segmento-Agroneg%C3%B3cio%20%2F%20TI-orange)
![Tecnologias](https://img.shields.io/badge/IA-Google%20NotebookLM%20%7C%20Python-blue)

---

## 🎯 1. Contexto e Objetivos Estruturados

### Contexto Profissional
O autor deste projeto atua como **perito judicial especialista em finanças e agronegócio** e encontra-se em um momento estratégico de **transição de carreira para a área de Tecnologia da Informação (TI)**, focando em automação com Inteligência Artificial. 

O agronegócio é o principal motor econômico do Brasil. A complexidade regulatória e financeira do setor gera uma demanda latente por soluções tecnológicas que garantam segurança jurídica e financeira aos produtores rurais e empresas do ecossistema AGRO.

### Objetivos do Caderno Temático
* **Objetivo Geral:** Construir um Caderno Temático inteligente utilizando o **Google NotebookLM** para consolidar o entendimento sobre os mecanismos legais, regulatórios e jurisprudenciais do alongamento de dívidas rurais no cenário econômico de 2026.
* **Objetivos Específicos:**
    * **Engenharia de Prompts:** Dominar técnicas avançadas de comandos para interagir com modelos de linguagem (LLMs) de forma analítica e consultiva, mitigando alucinações em textos jurídicos e normativos de alta complexidade.
    * **Mapeamento Regulatório:** Mapear os requisitos formais de elegibilidade e os fluxos procedimentais de renegociação de crédito rural controlados pelo Manual de Crédito Rural (MCR) e resoluções do Banco Central do Brasil (BACEN).
    * **Lógica de Automação:** Estruturar as regras de negócios extraídas dos julgados e normativas em tópicos lógicos descritivos, servindo de base para o desenvolvimento futuro de sistemas automatizados de triagem (scripts em Python/LangChain).

---

## 📋 2. Diretrizes do Desafio (DIO)

Este repositório cumpre integralmente os requisitos de entrega exigidos na plataforma da DIO para a validação do projeto "Nota 10":
1. **Contexto e Objetivos:** Delimitação clara do tema escolhido e aplicabilidade no mercado de trabalho.
2. **Curadoria de Fontes:** Seleção rigorosa de materiais públicos para alimentação da base de conhecimento da IA (RAG).
3. **Engenharia de Prompts e "Cicatrizes":** Documentação detalhada dos testes de comandos e do processo de *troubleshooting*.
4. **Miniguia de Estudo:** Consolidação do conhecimento em resumos, glossário estruturado em tabela e prompts reutilizáveis.

---

## 📚 3. Curadoria de Fontes Base (Upload NotebookLM)

Para mitigar alucinações e blindar o conhecimento do Caderno Temático, foram selecionadas as seguintes fontes normativas e doutrinárias:

* 📄 **Manual de Crédito Rural (MCR) - Banco Central do Brasil:** Base regulatória oficial contendo as seções de Condições Básicas, Orçamentos e Fiscalização (MCR 2-6-4).
* 📄 **Resolução CMN nº 5.220/2025 (CMN/BACEN):** Nova normativa que flexibilizou as regras para renegociação do custeio rural e ritos de extemporaneidade.
* 📄 **Resolução CMN nº 5.314/2026 (CMN/BACEN):** Fato novo regulatório que alterou o rito do alongamento compulsório incluindo o termo "por sua conveniência e decisão".
* 📄 **Jurisprudência Vinculante - Súmula 298 do Superior Tribunal de Justiça (STJ):** Enunciado que define o alongamento do crédito rural como direito do devedor.
* 📄 **Precedente Jurisprudencial de 2026 - Tribunal de Justiça de Minas Gerais:** Acórdão da 10ª Câmara Cível (Apelação Cível nº 1.0000.24.345628-2/002) versando sobre a tempestividade do rito administrativo.

---

## 🧠 4. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

### 🔄 Bloco 1: Do Prompt Genérico ao Prompt Especialista

#### ❌ Prompt 1 (Abordagem Inicial - Baixa Previsibilidade)
```text
"Como funciona o alongamento de dívida rural segundo o Manual do Banco Central?"

---
Resultado da IA: O NotebookLM gerou uma resposta estruturada detalhando os pilares do MCR 2-6-4. Contudo, a resposta dependeu exclusivamente do contexto estrito dos arquivos carregados no caderno. Em um modelo de linguagem aberto (sem fontes anexadas), um comando genérico como este costuma retornar conceitos superficiais do Direito Civil comum (renegociação bancária padrão), deixando de isolar o microssistema do Crédito Rural e ignorando as nuances regulatórias recentes de 2026.

Troubleshooting (A "Cicatriz" Técnica): O comando pecou pela falta de técnicas de contextualização de escopo e definição de persona. Confiar que a IA trará a resposta certa apenas porque os arquivos estão lá é um risco em ambiente de produção. Em engenharia de software ou automações analíticas, prompts precisam ser determinísticos.

🔄 Prompt 2 (Refinado - Engenharia de Prompt Avançada)
"Atue como um analista de risco de crédito e perito em agronegócio. Com base estritamente no Manual de Crédito Rural (MCR 2-6-4) fornecido nos documentos, identifique quais são os requisitos formais para que um produtor rural solicite a prorrogação de uma dívida de custeio agrícola. Estruture a resposta destacando os fatores de comprovação e a jurisprudência do STJ."

Análise do Ganho Técnico: Ao introduzir uma persona especialista e uma cláusula de barreira restritiva ("com base estritamente..."), o modelo foi blindado. O resultado deixa de ser uma resposta explicativa passiva e passa a ser um parecer técnico-processual. O prompt refinado força a IA a correlacionar os requisitos fáticos (laudos e fluxos de caixa) diretamente com o nexo causal exigido pelos Tribunais e pela Súmula 298 do STJ, gerando o insumo perfeito para desenhar a lógica de uma futura automação.

🏛️ Bloco 2: Prompt Avançado 1 – O Confronto do Fato Novo (Regulatório 2026)
Prompt 3 (Especialista em Conflito Normativo)
"Atue como um Perito Econômico-Financeiro sênior especializado no Agronegócio. Com base estritamente nos documentos fornecidos, analise o impacto da recente Resolução CMN 5.314/2026 (que alterou o MCR para indicar que o banco prorroga 'por sua conveniência e decisão') em face da histórica Súmula 298 do STJ (que define o alongamento como direito subjetivo do devedor). Redija um parecer técnico-financeiro de orientação para um produtor de soja que teve quebra de safra climática comprovada, demonstrando como rebater uma resposta negativa e genérica do banco que utilize a nova resolução como justificativa."

📝 Resolução do Prompt 3 (Parecer Técnico Estruturado)
Contexto do Conflito Regulatório: A Resolução CMN 5.314, publicada em 25 de junho de 2026, alterou a redação do Manual de Crédito Rural (MCR) inserindo o dispositivo de que as instituições de crédito estão autorizadas a proceder ao alongamento "por sua conveniência e decisão". Esta inserção normativa representa um esforço evidente do setor bancário para afastar a natureza compulsória das renegociações. Contudo, a Súmula 298 do STJ permanece plenamente ativa e dita de forma vinculante que o alongamento não constitui faculdade da instituição financeira, mas sim um direito do devedor nos termos da lei.

Tese de Defesa Baseada em Normas de Ordem Pública: O crédito rural opera no Brasil sob o manto de uma política pública nacional. Sendo composto predominantemente por recursos controlados e subsidiados, ele sujeita-se a um rígido dirigismo contratual estatal. Portanto, a "autorização por conveniência" dada pelo BACEN confere poder de análise de risco aos bancos, mas não aval para a prática de arbitrariedades. Diante de um produtor que preenche os requisitos fáticos do MCR 2-6-4, a recusa imotivada ou genérica do agente financeiro configura patente abuso de direito, passível de anulação e imposição judicial compulsória.

O Rigor Probatório do Nexo Causal: Para desarmar a prerrogativa de "conveniência" do banco, a perícia e o parecer de defesa do produtor de soja não podem se limitar a alegações abstratas. É indispensável estruturar o nexo causal com:

Laudo Agronômico Individualizado: Documento assinado por engenheiro agrônomo habilitado comprovando o índice de quebra, a causa climática restrita às coordenadas da lavoura e o percentual exato de perda de renda.

Laudo de Fluxo de Caixa Futuro: Estudo demonstrando o descréscimo econômico imediato e simulando a viabilidade da propriedade rural nos ciclos subsequentes, garantindo que o montante será liquidado no novo cronograma desenhado.

💻 Bloco 3: Prompt Avançado 2 – Lógica e Engenharia de Regras para TI
Prompt 4 (Lógica de Algoritmo para Programação)
"Atue como um Engenheiro de Software especialista em Sistemas de Automação para o Agronegócio. Com base nos manuais, julgados e artigos do caderno de estudos, crie uma Estrutura Lógica de Triagem (Pseudocódigo ou Fluxo de Decisão IF/ELSE) para analisar se uma carteira de clientes de uma cooperativa agropecuária é elegível ou não ao alongamento compulsório de dívida rural. O fluxo deve processar variáveis como Natureza do Débito, Origem dos Recursos, Status do Pedido e Presença de Laudo."

📝 Resolução do Prompt 4 (Pseudocódigo de Regras de Negócio)
---
# Algoritmo de Elegibilidade para Alongamento Compulsório (MCR 2-6-4 / Súmula 298 STJ)
def triagem_alongamento_divida(cliente_cooperado):

    # 1. VERIFICAÇÃO DA NATUREZA DO DÉBITO
    naturezas_elegiveis = ["CUSTEIO", "INVESTIMENTO", "COMERCIALIZACAO"]
    if cliente_cooperado.natureza_debito not in naturezas_elegiveis:
        return "INELEGÍVEL: Natureza da dívida não amparada pelo MCR 2-6-4 (Ex: Compra de terra, Multas, Tributos)"

    # 2. ANÁLISE DA ORIGEM DOS RECURSOS
    # A jurisprudência consolida a obrigatoriedade principalmente para Recursos Controlados
    if cliente_cooperado.origem_recursos != "CONTROLADOS_SNCR":
        # Se for recurso livre, a elegibilidade é subjetiva e depende de negociação comercial
        return "RISCO ALTO: Recursos Livres possuem baixa taxa de êxito judicial para alongamento compulsório"

    # 3. VALIDAÇÃO DO ACERVO TÉCNICO (REQUISITO OBJETIVO)
    # A ausência de prova técnica inviabiliza o direito subjetivo
    if not (cliente_cooperado.possui_laudo_agronomico and cliente_cooperado.possui_laudo_viabilidade):
        return "REPROVADO: Falta de robustez probatória (Laudo Agronômico ou Fluxo de Caixa ausente)"

    # 4. VERIFICAÇÃO DO FATO GERADOR (SINISTRO)
    motivos_legais = ["FRUSTRACAO_SAFRA", "DIFICULDADE_COMERCIALIZACAO", "OCORRENCIA_PREJUDICIAL"]
    if cliente_cooperado.fato_gerador not in motivos_legais:
        return "REPROVADO: Causa da dificuldade não prevista no item 4 da Seção 6 do Cap. 2 do MCR"

    # 5. STATUS DO PEDIDO E TEMPESTIVIDADE
    if cliente_cooperado.status_pedido == "ANTERIOR_AO_VENCIMENTO":
        # Direito subjetivo pleno conforme Súmula 298 STJ e MCR
        cliente_cooperado.score_elegibilidade = 100
        status_final = "ELEGÍVEL: Direito Subjetivo Protegido (Súmula 298 STJ)"

    elif cliente_cooperado.status_pedido == "APOS_VENCIMENTO":
        # Aplicação da flexibilidade trazida pela Resolução CMN 5.220/2025
        cliente_cooperado.score_elegibilidade = 80
        status_final = "ELEGÍVEL: Amparado pela Resolução CMN 5.220/2025 (Prorrogação Extemporânea)"
    else:
        return "REPROVADO: Inexistência de protocolo administrativo de prorrogação"

    # 6. FILTRO DE CONFLITO NORMATIVO (RESOLUÇÃO 5.314/2026)
    # Refuta o argumento de "conveniência e decisão" do banco se os requisitos técnicos acima forem TRUE
    if status_final.startswith("ELEGÍVEL"):
        impor_compulsoriedade = True
        observacao_tecnica = "Refutar negativa genérica baseada na Res. 5.314/2026 via Súmula 298 STJ"
        return f"{status_final} | Ação: Notificar Credor sobre Compulsoriedade do MCR 2-6-4"
        
    return "CONSULTAR DEPARTAMENTO JURÍDICO"
---
📖 5. Miniguia de Estudo (Entrega Final Consolidada)
Resumos Estruturados do Assunto
A Engrenagem da Política Agrícola: O alongamento de crédito rural é um mecanismo protetivo de ordem pública concebido para salvaguardar a capacidade produtiva e a sobrevivência da empresa agrária frente a intempéries sistêmicas involuntárias.

O Roteiro Processual de Rigor: Para afastar os riscos de consolidação de mora, inscrições restritivas em cadastros de inadimplentes e execuções precipitadas de garantias reais, o produtor e seu corpo técnico devem agir com antecipação. O rito exige constatação pericial imediata do sinistro, cálculo pericial de fluxo de caixa, protocolo formal tempestivo perante a agência detentora do crédito e, em caso de recusa arbitrária, propositura ágil de tutela de urgência.
---
### 📕 Glossário de Conceitos Chave

| Termo | Definição Técnico-Jurídica / Pericial | Fonte Regulatória / Jurisprudencial |
| :--- | :--- | :--- |
| **MCR** | Manual de Crédito Rural. O código normativo expedido pelo BACEN que reúne as regras de política de crédito rural do país. | MCR - BACEN |
| **Súmula 298 do STJ** | Enunciado vinculante do Superior Tribunal de Justiça que determina que o alongamento de dívida originada de crédito rural não constitui faculdade da instituição financeira, mas direito do devedor nos termos da lei. | Superior Tribunal de Justiça |
| **Alongamento de Dívida** | Mecanismo político e jurídico para reprogramar o calendário de pagamento da dívida nos casos de comprovada impossibilidade de adimplemento. | MCR 2-6-4 / Súmula 298 STJ |
| **Recursos Controlados** | Linhas de financiamento agrário subsidiadas pelo Tesouro Nacional ou lastreadas em exigibilidades legais (depósitos compulsórios), protegidas pelo microssistema do MCR. | MCR 6-2 / SNCR |
| **Nexo Causal** | A obrigação pericial de comprovar a relação direta de causa e efeito entre a intempérie climática/de mercado e o decréscimo econômico verificado na propriedade. | MCR - Documento 3 (RCP) |
| **Zarc** | Zoneamento Agrícola de Risco Climático. Parâmetro que dita os períodos e regiões de plantio para fins de compliance e cobertura. | Ministério da Agricultura (MAPA) |
| **Resolução CMN 5.220/2025** | Norma que abriu o rito de flexibilidade, permitindo a solicitação de dilação de parcelas mesmo após o vencimento do título. | Conselho Monetário Nacional |
| **Resolução CMN 5.314/2026** | Alteração que inseriu a expressão "por sua conveniência e decisão", originando o atual conflito com o direito subjetivo do produtor. | Conselho Monetário Nacional |
| **Stay Period** | Período de suspensão automática de ações e execuções (180 dias) obtido via blindagem de Recuperação Judicial para produtores rurais. | Lei de Recuperação de Empresas e Falências |
| **Comissão de Permanência** | Encargo moratório considerado ilegal e abusivo quando aplicado em Cédulas de Crédito Rural por ausência de previsão legal. | Decreto-Lei nº 167/67 / STJ |
| **Sicor** | Sistema de Operações do Crédito Rural e do Proagro. Terminal do BACEN onde as instituições registram dados de risco e coordenadas geodésicas. | Banco Central do Brasil |
---

🔄 Prompts Reutilizáveis para Análise e Revisão
💡 Prompt para Auditoria de Cédulas: "Atue como um perito contábil financeiro judicial. Analise esta memória de cálculo de débito rural fornecida pelo banco e verifique se há incidência disfarçada de comissão de permanência, elevação unilateral de juros em aditivos contratuais ou capitalização de juros não contratada, confrontando com as vedações do Decreto-Lei nº 167/1967."

💡 Prompt para Checklist de IA: "Atue como um analista de sistemas. Com base na árvore de decisão de triagem de alongamento do MCR 2-6-4, monte um checklist interativo em formato markdown para auditar se um dossiê encaminhado por um produtor atende aos critérios formais exigidos pelas Câmaras de Direito Privado do TJSP e TJPR."

🛠️ 6. Considerações sobre Transição de Carreira e Automação
Este projeto prova que a transição de carreira para a área de TI potencializada por Inteligência Artificial não exige o descarte da experiência prévia. Ao contrário, o mercado de tecnologia de ponta exige especialistas de domínio (Subject Matter Experts) que saibam o que construir.

Unir a bagagem analítica e jurídica da perícia judicial à engenharia de prompts avançada cria a base perfeita para construir ecossistemas de automação corporativa de alto valor de mercado no ecossistema do Agronegócio brasileiro.
