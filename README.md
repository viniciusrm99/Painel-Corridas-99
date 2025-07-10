## Projeto de BI: Análise do Brasileirão (Série A)

---

### 🤖 Objetivo do Projeto

Criar um dashboard interativo que analisa o desempenho dos times do Brasileirão, comparando:

* Gols marcados e sofridos
* Aproveitamento em casa/fora
* Artilheiros
* Classificação rodada a rodada
* Tendências e destaques por time

---

### 📁 Fontes de Dados

* Kaggle: "Brazilian Serie A Matches Dataset (2012-2023)"
* Alternativas: FBref, Footystats, Transfermarkt

---

### 📅 Importação dos Dados

No Power BI:

1. Obter dados > Arquivo CSV/Excel
2. Importar as tabelas:

   * Matches (dados dos jogos)
   * Teams (opcional: informações dos times)
   * Players (opcional: para detalhar artilharia)

---

### 🧼 Limpeza e Tratamento dos Dados (Power Query)

* Renomear colunas
* Padronizar nomes dos times
* Converter tipos de dados (data, números)
* Criar colunas derivadas:

  * Resultado do jogo (Vitória / Empate / Derrota)
  * Mandante venceu? (if home\_goals > away\_goals then "Sim"...)
  * Gols totais
  * Diferença de gols

---

### 🧬 Modelagem dos Dados

**Tabelas:**

* Fato: Fato\_Jogos
* Dimensão: Dim\_Times, Dim\_Data, Dim\_Campeonato

**Relacionamentos:**

* Fato\_Jogos\[time\_mandante\_id] ↔ Dim\_Times\[ID]
* Fato\_Jogos\[data] ↔ Dim\_Data\[data]

---

### 🧩 Criação de Medidas (DAX)

* Total de Gols:

```DAX
Total Gols = SUM(Fato_Jogos[home_goals]) + SUM(Fato_Jogos[away_goals])
```

* Aproveitamento (%):

```DAX
Aproveitamento = DIVIDE([Pontos], [Jogos])*100
```

* Vitórias, Derrotas, Empates por time
* Gols marcados / sofridos por local (casa x fora)

---

### 📊 Visualizações Sugeridas (Power BI)

**Página 1: Visão Geral do Campeonato**

* Tabela de classificação com filtro de temporada
* Cartões: total de gols, média por jogo
* Barras horizontais: gols por time

**Página 2: Análise por Time**

* Seletor de time
* Linha: evolução na classificação
* Coluna: gols marcados x sofridos

**Página 3: Mandante vs Visitante**

* Comparativo de desempenho
* Gráfico de pizza: vitórias casa x fora

**Página 4: Artilharia**

* Top 10 artilheiros
* Eficiência: gols por minuto jogado

---

### 💡 Possíveis Insights

* Time com melhor desempenho fora de casa
* Time que mais vira jogo
* Jogo com mais gols
* Time que mais toma gol no fim do jogo
* Rodada com mais empates

---

### 🏰 Extras para valorizar o projeto

* Ícones dos times
* Slicers de temporada, rodada, time
* Página "Sobre o Projeto" com contexto, fonte dos dados e objetivo

---

### 💥 Finalização

* Publicar no Power BI Service ou exportar como PDF
* Compartilhar no LinkedIn com texto e insights
* (Opcional) Postar no GitHub com PBIX + README explicando o projeto
