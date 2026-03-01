#  NDVI Analysis – Florianópolis | Americas TechGuard

Este projeto realiza o cálculo e análise do NDVI (Normalized Difference Vegetation Index) aplicado ao município de Florianópolis (SC), utilizando imagens do satélite Sentinel-2.

O objetivo é compreender a cobertura vegetal da região e sua possível relação com o risco de inundação, dentro do contexto do projeto Americas TechGuard.

---

##  Objetivos

- Executar e compreender o script base de cálculo do NDVI
- Replicar a análise em nova região (Florianópolis)
- Gerar mapa temático e histograma
- Interpretar resultados quantitativamente
- Relacionar cobertura vegetal com risco de inundação

---

##  Dados Utilizados

- Satélite: Sentinel-2 (L2A)
- Resolução espacial: 10 metros
- Bandas utilizadas:
  - B4 (Red)
  - B8 (NIR)

---

##  Fórmula do NDVI

\[
NDVI = \frac{NIR - Red}{NIR + Red}
\]

Valores variam entre -1 e +1:

- Próximo de +1 → vegetação densa
- Próximo de 0 → solo exposto / área urbana
- Negativo → água ou superfície não vegetada

---

##  Resultados Obtidos – Florianópolis

Estatísticas do NDVI:

- Valor mínimo: -0.643
- Valor máximo: 0.772
- Média: 0.168
- Desvio padrão: 0.260

Distribuição percentual:

- NDVI < 0 → 42.99%
- 0 – 0.2 → 23.20%
- 0.2 – 0.4 → 3.88%
- ≥ 0.4 → 29.93%

Observa-se forte heterogeneidade territorial, típica de ambiente urbano costeiro com presença de áreas vegetadas e corpos d’água.

---

##  Relação com Risco de Inundação

Regiões com menor NDVI tendem a apresentar:

- Maior impermeabilização
- Maior escoamento superficial
- Potencial aumento de risco de alagamento

Áreas com vegetação mais densa favorecem infiltração e retenção hídrica.

---

##  Tecnologias Utilizadas

- Python
- Rasterio
- NumPy
- Matplotlib
- Jupyter Notebook

---

##  Próximos Passos

- Integração com Modelo Digital de Elevação (MDE)
- Análise pluviométrica histórica
- Construção de modelo preditivo multivariado
- Integração com sistema de alerta climático

---

##  Autor

Pedro Henrique Nunes Zanette  
Projeto acadêmico – Americas TechGuard  
Centro Universitário SENAI/SC – Florianópolis