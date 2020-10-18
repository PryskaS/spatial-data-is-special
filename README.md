
# Geodata science

* **Libraries para explorar**
  * [Pysal](https://pysal.org/pysal/): library for geospatial data science with an emphasis on geospatial vector data written in Python, [geemap](https://pypi.org/project/geemap/): package for interactive mapping with Google Earth Engine,[MovingPandas](https://anitagraser.github.io/movingpandas/): working with movement data, [Momepy](http://docs.momepy.org/en/latest/): quantitative analysis of urban morphology, [Satpy](https://satpy.readthedocs.io/en/stable/): package for earth-observing satellite data processing, [xesmf](https://xesmf.readthedocs.io/): Universal Regridder for Geospatial Data, [verde](https://www.fatiando.org/verde/): interpolating spatial data on regular grids, [rioxarray](https://github.com/corteva/rioxarray): linking rasterio functionality with xarray, [MetPy](https://unidata.github.io/MetPy): working with weather data, [xgcm](https://xgcm.readthedocs.io/en/latest/index.html): working with output from General Circulation Models, [osmnx](https://github.com/gboeing/osmnx): street networks, [geoplot](https://residentmario.github.io/geoplot/): high-level Python geospatial plotting library (combining GeoPandas, matplotlib and cartopy), [geobr](https://github.com/ipeaGIT/geobr#geobr--): package to download official spatial data sets of Brazil, [Basedosdados](https://basedosdados.github.io/mais/): Mecanismo de busca e repositório de bases de dados brasileiras e internacionais, [PyTorch Geometric Temporal](https://github.com/benedekrozemberczki/pytorch_geometric_temporal): PyTorch Geometric Temporal makes implementing Dynamic and Temporal Graph Neural Networks quite easy, 
  * **Machine learning**: scikit-learn, tensorflow, pytorch, keras, chainer, ... **Performance**: Numba, Cython, Numexpr, Pythran, C/Fortran wrappers, ...**Visualisation**: Bokeh, Seaborn, Plotnine, Altair, Plotly, Mayavi, HoloViews, datashader, vaex ... **Data structures and parallel/distributed computation**: Xarray, Dask, Distributed, Cupy, ... **Specialized packages in many scientific fields**: astronomy, natural language processing, image processing, geospatial, ... **Packaging and distribution**: pip/wheels, conda, Anaconda, Canopy.
 
* [Good Enough Practices in Scientific Computing](https://arxiv.org/pdf/1609.00037v1.pdf)

---
### Conteúdo

| **Cartografia básica** |

  * **[Fundamentos conceituais](https://github.com/PryskaS/spatial-data-is-special/blob/master/1.%20Notebooks/Fundamentos%20de%20Cartografia%20para%20SIG%20I.ipynb)**: Conceitos básicos de cartografia, Sistema de Informação Geográfica (SIG/GIS), dados espaciais, projeções cartográficas, sistemas de coordenadas, modelos de representação da terra - Datum, sistema de referência de coordenadas. 
  
 * **[Framework]()**: Base inicial para todos os projetos; cuidados para manter a base cartográfica em conformidade com a geomática.
 
| **Representação computacional do Espaço** |

  * Níveis de abstração, objetos vs campos, estrutura de dados espaciais, topologia, superposição de planos de informação.
  * Modelagem Numérica de Terreno (MNT): Pontos cotados (z, y, z), isolinhas, malha triangular (TIN), dados altimétricos, shuttle radar topography Mission (SRTM).

| **Manipulação de dados geográficos** |

  * **[Data wrangling]()**: Importar dados vetoriais e  matriciais, unir dados espaciais por atributo (attribut join) e por localização (spatial join), consulta e edição de atributos, modificar dados (Field Calculator), select by attribute, select by expresso, select by location, criar novas feições, remodelar feições, offset (linhas), cortar feições (split), dividir partes, mesclar feições (merge).

| **Fonte de dados** |

  * Infraestrutura de informação espacial (SDI), padrões OGC (WMS, WFS, WCS), metadados.

| **Qualidade dos dados geoespaciais** | 

  * Consistência lógica, consistência tipológica, adequação quanto ao nível de generalização cartográfica empregado.

| **Generalização** | 

  * Simplicacação (building, Line, polygon), suavização (smooth), agregação (dissolve, agregaste polygons, Eliminate), fusão (merge divided roads, collapse dual lines), colapso, refinamento.
 
| **Geovizualização** |

  * Forma espacial e modo de implementação, ideia de qualidade (distinção/diferenciação), ideia de quantidade e ordem, classes (intervalos iguais, quantil, desvio padrão, quebras naturais - jernks -, intervalo geométrico, mapas coropláticos e de símbolos proporcionais, cartogramas e cartografia temática, mapas de densidade de pontos e mapas de fluxos, geovisualização multivariada, temporal e de incerteza.

| **Análise espacial** |

  * **[Abordagens]**: Estatística espacial, análise espacial, econometria espacial e geoestatística.
  * **[Teste de hipóteses sobre autocorrelação espacial]**:
  * **[Análise de eventos pontuais]**: Distribuição de Poisson Homogênea - complete spatial randomness (CSR), Método do vizinho mais próximo, Função K de Ripley (univariada e bivariada), estimador de intensidade (Kernel estimation), processo pontual marcado, estudos caso-controle.
  * **[Análise de superfícies por geoestatística linear]**: modelos determinísticos locais, modelos estatísticos de efeitos locais e globais (krigagem), modelos determinísticos de efeitos globais (superfícies de tendência), semivariograma. 
  * **[Análise de superfícies por geoestatística indicadora]**: Krigeagem por indicação ordinária, correção dos desvios de ordem, estimativa de incertezas locais, estimadores ótimos para as superfícies interpoladas, incertezas locais para atributos categóricos, classificadores para atributos categóricos, medidas de incerteza para atributos Categóricos.
  * **[Análise de dados de área]**: Índice de Moran (global e local), índice C de Geary, Variograma, Matrizes de Proximidade Espacial, Média Móvel Espacial.
  * **[Modelagem dinâmica]**: Cadeias de Markov, Logístico de Difusão, Regressão, Simulação de Ecossistemas, Simulação Espacial Dinâmica.
  * ESDA: Exploratory Spatial Data Analysis
  * Modelos de Regressão Espacial Globais: Spatial Lag e Spatial Error
  * Modelos de Regressão Espacial Locais: Regimes Espaciais e Regressão Geograficamente Ponderada (GWR).
  * Cluster Analysis: LISA.
  * Geral: Interpolação, Krigagem, centro médio, distância padrão, elipse de distância padrão, padrões de agregação, vizinho mais próximo, vizinhos naturais (k-means), análise de Lacunaridade, métodos de estimação de kernel e kernel adaptativo,  mapas de proximidade vs mapas de kernel, polígonos de voronoi, triangulação de Deulanay.

| **Geocodificação de endereços** | 

| **GeoWeb/WebGIS** | 

  * Framework para Carto
  * Framework para Kepler
  * GeoWeb Crawler

| **Sensoriamento remoto** |

  * Conceitos básicos e princípios da radiação eletromagnética
  * Níveis de aquisição, sensores, geração de imagem, assinatura espectral x bandas
  * Composições coloridas 
  * Resolução espacial, resolução espectral, resolução radiométrica, resolução temporal
  * Comportamento espectral
  * NDVI
  * Elementos de fotointerpretação
  * Pré-processamento (estatísticas da imagem, transformações lineares e não-lineares)
  * Modelos de correção geométrica
  * Mapeamento inverso
  * Reamostragem, erro médio quadrático, qualidade dos pontos
  * Transformações de imagens: fatiamento de histograma, IHS, alterações da componente S, componentes principais, espalhamento bi-dimensional, espalhamentos para imagens correlacionadas e não-correlacionadas.
  * NDWI - Normalized Difference Water index, Fusão.
  * Classificação supervisionada e não-supervisionada. 

| **Spatio-temporal Models** |  

