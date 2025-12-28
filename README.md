# Eficiência Energética na Indústria Siderúrgica

**Tipo:** Regressão (Supervisionado)
**Dataset:** [Steel Industry Energy Consumption - UCI](https://archive.ics.uci.edu/ml/datasets/Steel+Industry+Energy+Consumption)

## Sobre o Projeto
Este projeto foca em **custos e eficiência** (Regressão). O objetivo foi criar um modelo capaz de prever o consumo de energia elétrica (kWh) de uma siderúrgica com base em variáveis operacionais e de fator de potência.

## Desafio de Negócio
Indústrias intensivas em energia pagam caro por desvios de demanda. O desafio era traduzir variáveis elétricas complexas (Potência Reativa Indutiva/Capacitiva) em um modelo preditivo que auxiliasse no planejamento de produção e redução de custos.

## Tecnologias e Estratégia
* **Python:** Pandas, Seaborn, Scikit-Learn.
* **Engenharia de Atributos:** Tratamento de *Data Leakage* (remoção da variável CO2 que era derivada da resposta) e tradução de termos técnicos (Leading/Lagging Power).
* **Modelo:** Random Forest Regressor.

## Resultados Chave
* **R² (Precisão):** > 0.98 (O modelo explica 98% da variação do consumo).
* **Insights de Engenharia:**
    * Identificada correlação negativa (-0.32) na Potência Capacitiva, sugerindo comportamento de sobrecorreção dos bancos de capacitores em baixa carga.
    * O modelo mostrou-se extremamente robusto na faixa operacional padrão (até 140 kWh), com desvios mínimos.

## Visualização
<img width="1005" height="547" alt="image" src="https://github.com/user-attachments/assets/d6dd0dcb-7f6d-47a8-b68b-bd24c9f283eb" />

---
*Desenvolvido por Davi Duarte Cucco | [LinkedIn](https://www.linkedin.com/in/davi-duarte-cucco-8b272a238/)*
