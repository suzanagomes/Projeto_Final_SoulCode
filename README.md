# Projeto_Final_SoulCode
ETL e análise de dois datasets sobe Crimes

<aside>
🚀 **A Empresa:**

A **Mindful Data,** empresa de consultoria da área de engenharia de dados, fundada por nós, alunos recém formados do curso de **Engenharia de Dados** da **Soul Code Academy,** tem a proposta de atender à demanda de empresas no que se trata de:

- Data Migration;
- Processos de ETL;
- Produção de insights e dashboards para apoiar decisões de negócios;

Nosso **squad** é composto por:

</aside>
![3.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e3118646-ce44-4d71-9d28-9585359c9da2/3.png)

![Design sem nome (1).png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ef78bf14-e393-460d-93b0-377dfc5a18c9/Design_sem_nome_(1).png)

![2.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8c39b4c0-2e0b-4e8d-93c8-3d306887edc3/2.png)

![4.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/72559785-117d-443a-a1f8-aa66b4c116cb/4.png)

## Os Requisitos

<aside>
⭐ **Diretrizes:**

Nosso projeto seguiu as diretrizes determinada pelos professores do curso de engenharia de dados da SoulCode Academy e fora orientado pelo professor **Igor Gondim.** 

Os requisitos estão descritos logo abaixo:

[Requisitos do projeto](https://www.notion.so/Requisitos-do-projeto-7d9f86f72b5943e88e9c6c0ce9970a88)

</aside>

## O Projeto

<aside>
📌 **Definição dos objetivos:**

A partir do tema, passamos a etapa de definição dos objetivos e criação de insights preliminares para atender às expectativas das diretrizes passadas pelo proposto do projeto.

Essa etapa está contida aqui:

[**Objetivos e organização das ideias gerais**](https://www.notion.so/Objetivos-e-organiza-o-das-ideias-gerais-c971c8ee5b464d53a76c2474b5f3a1ac)

📊 **Tema escolhido com objetivo geral**:

> Estudo dos casos de crimes envolvendo mortes entre as cidades de **Nova York** e **São Paulo**
> 

📑 **Objetivos específicos:**

- Traçar o perfil das vítimas
- Mapear quais locais mais violentos
- Evolução da quantidade de crimes de acordo com o período

📈**Insights a serem resolvidos:**

1. Qual o total de ocorrências das duas cidades?
2. Ranking dos tipos de crime campeãs em ocorrências
3. Qual o período do dia com maior número de ocorrências?
4. Laço temporal dos crimes por ano e mês
5. Número de ocorrências por cor da pele e sexo
6. Quais as regiões (bairros ou distritos) mais perigosos?
</aside>

## O Processo de ETL

<aside>
📌 **Workflow**

Todo nosso processo está descrito no modelo abaixo, passando por todos os tópicos solicitados nas diretrizes do projeto.

![WhatsApp Image 2023-01-16 at 17.01.02.jpeg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c588b1f8-1273-4620-8369-9a0a0831b3cc/WhatsApp_Image_2023-01-16_at_17.01.02.jpeg)

📄**Definição das bases de dados**

Com os objetivos traçados, começamos a busca das bases de dados que utilizaremos. Nos dividimos na busca e encontramos dados oficiais de ambas as cidades disponíveis publicamente. 

Para melhorar o entendimento, a partir daqui trataremos ambas as cidades de forma paralela para facilitar a construção do raciocínio.

### **São Paulo**

**Fonte de dados:**

Os dados foram tirados do Portal transparência do Governo do Estado de São Paulo e filtrado apenas os crimes com homicídios para a cidade de São Paulo, dos anos de 2018 a 2021.

[Segurança Pública - Transparência](http://www.ssp.sp.gov.br/transparenciassp/Consulta.aspx)

### **Nova York**

**Fonte de dados:**

Os dados escolhidos estão disponíveis no site **NYC Open Data**, administrado pelos órgão públicos da cidade de **Nova York** (**USA)**, onde filtramos as ocorrências que tiveram homicídios entre os anos de 2018 a 2021.

[NYPD Complaint Data Historic | NYC Open Data](https://data.cityofnewyork.us/Public-Safety/NYPD-Complaint-Data-Historic/qgea-i56i)

**Tratamentos dos dados**

Abaixo estão descritos todo o passo a passo desde a extração, até a união dos datasets de SP e NY já tratados.

**DataSet Original SP:** 

[Google Colaboratory](https://colab.research.google.com/drive/1eV38I-n5OIjpW3-0Sq5ZufqgKW2t4xcm#scrollTo=vlvmxhs9gz3i)

**DataSet Tratado SP:**

[Google Colaboratory](https://colab.research.google.com/drive/13qLkbFJe_wSJGXic6iynm9PdZQha2qqc?usp=sharing#scrollTo=YJi1DahFj2JA)

**DataSet Original NY:** 

[Google Colaboratory](https://colab.research.google.com/drive/1SaJsTqgnlMG1bhi3EAuSWcgQbvKC_9HN?usp=sharing)

**DataSet Tratado NY:**

[Google Colaboratory](https://colab.research.google.com/drive/18xT-9DM1DLl5xQUe94PORFBuSxu8JbRa?usp=sharing)

**Data Frame juntando os dados de SP e NY:**

[Google Colaboratory](https://colab.research.google.com/drive/10DKEuS-6YmLVSqLintBcaIJbX1kr-85A?usp=sharing)

**Envio do DataSet tratado ao BigQuery via Apache Beam:**

[Google Colaboratory](https://colab.research.google.com/drive/1_AGCOsc5T1UfPD9jaMlxC7f-F0B2FCJH?usp=sharing)

</aside>

## Data Visualization

<aside>
📈 **BigQuery**
Após realizar todos os tratamentos necessários e salvar os dados nos Data Lakes (**Cloud Storage** e **MongoDB**), puxamos os dados para o BigQuery, onde fizemos os últimos ajustes e algumas queries para constatar se nosso dados atendiam ao nosso objetivo antes do envio ao Looker Studio.

**Dashboard Looker Studio**

[Dashboard-Projeto Final](https://datastudio.google.com/reporting/2ecaecd3-dde9-4171-8a27-c5c589a6daed)

</aside>

## Apresentação

<aside>
🎞️ **Apresentação Grupo 1 - Crimes:**

No card abaixo está nossa apresentação de slides, neste documento traremos mais detalhes sobre todo o processo.
  
[Apresentacao-Projeto Final](https://docs.google.com/presentation/d/1MOZrRZjA0osVoUOXwtIEGe0eB5-IHpQPyh5FzGpo74U/edit#slide=id.g1c679854a04_0_2587)

</aside>
