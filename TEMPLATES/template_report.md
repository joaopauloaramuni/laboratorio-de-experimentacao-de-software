# TEMPLATE DE RELATÓRIO DE LABORATÓRIO

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

**Exemplo de hipótese informal:**
> Sistemas populares recebem mais contribuições externas e lançam releases com maior frequência, refletindo um processo de desenvolvimento ativo.

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
- [RQ07 opcional para análise por linguagem]

---

## 6. Resultados
Apresente os resultados obtidos, com tabelas e gráficos, sempre que possível.
- Valores medianos, médias e desvio padrão.
- Distribuição por categoria (Ex.: linguagem de programação).
- Resultados adicionais segmentados por subgrupos se necessário.

**Exemplo de tabela:**
| Métrica | Mediana | Média | Desvio Padrão |
|---------|--------|------|---------------|
| Idade (anos) | X | Y | Z |
| Pull Requests Aceitas | X | Y | Z |

**Exemplo de gráfico:**
- Histogramas de distribuição de métricas.
- Boxplots para valores de dispersão.

---

## 7. Discussão
Compare os resultados obtidos com as hipóteses iniciais.
- Pontos que confirmam ou refutam as hipóteses.
- Possíveis explicações para os resultados divergentes.
- Observações sobre padrões interessantes nos dados.

---

## 8. Conclusão
Resumo das principais descobertas do laboratório.
- Destaque insights relevantes.
- Sugestões para trabalhos futuros ou análises adicionais.

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

```
# Fim do TEMPLATE
```

