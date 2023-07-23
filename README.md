# Curso AWS Data Analytics for IoT

###  Quais as soluções AWS estudadas? e o que cada uma atende?

1. Store data in Amazon S3

2. Query Data in Amazon Athena

    Busca de grande volumes de dados

3. Query data in Amazon S3 with Amazon Athena and AWS Glue

4. Analyze Data with Amazon Redshift

    Busca de grande volumes de dados utilizando clusters de containers

5. Analyze Data with Amazon Sagemaker, Jupyter Notebooks and Bokeh

6. Automate Loading Data with the AWS Data Pipeline

7. Analyze Streaming Data with Amazon Kinesis Data Firehose, Amazon Elasticsearch Service, and Kibana

    No capítulo 7 deste curso, aprendemos sobre como capturar os dados de stream, prepará-los para uma análise e exibir os resultados em gráficos. O Amazon Kinesis Data Firehose é o responsável pela captura dos dados de stream, que são dados que vão usar um dos 5 V's comentados durante o curso: a velocidade. 
    
    O Stream possui dados que precisam ser tratados em tempo real, como os vídeos e os logs de servidores web por exemplo. O Firehose também servirá como um injetor de dados que serão recebidos através do Elastic Searsh, ao qual será a ponte entre o Kinesis e o Kibana, que exibirá os dados em gráficos. 

    Alguns serviços da Amazon tiveram seus nomes alterados, como é o caso do Elastic Search. Por ser um serviço que possui a patente desse nome, a AWS criou o seu produto "open source" chamado Amazon OpenSearch Service.

8.

### Explique três exemplos de atividades que você realizou no laboratório prático?

1. Capítulo 7

A prática deste capítulo propõe a captura de logs de um servidor web em dois navegadores diferentes enquanto se navega entre as suas páginas, utilizando o Amazon Kinesis Data Firehose Service, injetando esses dados no Amazon Elastic Search Service, e preparando a visualização desses dados no Kibana. 

O aws forcene instâncias de servidores e uma delas é a demo do kibana. Nas suas propriedades de rede podemos pegar o seu IPV4 público e fazer o login com as credências fornecidas pelo capítulo atual do curso. Após o lógin, utilizamos textos que informam o methodo http utlizado e dados do tipos json, para excluir logs antigos do servidor web e acrescentar as novas pesquisas. Esses dados contêm os campos e valores aos quais serão montados nos gráficos do Kibana. No Kibana, escolhemos as cores, qual o tipo de gráfico e os campos/valores que serão exibidos. 

### Quais as principais lições apreendidas do curso?

Com o curso de análise de dados da AWS é possível perceber que existem diversos tipos de dados e várias formas de análisar os mesmo. As ferramentas da AWS apresentadas nesse curso mostram algumas dessas análises e tipos de dados: análise mais rápida(stream e Kinesis), análise mais robusta, de volume (Redshift e Athena), dados do tipo json, logs, entre outros. 

Muitas das vezes pra quem apenas cria um gráfico que possa mostrar alguns dados não se pensa em porque esses dados precisam ser exibidos, não vê como um investidor na bolsa, um dono de uma empresa de produção de carros, um gestor de uma fabrica de tecidos, etc. Sendo essa análise mais rápida, com uma quantidade maior de dados e sendo estes com uma finalidade escolhida a dedo por analistas de dados, faz uma grande diferença na hora de uma produção ou de uma compra de insumos por exemplo. 

Dados são coletados e gerados a todos os momentos e eles precisam ser analisados. O melhor uso das ferramentas ou mesmo do SGBD com o sql/NoSql pode mudar muito a vida de grandes empresas e empresários. 