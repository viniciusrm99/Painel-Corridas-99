https://www.youtube.com/watch?v=Kp7BlmfFhz4 1:09:13 

# 🚖 Análise de Viagens Uber – Projeto Power BI

Dashboard interativo em Power BI analisando dados de viagens da Uber para descobrir tendências de reservas, insights de receita e eficiência das viagens, ajudando stakeholders a tomar **decisões baseadas em dados**.  

---

## 📊 Dashboard 1: Análise Geral  
Analisa dados de viagens para identificar tendências, geração de receita e eficiência das viagens.

### **Principais KPIs**
- 📌 **Total de Reservas** – Total de viagens realizadas em um período.  
- 💰 **Valor Total das Reservas** – Receita total de todas as viagens.  
- 📏 **Valor Médio por Reserva** – Receita média por viagem.  
- 🛣 **Distância Total das Viagens** – Distância total percorrida em todas as viagens.  
- 📍 **Distância Média por Viagem** – Distância média percorrida por viagem.  
- ⏱ **Tempo Médio de Viagem** – Duração média das viagens.  

**✅ Resultados Esperados:**  
✔ Identificar tendências em reservas e geração de receita.  
✔ Analisar a eficiência das viagens (distância e duração).  
✔ Comparar valores de reservas e padrões de viagem ao longo do tempo.  
✔ Apoiar otimização de preços e aumentar a satisfação do cliente.  

**📈 Gráficos e Funcionalidades:**  
- **Selector de Métricas** 🎛 – Alterna entre Total de Reservas, Valor Total das Reservas e Distância Total das Viagens usando uma tabela desconectada.  
- **Por Tipo de Pagamento** 💳 (Cartão, Dinheiro, Carteira, etc.)  
- **Por Tipo de Viagem** 🌞🌙 (Dia/Noite)  
- **Título Dinâmico** ✨ – Atualiza conforme a métrica selecionada.  
- **Slicers Interativos** 🗂 – Filtragem por Data, Cidade e outros para análises detalhadas.  
- **Tooltips** 🛠 – Mostra detalhes adicionais como Valor Médio por Reserva ou Distância da Viagem.  

---

## 🚘 Análise por Tipo de Veículo  
- Tabela em Grid (Matrix) para analisar KPIs por Tipo de Veículo.  
- Formatação condicional para destacar valores altos e baixos.  
- Permite ordenar e filtrar para interações do usuário.  

---

## 📅 Reservas por Dia  
- Identificação de tendências e variações diárias.  
- Reconhecimento de dias de pico e fora de pico.  
- Avaliação do impacto de fatores externos (feriados, eventos, clima) na demanda.  

---

## 📍 Análise de Localização  
- **Pontos de Partida Mais Frequentes** – Otimização de disponibilidade de motoristas.  
- **Pontos de Chegada Mais Frequentes** – Análise de demanda e estratégias de preço dinâmico.  
- **Viagem Mais Longa** – Identificação de outliers e otimização de tarifas.  
- **Top 5 Locais por Reservas** – Previsão de demanda e alocação de motoristas.  
- **Veículo Mais Preferido por Local de Partida** – Distribuição estratégica de veículos.  

---

## ⏰ Dashboard 2: Análise Temporal  
- Seleção dinâmica de métricas para atualizar todos os gráficos.  
- **Por Hora de Pickup (intervalos de 10 min)** – Identificação de períodos de pico.  
- **Por Dia da Semana** – Comparação entre dias úteis e finais de semana.  
- **Heatmap Hora x Dia** – Destaca horários de maior demanda.  

---

## 📋 Dashboard 3: Detalhes  
- Grid com detalhes completos das viagens.  
- Funcionalidade de Drill-Through – acessar registros detalhados a partir de seleções em outros dashboards.  
- Bookmark "Visualizar Todos os Dados" para alternar entre dados filtrados e dataset completo.  

---

## ⚙️ Funcionalidades Extras  
- **Bookmark “Detalhes dos Dados”** 📝 – Explicação de métricas e fontes de dados.  
- **Botão Limpar Filtros** 🔄 – Reset rápido de todos os slicers.  
- **Download de Dados** 📥 – Exportação em CSV ou Excel via Power Automate ou funcionalidade nativa do Power BI.
