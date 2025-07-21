# 🧠 Projeto Power BI - Dashboard de Vendas - Laboratório 1 - Data Science Academy

## 📌 Sobre o Projeto

Este projeto foi desenvolvido como parte de um curso prático de Power BI, no qual o desafio consistia em construir um dashboard do zero com base em dados fornecidos e responder a perguntas específicas através de visualizações interativas.

O principal objetivo foi transformar dados brutos em insights relevantes por meio de gráficos e segmentações, possibilitando ao usuário final uma análise clara e dinâmica das informações.

---

## 📁 Fonte dos Dados

- Arquivo CSV com os dados de vendas (produto, país, data do pedido, valor total, desconto, entre outros).
- Os dados foram importados via:  
  `Obter dados` → `Texto/CSV` → Selecionar arquivo → `Conectar`.

A estrutura das colunas foi ajustada e validada no **Power Query**, garantindo que os tipos de dados estivessem corretamente definidos (texto, número, data, etc).

---

## ❓ Perguntas Respondidas no Dashboard

1. **💰 Qual o valor total vendido?**  
   - Utilizado o visual de **Cartão** com a coluna `TOTAL_VENDAS`.

2. **📦 Quantas vendas foram realizadas por categoria de produto?**  
   - Utilizado **gráfico de pizza**, com `CATEGORIA` como legenda e contagem de `ID_PEDIDO` como valores.

3. **🌍 Quantas vendas foram realizadas por país considerando a prioridade de entrega?**  
   - Utilizado **gráfico de barras empilhadas**, com:  
     - Eixo Y: `PAÍS`  
     - Eixo X: `ID_PEDIDO`  
     - Legenda: `PRIORIDADE`

4. **📉 Qual foi a média de desconto nas vendas por subcategoria de produto?**  
   - Utilizado **gráfico de barras**, com:  
     - Eixo X: `SUBCATEGORIA`  
     - Eixo Y: `DESCONTO` (agregado como **média**)

5. **🗺️ Quais países tiveram maior média de valor de venda?**  
   - Utilizado **gráfico de mapa**, com:  
     - Localização: `PAÍS`  
     - Tamanho da bolha: `TOTAL_VENDAS` (agregado como **média**)  
   - Adicionado filtro interno para exibir apenas valores **maiores que 250**, a fim de evitar poluição visual.

---

## 🎛️ Funcionalidades do Dashboard

- Filtros interativos por:
  - **Ano**
  - **Segmento**
  - **País**
- Aplicados via o recurso de **Segmentação de Dados**.
- Os gráficos são dinâmicos e se adaptam conforme as seleções feitas.

---

## 🧩 Recursos Utilizados

- Power BI Desktop
- Power Query (ETL e transformação de dados)
- DAX básico para agregações
- Visualizações: cartão, pizza, barras, mapa
- Segmentações (filtros dinâmicos)

---

## 📚 Aprendizados

- Importação e preparação de dados no Power Query.
- Escolha adequada de gráficos com base nas perguntas.
- Agregações personalizadas (média, soma).
- Filtros e segmentações para refinar análises.
- Melhoria da experiência do usuário com interatividade.

---

