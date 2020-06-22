# Teste Engenheiro de Dados - DataSprints

Este material é parte do processo de seleção para Engenheiros de Dados na DataSprints. 

Para este desafio foi disponibilizado 3 conjuntos de dados contendo:
- dados sobre corridas de Taxi na cidade de New York ocorridas entre 2009 e 2012;
- empresas de Taxi;
- Prefixos e os tipos de pagamento.

Este repositório contém a resolução dos Quesistos Mínimos e dos Quesistos bônus.


## Instruções para Reprodução de Análises
Para reprodução local, é necessario o Python ^3.5.

Na pasta principal do repositorio, execute o seguinte comando para execução dos desafios:

```python desafio.py```

Será criado uma pasta '/output' com os resultados das Questões 1 à 6.

Para reprodução das análises passo a passo, abrir o arquivo desafio.ipynb através do Jupyter Notebbok.

```jupyter notebook desafio.ipynb```

Todo o conteúdo do desafio pode ser visualizado no browser abrindo o arquivo 'Analise.html'.

 
### Processamento em Cluster
O arquivo "/cluster/AWS.ipynb" contém uma sequencia de configuração dos servidos da Amazon (S3, Group Resource, EMR) para a criação de um cluster Spark On-Demand formado por um Master e dois Slaves.

A execução deste script requer que o Engenheiro de Dados possua uma conta ativa na AWS e que possua configurado localmente o AWS CLI. 

Esta execução pode causar COBRANÇA da AWS pelo uso dos serviços. É necessario observar o tempo de duração dos serviços para não causar prejuízo. Para efeito de referencia, durante os meus testes, a configuração e a utilização do cluster levou no melhor tempo 8 minutos e no pior tempo cerca de 20 minutos.

Foi criado um step no cluster da EMR para a execução do Script Python. A entrada de dados, o script pyspark e a saída parquet todos foram armazenados no bucket S3.

