# Template de Relatório Técnico de Laboratório

## 1. Informações do Grupo
- **Curso:** Engenharia de Software
- **Disciplina:** [Nome da disciplina]
- **Período/Sala:** [Informar]
- **Membros do Grupo:** [Lista de integrantes]
- **Professor(a):** [Nome do professor]

---

## 2. Introdução
Descreva o contexto do laboratório, objetivo do estudo e a relevância da análise.  
Inclua hipóteses informais sobre os resultados esperados.

**Exemplos de hipóteses informais:**
- Sistemas populares recebem mais contribuições externas e lançam releases com maior frequência, refletindo um processo de desenvolvimento ativo.
- Mais de 50% dos repositórios populares são mantidos há mais de 5 anos, indicando maturidade do projeto.
- Espera-se que mais de 50% dos repositórios populares tenham pelo menos 70% das issues fechadas, demonstrando boa gestão de problemas.
- Repositórios populares tendem a ser escritos nas linguagens mais utilizadas (por exemplo, JavaScript, Python, Java), representando a adoção de linguagens consolidadas.
- Mais de 50% dos repositórios populares recebem atualizações nos últimos 3 meses, refletindo atividade contínua da comunidade.
- Projetos populares com maior número de forks tendem a ter mais pull requests aceitas, indicando engajamento externo significativo.
- Repositórios populares com grande número de stars podem apresentar Big Numbers em métricas como número de commits, branches e releases, destacando sua relevância na comunidade open-source.

---

## 3. Tecnologias e Ferramentas Utilizadas
- **Linguagem de Programação:** [Ex.: Python, Java]
- **Frameworks/Bibliotecas:** [Ex.: Pandas, Matplotlib, Seaborn, CK]
- **APIs utilizadas:** [Ex.: GitHub GraphQL API, GitHub REST API]
- **Dependências:** [Ex.: requests, numpy]

---

## 4. Metodologia
Descreva detalhadamente as etapas do experimento ou estudo, incluindo coleta de dados, filtragem, normalização, análise e visualização.

**Exemplo:**

### 4.1 Coleta de Dados
- Foram coletados dados de [X] repositórios usando a [GitHub API].
- Critérios de seleção: [Ex.: top-1000 por número de estrelas, linguagem específica, etc.]

### 4.2 Filtragem e Paginação
- Utilizou-se paginação da API devido ao alto volume de dados.
- Tempo médio de coleta: [XX minutos].

### 4.3 Normalização e Pré-processamento
- Dados normalizados com [ex.: min-max scaling] para garantir consistência.

### 4.4 Cálculo de Métricas
- Métricas de interesse: idade do repositório, número de pull requests aceitas, número de releases, tempo desde a última atualização, linguagem primária, percentual de issues fechadas.
- Métricas compostas calculadas utilizando combinação linear ponderada de fatores relevantes.

### 4.5 Ordenação e Análise Inicial
- Repositórios ordenados por pontuação composta ou por número de estrelas.
- Análise inicial baseada em valores medianos e contagem de categorias.

---

## 5. Questões de Pesquisa
Liste as questões de pesquisa que guiaram o estudo.

**Exemplo:**
- RQ01: Sistemas populares são maduros/antigos?
- RQ02: Sistemas populares recebem muita contribuição externa?
- RQ03: Sistemas populares lançam releases com frequência?
- RQ04: Sistemas populares são atualizados com frequência?
- RQ05: Sistemas populares são escritos nas linguagens mais populares?
- RQ06: Sistemas populares possuem alto percentual de issues fechadas?

---

## 6. Resultados

Apresente os resultados obtidos, com tabelas e gráficos, sempre que possível.

### 6.1 Métricas

Inclua métricas relevantes de repositórios do GitHub, além das RQs:

| Métrica | Mediana | Média | Desvio Padrão |
|---------|--------|------|---------------|
| Idade do Repositório (anos) | X | Y | Z |
| Pull Requests Aceitas | X | Y | Z |
| Número de Releases | X | Y | Z |
| Tempo desde a Última Atualização (dias) | X | Y | Z |
| Percentual de Issues Fechadas (%) | X | Y | Z |
| Número de Estrelas (Stars) | X | Y | Z |
| Número de Forks | X | Y | Z |
| Tamanho do Repositório (LOC) | X | Y | Z |

> Obs.: Adapte ou acrescente métricas conforme o seu dataset.

### 6.2 Distribuição por Categoria

Para métricas categóricas, como linguagem de programação, faça contagens e tabelas de frequência:

| Linguagem | Quantidade de Repositórios |
|-----------|---------------------------|
| Python    | 350                       |
| JavaScript| 300                       |
| Java      | 200                       |
| Outros    | 150                       |

### 6.3 Sugestões de Gráficos

Para visualização de métricas, sugiro consultar o projeto **Seaborn Samples**:
- Repositório: [Projeto Seaborn Samples](https://github.com/joaopauloaramuni/laboratorio-de-experimentacao-de-software/tree/main/PROJETOS/Projeto%20Seaborn%20Samples)

- **Histograma**: `grafico_histograma.png` → distribuição de idade, PRs aceitas ou estrelas.  
- **Boxplot**: `grafico_boxplot.png` → dispersão de métricas como forks, issues fechadas ou LOC.  
- **Gráfico de Barras**: `grafico_barras.png` → comparação de métricas entre linguagens.  
- **Gráfico de Pizza**: `grafico_pizza.png` → percentual de repositórios por linguagem.  
- **Gráfico de Linha**: `grafico_linha.png` → evolução de releases ou PRs ao longo do tempo.  
- **Scatterplot / Dispersão**: `grafico_dispersao.png` → relação entre estrelas e forks.  
- **Heatmap**: `grafico_heatmap.png` → correlação entre métricas (idade, PRs, stars, forks, issues).  
- **Pairplot**: `grafico_pairplot.png` → análise de múltiplas métricas ao mesmo tempo.  
- **Violin Plot**: `grafico_violin.png` → distribuição de métricas detalhada, por subgrupo.  
- **Barras Empilhadas**: `grafico_barras_empilhadas.png` → comparação de categorias dentro de métricas.

> Dica: combine tabelas e gráficos para facilitar a interpretação e evidenciar padrões nos dados. Use o projeto **Seaborn Samples** como base para implementar todos esses gráficos.

---

## 7. Discussão

Nesta seção, compare os resultados obtidos com as hipóteses informais levantadas pelo grupo no início do experimento.

- **Confirmação ou refutação das hipóteses**: identifique quais hipóteses foram confirmadas pelos dados e quais foram refutadas.  
- **Explicações para resultados divergentes**: caso algum resultado seja diferente do esperado, tente levantar possíveis causas ou fatores que possam ter influenciado.  
- **Padrões e insights interessantes**: destaque tendências ou comportamentos relevantes observados nos dados que não haviam sido previstos nas hipóteses.  
- **Comparação por subgrupos (opcional)**: se houver segmentação dos dados (ex.: por linguagem de programação, tamanho do repositório), discuta como os resultados se comportam em cada grupo.  

> Lembre-se de sempre relacionar os pontos observados com as hipóteses informais definidas na introdução, fortalecendo a análise crítica do experimento.

---

## 8. Conclusão

Resumo das principais descobertas do laboratório.

- **Principais insights:**  
  - Big numbers encontrados nos repositórios/popularidade/métricas destacadas.  
  - Descobertas relevantes sobre padrões de contribuição, releases, issues fechadas ou linguagens mais utilizadas.  
  - Confirmações ou refutações das hipóteses informais levantadas pelo grupo.

- **Problemas e dificuldades enfrentadas:**  
  - Limitações da API do GitHub e paginação de grandes volumes de dados.  
  - Normalização e tratamento de dados inconsistentes ou ausentes.  
  - Desafios com cálculos de métricas ou integração de múltiplos arquivos CSV.  

- **Sugestões para trabalhos futuros:**  
  - Analisar métricas adicionais ou aprofundar correlações entre métricas de qualidade e métricas de processo.  
  - Testar outras linguagens de programação ou frameworks.  
  - Implementar dashboards interativos para visualização de grandes volumes de dados.  
  - Explorar métricas de tendências temporais ou evolução de repositórios ao longo do tempo.

---

## 9. Referências
Liste as referências bibliográficas ou links utilizados.
- [GitHub API Documentation](https://docs.github.com/en/graphql)
- [CK Metrics Tool](https://ckjm.github.io/)
- [Biblioteca Pandas](https://pandas.pydata.org/)
- [Power BI](https://docs.microsoft.com/en-us/power-bi/fundamentals/service-get-started)

---

## 10. Apêndices (opcional)
- Scripts utilizados para coleta e análise de dados.
- Consultas GraphQL ou endpoints REST.
- Planilhas e arquivos CSV gerados.

---
