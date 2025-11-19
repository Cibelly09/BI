<div align="center">

# 🧠✨ Case 1 — ACM + K-Means + Power BI  
## Perfil dos Eleitores com Deficiência no Brasil  
Análise Sociodemográfica, Geográfica e Multivariada

</div>

---

<div align="center">

Este case apresenta uma análise completa sobre o perfil dos eleitores com deficiência no Brasil.  
O projeto combina técnicas estatísticas de ACM (Análise de Correspondência Múltipla), clusterização K-Means e visualização interativa no Power BI, resultando em uma leitura clara e integrada sobre as similaridades entre estados, seus padrões demográficos e seus comportamentos dentro da inclusão eleitoral.

</div>

---

# 1. Base Granular — df_obs  
A jornada começa pela base granular **df_obs**, que contém o nível mais detalhado das informações dos eleitores.  
Nela estão os atributos sociodemográficos originais utilizados para calibrar e validar os eixos da ACM.

Esses dados incluem:

Faixa etária  
Estado civil  
Raça/cor  
Gênero  
Identidade de gênero  
Escolaridade  
Atributos derivados da ACM (Axis1 e Axis2)  
Cluster numérico pré-modelo  

A df_obs funciona como a referência estatística do projeto, garantindo que o modelo multidimensional represente adequadamente a distribuição real dos eleitores.

<img src="imgs/wiki.png" width="800">

---

# 2. Página 1 — Mapa Perceptual (ACM + K-Means)

A análise visual inicia pelo **Mapa Perceptual**, que combina os dois principais eixos da ACM:

Dimensão Sociodemográfica  
Perfil de Inclusão Regional  

Cada ponto representa um estado brasileiro.  
As distâncias no gráfico expressam similaridade entre perfis, enquanto o algoritmo K-Means divide o espaço em **três clusters distintos**, agrupando estados que compartilham padrões semelhantes.

A página também conta com filtros dinâmicos por Região e Cluster, além de indicadores como:

- Estados Filtrados  
- Clusters Ativos  

Essa primeira visão revela a estrutura oculta dos dados e posiciona o Brasil em um mapa de similaridade social.

<img src="imgs/mapaperceptual.PNG" width="900">

---

# 3. Página 2 — Análise Geográfica por Cluster

Após entender o mapa perceptual, o usuário é direcionado ao **Mapa do Brasil**, que exibe cada estado colorido conforme o cluster ao qual pertence.  
Essa página permite observar:

A distribuição espacial dos clusters  
O Top Estado dentro da seleção  
O percentual médio de eleitores PCD  
Tendências regionais  

É aqui que percebemos padrões geográficos relevantes, como concentração de clusters em determinadas regiões e variações expressivas no percentual médio de PCD por UF.

<img src="imgs/mapabrasil.PNG" width="900">

---

# 4. Página 3 — Perfil Analítico do Cluster

A terceira página consolida o storytelling ao aprofundar o perfil de um cluster específico.  
Quando filtrado, o dashboard apresenta:

KPIs principais (ex.: % Médio PCD por UF, Score Final do Cluster)  
KPIs secundários (Total de Eleitores, Share do Cluster, Delta vs Brasil)  
Distribuição sociodemográfica  
Gênero predominante  
Raça predominante  
Composição do cluster  
Gráficos analíticos e contextualização  
Scatter ACM com destaque dos indivíduos daquele grupo  

Essa visão oferece a interpretação final e estratégica do cluster, permitindo tomadas de decisão e insights profundos.

<img src="imgs/perfil.png" width="900">

---

# 5. Wiki Interna e Documentação Analítica

O projeto conta também com uma página auxiliar de **Wiki**, responsável por centralizar descrições dos clusters, definições de métricas, explicações das variáveis e lógica dos eixos da ACM.  
É o espaço destinado a anotações e suporte à leitura analítica.

<img src="imgs/wiki.png" width="900">

---

# 6. Modelo Dimensional — Estrela + Snowflake

A estrutura de dados foi cuidadosamente modelada utilizando Esquema Estrela, garantindo performance, simplicidade e clareza.  
Algumas dimensões foram normalizadas (Snowflake) para reduzir redundância e melhorar segmentações regionais.

O modelo inclui:

Fato_Estados  
Dim_Estado  
Dim_Região  
Dim_Atributos_PCD  
Derivações dos eixos da ACM  
Atributos para visualizações e cálculos  

A seguir está o diagrama completo do modelo:

<img src="imgs/esquema.PNG" width="900">

---

# 7. Tecnologias e Metodologia Integrada

O projeto combina três frentes principais:

**Python** para pré-processamento, normalização, ACM, K-Means e criação dos scores.  
**Power BI** para visualização futurista em tema Neon, com métricas DAX e navegação interativa.  
**Modelagem Estatística** estruturada para explicar perfis e agrupar estados conforme similaridade social.

---

# 8. Design e Estética — Tema Futurista Neon

Todo o dashboard foi construído com identidade visual própria:

Azul ciano sobre fundo escuro  
Bordas luminosas  
Componentes geométricos  
Layout organizado em blocos temáticos  
Visual moderno e coerente em todas as páginas  

Essa estética reforça a sensação de tecnologia avançada e clareza visual.

---

<div align="center">

# ✍️ Autoria  
**Cibelly Viegas — 2025**

</div>
