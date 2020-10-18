
# Geodata science

* **Libraries para explorar**
  * [Pysal](https://pysal.org/pysal/): library for geospatial data science with an emphasis on geospatial vector data written in Python, [geemap](https://pypi.org/project/geemap/): package for interactive mapping with Google Earth Engine,[MovingPandas](https://anitagraser.github.io/movingpandas/): working with movement data, [Momepy](http://docs.momepy.org/en/latest/): quantitative analysis of urban morphology, [Satpy](https://satpy.readthedocs.io/en/stable/): package for earth-observing satellite data processing, [xesmf](https://xesmf.readthedocs.io/): Universal Regridder for Geospatial Data, [verde](https://www.fatiando.org/verde/): interpolating spatial data on regular grids, [rioxarray](https://github.com/corteva/rioxarray): linking rasterio functionality with xarray, [MetPy](https://unidata.github.io/MetPy): working with weather data, [xgcm](https://xgcm.readthedocs.io/en/latest/index.html): working with output from General Circulation Models, [osmnx](https://github.com/gboeing/osmnx): street networks, [geoplot](https://residentmario.github.io/geoplot/): high-level Python geospatial plotting library (combining GeoPandas, matplotlib and cartopy), [geobr](https://github.com/ipeaGIT/geobr#geobr--): package to download official spatial data sets of Brazil, [Basedosdados](https://basedosdados.github.io/mais/): Mecanismo de busca e repositório de bases de dados brasileiras e internacionais.
  * **Machine learning**: scikit-learn, tensorflow, pytorch, keras, chainer, ... **Performance**: Numba, Cython, Numexpr, Pythran, C/Fortran wrappers, ...**Visualisation**: Bokeh, Seaborn, Plotnine, Altair, Plotly, Mayavi, HoloViews, datashader, vaex ... **Data structures and parallel/distributed computation**: Xarray, Dask, Distributed, Cupy, ... **Specialized packages in many scientific fields**: astronomy, natural language processing, image processing, geospatial, ... **Packaging and distribution**: pip/wheels, conda, Anaconda, Canopy.
 
* [Good Enough Practices in Scientific Computing](https://arxiv.org/pdf/1609.00037v1.pdf)

---
### Conteúdo

**Fundamentos de Cartografia para SIG** | [notebook](https://github.com/PryskaS/spatial-data-is-special/blob/master/1.%20Notebooks/Fundamentos%20de%20Cartografia%20para%20SIG%20I.ipynb) | medium|
  * Conceitos básicos de cartografia, Sistema de Informação Geográfica (SIG/GIS), dados espaciais, projeções cartográficas, sistemas de coordenadas, modelos de representação da terra - Datum, sistema de referência de coordenadas.
  
 **Representação computacional do Espaço** | notebook | medium|
  * Níveis de abstração, objetos vs campos, estrutura de dados espaciais, topologia, superposição de planos de informação.
  * Modelagem Numérica de Terreno (MNT): Pontos cotados (z, y, z), isolinhas, malha triangular (TIN), dados altimétricos, shuttle radar topography Mission (SRTM).

**Manipulação de dados geográficos** | notebook | medium|
  *  importar dados matriciais e vetoriais, unir dados espaciais, consulta e edição de atributos, modificar dados (Field Calculator), select by attribute, select by expresso, select by location, criar novas feições, remodelar feições, offset (linhas), cortar feições (split), dividir partes, mesclar feições (merge).

**Fonte de dados** | notebook | medium|
  * Infraestrutura de informação espacial (SDI), padrões OGC (WMS, WFS, WCS), metadados.

**Qualidade dos dados geoespaciais** 
  * Consistência lógica, consistência tipológica, adequação quanto ao nível de generalização cartográfica empregado.

**Generalização** | notebook | medium|
  * Simplicacação (building, Line, polygon), suavização (smooth), agregação (dissolve, agregaste polygons, Eliminate), fusão (merge divided roads, collapse dual lines), colapso, refinamento.
 
**Geovizualização** | notebook | medium|
  * Forma espacial e modo de implementação, ideia de qualidade (distinção/diferenciação), ideia de quantidade e ordem, classes (intervalos iguais, quantil, desvio padrão, quebras naturais - jernks -, intervalo geométrico, mapas coropláticos e de símbolos proporcionais, cartogramas e cartografia temática, mapas de densidade de pontos e mapas de fluxos, geovisualização multivariada, temporal e de incerteza.

**Análise espacial** | notebook | medium| 
  * Estatística espacial vs análise espacial, Análise de eventos pontuais, análise de superfícies por geoestatística linear, análise de superfícies por geoestatística indicadora, análise de dados de área, modelagem dinâmica. ESDA: Exploratory Spatial Data Analysis, Modelos de Regressão Espacial Globais: Spatial Lag e Spatial Error, Modelos de Regressão Espacial Locais: Regimes Espaciais e Regressão Geograficamente Ponderada (GWR), Cluster Analysis. Interpolação, Krigagem, centro médio, distância padrão, elipse de distância padrão, padrões de agregação, vizinho mais próximo, vizinhos naturais (k-means), função K de Ripley (univariada e bivariada), Análise de Lacunaridade, métodos de estimação de kernel e kernel adaptativo,  mapas de proximidade vs mapas de kernel, polígonos de voronoi, triangulação de Deulanay.

**Geocodificação de endereços** | notebook | medium| 

**GeoWeb/WebGIS** | notebook | medium| 
  * Framework para Carto, Kepler, GeoWeb Crawler.

**Sensoriamento remoto** | notebook | medium|
  * Conceitos básicos e princípios da radiação eletromagnética, níveis de aquisição, sensores, geração de imagem, assinatura espectral x bandas, composições coloridas, resolução espacial, resolução espectral, resolução radiométrica, resolução temporal, comportamento espectral, NDVI, elementos de fotointerpretação, pré-processamento (estatísticas da imagem, transformações lineares e não-lineares), modelos de correção geométrica, mapeamento inverso, reamostragem, erro médio quadrático, qualidade dos pontos, transformações de imagens (fatiamento de histograma, IHS, alterações da componente S, componentes principais, espalhamento bi-dimensional, espalhamentos para imagens correlacionadas e não-correlacionadas, NDWI - Normalized Difference Water index, Fusão, classificação supervisionada e não-supervisionada. 
