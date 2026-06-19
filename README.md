# Caderno Temático de Aprendizagem: Fundamentos de Engenharia de Prompts com NotebookLM

## Contexto e Diretrizes do Projeto
Este repositório documenta a execução do projeto prático proposto no Bootcamp da DIO. O objetivo deste trabalho é consolidar o entendimento prático sobre a dinâmica de comunicação com Modelos de Linguagem (LLMs), utilizando o **NotebookLM (Google)** como ambiente de curadoria de conhecimento e testes de eficácia de instruções.

A abordagem adotada prioriza a aplicação da Inteligência Artificial como ferramenta de produtividade e otimização de fluxos informacionais, avaliando como o refinamento de comandos (Engenharia de Prompts) impacta diretamente a governança e a precisão das respostas geradas.

---

## Curadoria de Fontes e Base de Dados
Para fundamentar os testes com dados de alta credibilidade e evitar inconsistências teóricas, a base de conhecimento do NotebookLM foi alimentada com as seguintes documentações de referência do mercado:
1. **Diretrizes Oficiais de Prompting da OpenAI:** Análise de estratégias para o desenvolvimento de instruções claras e divisão de tarefas complexas.
2. **Guias de Contextualização da Google DeepMind:** Princípios técnicos para a estruturação de cenários e parametrização de respostas em modelos avançados, e outras fontes confiáveis.

---

## Avaliação Prática e Validação de Instruções (Troubleshooting)

A validação dos conceitos teóricos apresentados nas aulas foi realizada por meio de testes comparativos no ambiente do NotebookLM, analisando o comportamento do modelo diante de diferentes níveis de clareza instrucional:

### Abordagem 1: Prompt de Escopo Aberto (Inconsistente)
*   **Comando Aplicado:** *"Me explica como fazer um prompt bom."*
*   **Comportamento do Modelo:** Retornou uma resposta de alta volumetria textual, genérica e de difícil aplicação prática.
*   **Análise Crítica:** A ausência de delimitações e de um papel de atuação permitiu que o modelo operasse em um espectro probabilístico muito amplo, gerando desperdício de tempo operacional e redundâncias.

### Abordagem 2: Prompt Estruturado com Restrições (Eficiente)
*   **Comando Aplicado:** *"Atue como um Especialista em Processos Corporativos. Com base exclusivamente nas fontes do canal de Engenharia de Prompts fornecidas, crie uma lista em tópicos com as 3 principais regras para evitar que um modelo de IA cometa erros em relatórios de negócios. Seja objetivo."*
*   **Comportamento do Modelo:** Entrega precisa, curta, restrita estritamente aos documentos fornecidos e sem desvios conceituais.
*   **Análise Crítica:** A imposição de barreiras (*Guardrails*) e a definição clara do formato de saída demonstraram que a previsibilidade e a utilidade da IA são diretamente proporcionais à qualidade técnica da instrução inserida.

---

## Consolidação Técnica (Entrega Final)

### 1. Resumo Estruturado dos Fundamentos
*   **Processamento de Linguagem:** Os modelos de IA operam por meio da quebra de texto em unidades numéricas denominadas *tokens* (sílabas ou fragmentos de palavras), prevendo estatisticamente a próxima palavra mais provável com base nos padrões do treinamento original.
*   **Mecânica da Janela de Contexto:** Refere-se à capacidade limite de memória de trabalho do modelo em uma mesma sessão. Quando o volume de dados da conversa excede o limite de *tokens* suportado, ocorre o descarte progressivo do histórico mais antigo para a manutenção do processamento atual.
*   **Estrutura de Alta Performance:** Um prompt eficiente exige a combinação sinérgica de elementos essenciais: atribuição de papel (persona), contextualização do cenário, definição clara da tarefa, aplicação de restrições de escopo e especificação rigorosa do formato de saída.

### 2. Glossário de Termos Técnicos
*   **Prompt Engineering:** Prática de projetar, refinar e otimizar instruções em linguagem natural para direcionar o comportamento de sistemas de IA.
*   **Guardrails:** Parâmetros ou limitações explícitas embutidas no comando para assegurar a conformidade, manter o tom corporativo e mitigar o risco de alucinações (fatos inventados).
*   **Few-shot Learning:** Técnica de inserção de pares de exemplos (entrada/saída esperada) no corpo do prompt para acelerar a curva de aprendizado do modelo por replicação de padrão.
*   **Chain of Thought:** Estratégia de indução lógica que força o modelo a externalizar o raciocínio sequencial passo a passo antes de apresentar a conclusão final, aumentando a assertividade.

### 3. Matriz de Prompts Reutilizáveis para Aplicação Futura
*   *Sintetização de Textos Técnicos:*
    > "Atue como um Analista de Negócios. Reduza o documento técnico inserido abaixo a um resumo executivo de 3 parágrafos, focando exclusivamente nos impactos operacionais e pontos-chave: [Inserir Texto]"
*   *Análise de Cenário - Ecossistema SAP SD (Foco de Interesse):*
    > "Atue como um Consultor Funcional SAP SD Sênior. Explique de maneira analítica e sequencial as dependências e o impacto do fluxo de 'Ordem de Venda' (Sales Order) na etapa de faturamento e geração de nota fiscal: [Inserir Dúvida ou Cenário]"
