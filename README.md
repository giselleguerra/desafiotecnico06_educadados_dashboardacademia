# 🏋️‍♂️ Painel de Performance - Gestão de Academias

## 📖 Sobre o projeto
Projeto prático de Análise de Dados desenvolvido como parte da formação da **Educadados**, sob mentoria do professor Felipy. 

O desafio consistiu em analisar os dados brutos de uma rede de academias, buscando compreender o comportamento dos alunos, a frequência de treinos, a receita gerada e, principalmente, identificar e prever riscos de cancelamento (churn) através de regras de negócio avançadas.

A solução proposta é um dashboard executivo de página única (One-Page Dashboard), desenvolvido no Power BI, focado na clareza visual e na tomada de decisão rápida.

## 🎯 Objetivos
- Analisar a sazonalidade e o engajamento real dos alunos.
- Acompanhar a evolução da frequência de treinos ao longo do tempo.
- Analisar a receita segmentada por tipo de plano (Mensal, Trimestral, Anual).
- Identificar de forma automática alunos ativos, inativos e em risco de evasão.
- Facilitar a otimização operacional mapeando horários de pico (superlotação).

## 📊 Escopo do Dashboard

O dashboard foi estruturado para responder às principais perguntas de negócio, contendo:

**KPIs (Indicadores Chave):**
- Total de Alunos
- Receita Total
- Média de Frequência Mensal por Aluno
- Percentual (%) de Alunos Ativos reais

**Visualizações:**
- **Frequência ao longo do tempo:** Gráfico de linhas demonstrando a evolução de acessos.
- **Receita por plano:** Gráfico de barras horizontais.
- **Alunos por status:** Gráfico de rosca detalhando a saúde da base de clientes.
- **Top alunos mais frequentes:** Tabela ranqueada.
- **Heatmap (Mapa de Calor):** Matriz cruzando Dias da Semana x Horários de pico.

**Filtros Dinâmicos:**
- Período (Mês/Ano)
- Unidade (Filtro por filial da academia)

## 🧠 Lógica de Negócio (Destaque DAX)
Para garantir análises precisas, foram aplicadas modelagens e cálculos avançados em DAX. O grande destaque do projeto é a **Regra de Retenção**, que classifica dinamicamente o status de cada aluno com base na sua última visita registrada:

* **Ativo:** Treinou nos últimos 10 dias.
* **Em Risco:** Não treina entre 11 e 30 dias (Janela ideal para atuação do time de Customer Success).
* **Inativo:** Não comparece há mais de 30 dias ou sem registros.

## 🛠️ Tecnologias e Ferramentas
- **Power BI:** Tratamento, modelagem relacional, análise e visualização de dados.
- **Power Query:** Processamento de ETL (Extração, Transformação e Carga).
- **Linguagem DAX:** Criação de medidas inteligência de tempo e regras de negócio.
- **Excel:** Armazenamento e estruturação da base de dados original.
- **Figma:** Criação de layout/visual do dashboard.

## 📁 Organização do Projeto

```
📦 painelPerformance_academia
 ┣ 📜 base_dados_academia.xlsx
 ┣ 📜 telaDesafioDataViz.svg
 ┣ 📜 DesafioModulo06DataViz.pbix
 ┗ 📜 README.md
````
✅ Progresso do Desenvolvimento
[x] Entendimento do problema e regra de negócio

[x] Processo de ETL e tratamento dos dados no Power Query

[x] Modelagem de dados (Criação de dCalendario e Schema)

[x] Desenvolvimento e validação das medidas DAX

[x] Planejamento de Layout e Identidade Visual

[x] Construção do dashboard no Power BI

[x] Validação dos requisitos e resultados

[x] Documentação final e versionamento no GitHub


📈 Resultado Final

<img width="1527" height="855" alt="telapainelperformanceacademia" src="https://github.com/user-attachments/assets/897f5749-3a5e-4f97-be42-b9712faeda34" />

[Clique aqui para acessar o Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZTNlY2FlYWItNzcyMC00NDRlLWI3NGItYjc2Y2YxMTczNzFhIiwidCI6IjU3NjM4MjI3LWY4NWYtNDgwMi05ZjlmLTllYTQxMzdjNjViYSJ9)


Desenvolvido por Giselle Guerra Ramos 🚀

🔗 [LinkedIn](https://www.linkedin.com/in/giselleguerra-ramos/) | 💻 [GitHub](https://github.com/giselleguerra)
