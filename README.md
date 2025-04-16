#Lista dos **Modelos preditivos**

---

![image](https://github.com/user-attachments/assets/8d500e00-80cb-4381-89f5-970e62217267)


### ✅ **Classificação dos modelos preditivos**
- Modelos estatísticos clássicos: AR, MA, ARMA, ARIMA, SARIMA, etc.
- Modelos estruturais: Prophet, Holt-Winters.
- Modelos multivariados: VAR, ARIMAX.
- Modelos de machine learning: XGBoost, LightGBM.
- Modelos de deep learning: RNN, LSTM, GRU, Transformer, CNN.

---

### 📋 Tabela detalhada de Modelos preditivos


| **#** | **Modelo** | **Descrição** | **Aplicações** | **Prós** | **Contras** |
|------:|------------|---------------|----------------|----------|-------------|
| 1 | **AR** (AutoRegressive) | Usa valores passados para prever o futuro. | Preço de ativos, demanda estável, séries estacionárias. | Simples, eficaz em séries estacionárias. | Ignora tendência e sazonalidade. |
| 2 | **MA** (Moving Average) | Usa erros passados (resíduos) para previsão. | Previsões de curto prazo em séries com ruído. | Suaviza variações aleatórias. | Não captura tendências nem ciclos. |
| 3 | **ARMA** | Combina AR e MA. | Séries com ruído e autocorrelação, sem tendência. | Mais robusto que AR/MA isoladamente. | Exige série estacionária. |
| 4 | **ARIMA** | ARMA com diferenciação para lidar com tendência. | Vendas, temperatura, séries com tendência. | Funciona bem com séries não estacionárias. | Não trata sazonalidade naturalmente. |
| 5 | **SARIMA** | ARIMA com componentes sazonais. | Séries com sazonalidade: vendas mensais, clima. | Lida com tendência e sazonalidade. | Muitos parâmetros, difícil ajustar. |
| 6 | **ARIMAX / SARIMAX** | ARIMA com variáveis exógenas. | Vendas afetadas por promoções, economia. | Inclui efeitos externos. | Requer bons dados exógenos. |
| 7 | **VAR** | Modela múltiplas séries ao mesmo tempo. | PIB, inflação, câmbio — indicadores interdependentes. | Capta interações entre variáveis. | Requer muitas observações históricas. |
| 8 | **ES** (Exponential Smoothing) | Suaviza a série com pesos decrescentes. | Séries com padrão estável de curto prazo. | Simples e rápido. | Não modela tendência/sazonalidade. |
| 9 | **Holt-Winters** | ES com tendência e sazonalidade. | Demanda por produtos sazonais. | Eficaz em sazonalidade simples. | Menos flexível que SARIMA. |
| 10 | **Prophet (Facebook)** | Modelo aditivo com tendência, sazonalidade e feriados. | Tráfego de sites, sazonalidade de negócios. | Fácil de ajustar, robusto a outliers. | Acurácia pode ser inferior a modelos complexos. |
| 11 | **RNN** | Rede neural com memória de curto prazo. | Texto sequencial, séries financeiras. | Aprende padrões sequenciais. | Difícil de treinar, instável. |
| 12 | **LSTM** | RNN com memória de longo prazo. | Séries com dependências longas, sensores. | Lida com dependência de longo prazo. | Pesado e lento para treinar. |
| 13 | **GRU** | Variante mais simples do LSTM. | Alternativa leve ao LSTM. | Mais rápido que LSTM com bom desempenho. | Pode perder precisão em casos complexos. |
| 14 | **Transformer** | Modelo de atenção sem recorrência. | Séries longas e multivariadas, NLP temporal. | Muito poderoso com grandes dados. | Requer muitos dados e recursos. |
| 15 | **XGBoost / LightGBM** | Árvores com features temporais. | Previsão de churn, vendas, séries com múltiplas variáveis. | Alta precisão e interpretabilidade. | Requer engenharia de features. |
| 16 | **CNN para séries** | Detecta padrões locais em sequências. | Detecção de anomalias, séries sensoriais. | Rápido e eficaz em padrões locais. | Não modela bem longas dependências. |

---

### 🧩 **Outros modelos preditivos relevantes que podem ser considerados**:

| Modelo / Técnica | Tipo | Descrição / Aplicação |
|------------------|------|------------------------|
| **TBATS**        | Estatístico | Variante do Holt-Winters com transformações Box-Cox, tendência, ARMA e sazonalidades múltiplas (bom para séries com múltiplas sazonalidades). |
| **Theta Model**  | Estatístico | Modelo simples e muito usado em competições como M4. Baseado em decomposição da série. |
| **Gaussian Processes (GP)** | Probabilístico | Útil para séries temporais com incerteza alta e pequena quantidade de dados. |
| **Kalman Filter / State Space Models** | Estatístico / Dinâmico | Utilizados para rastrear estados ocultos no tempo. Ex: posição de objetos em sistemas dinâmicos. |
| **Ensembles (Ex: híbrido ARIMA + LSTM)** | Híbrido | Combina modelos estatísticos com deep learning para melhor desempenho. |
| **TFT (Temporal Fusion Transformer)** | Deep Learning | Modelo SOTA (state-of-the-art) da Google para séries temporais multivariadas. Lida com tendências, dados ausentes e variáveis exógenas. |
| **DeepAR** | Deep Learning | Criado pela Amazon, modela séries temporais como problemas de aprendizado probabilístico. Ideal para previsão de múltiplas séries. |
| **N-BEATS / N-HITS** | Deep Learning | Modelos recentes da Meta AI, voltados a previsões altamente precisas. Usados em competições de forecasting. |

---

 
