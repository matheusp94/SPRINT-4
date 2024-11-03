Reflexões - o que funcionou, o que não funcionou, o que foi aprendido, o que seria feito diferente

<br>
<p>Possível falta de otimização: Obtivemos problemas de desempenho em alguns momentos, com pequeno impacto, mas que ainda poderiam ser solucionados. Em função do foco ter sido na funcionalidade e não no desempenho, este elemento acabou sendo posto de lado. Otimizadores de hiper parâmetros como GridSearchCV ou RandomizedSearchCV poderiam ter nos ajudado nessa tarefa.</p>

<p>Coleta de dados: Ao longo do percurso da construção dos modelos de machine learning, foi percebida uma dificuldade que agora parece bastante evidente: coleta de dados é uma tarefa árdua, e muitas vezes impossível a depender da proposta do projeto e investimento. Nossa proposta envolvia, desde o princípio, recolher dados que refletiam a qualidade dos hospitais, e nos deparamos com uma barreira: Estes dados hora são sigilosos, outrora possuem baixa qualidade, mas nunca é ideal, e isto reforça a ideia de que acumular um banco de dados é uma das tarefas mais difíceis do processo.
<br>Para resolver este impasse, buscamos proxys, utilizando fontes como sites de reclamações do consumidor, que poderiam direcionar sobre a qualidade do hospital, mas ao mesmo tempo o sentimento do consumidor poderia ser diferente da realidade. Então se tratando do aprendizado extraído desse tópico, fica evidente a importância de estar disposto a investir tempo e recursos (até financeiros) em uma coleta de dados com o maior grau de confiança possível. Em virtude do escopo e proposta do projeto, seria inviável prosseguir por este caminho.</p>

<p>Variedade de dados: A variedade dos dados se mostrou fundamental, assim como o esperado, mas fomos surpreendidos uma vez que nos deparamos com respostas enviesadas em alguns testes, mostrando que, embora o modelo criado seguisse o caminho para o qual foi direcionado, a depender da combinação de entradas nos testes, obteríamos um resultado que não reflete a realidade. Para esta dificuldade a solução passa a ser uma quantidade de dados cada vez maior e dividida de forma heterogênea entre as categorias, para minimizar o impacto do viés que uma categoria possa causar.</p>


<p>O que foi aprendido:
<br>•	A importância de usar visualizações e relatórios de avaliação detalhados para entender a performance do modelo;
<br>•	Coletar dados é uma tarefa trabalhosa e fundamental;
<br>•	O uso de técnicas de pré-processamento e a seleção de métricas de avaliação são fundamentais para um bom desempenho do pipeline.</p>

Planos futuros: 

<p><br>Incorporação de Novos Algoritmos e Técnicas Avançadas: Uso de modelos ensemble (Random Forest, Gradient Boosting) e deep learning com TensorFlow/PyTorch para melhorar a precisão e generalização.

<br>Otimização de Hiperparâmetros: Implementação de GridSearchCV e RandomizedSearchCV para busca de hiperparâmetros. Uso de técnicas de otimização bayesiana, como Optuna, para eficiência.

<br>Melhoria na Preparação e Engenharia de Features: Criação de variáveis derivadas e seleção de variáveis com técnicas como RFE e SelectKBest. Uso de pipelines automatizados com scikit-learn para consistência no pré-processamento.
<br>Validação e Acompanhamento: Validação cruzada com K-fold e estratificação. Dashboards de monitoramento com Dash ou Streamlit para avaliar a performance em produção.

<br>Integração e Escalabilidade: Uso de serviços em cloud (AWS, Google Cloud, Azure). Paralelização com Dask/Spark e uso de Docker/Kubernetes para escalabilidade.

<br>Adaptação e Customização para Diferentes Cenários: Fluxos de aprendizado contínuo para adaptação. Personalização para diferentes segmentos de dados.</p>

<br>Em suma, o produto final mostra um pipeline coerente que vai da importação dos dados até a avaliação do modelo. No entanto, há espaço para aprofundar a análise de variáveis e otimizações. Adotar mais técnicas de engenharia de características e adicionar capacidade de processamento de escalabilidade contínua para lidar com volume crescentes de dados podem ser melhorias futuras para o projeto.
