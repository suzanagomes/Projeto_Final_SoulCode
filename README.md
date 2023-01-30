**Projeto final do curso de Engenharia de dados da SoulCode Academy**
- **Autores:** Suzana Gomes, Anderson Calasans, Giovana de Brito, Wilbert Silva
 - **Data de entrega:** January 17, 2023
 - **Resumo:** Projeto final  do curso de engenharia de dados da SoulCode Academy, com relevância na área de crimes (segurança pública), que mostra um estudo comparativo entre as cidades de São Paulo (Brasil) e New York (United States of America) quanto ao número de casos de crimes envolvendo homicídios e os dados envolvendo este tipo de ocorrência.
 - **Status:** Finalizado
 - **Tema:** Crimes (Segurança Pública)
 - **Type:** Projeto Final - Soul Code
 - **Área de estudo:** ETL, Engenharia de dados, GCP, MongoDB, MySQL, Python, SQL
 
<aside>
🚀 **A Empresa:**

A **Mindful Data,** empresa de consultoria da área de engenharia de dados, fundada por nós, alunos recém formados do curso de **Engenharia de Dados** da **Soul Code Academy,** tem a proposta de atender à demanda de empresas no que se trata de:

- Data Migration;
- Processos de ETL;
- Produção de insights e dashboards para apoiar decisões de negócios;

</aside>


 

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

![Workflow](https://github.com/suzanagomes/Projeto_Final_SoulCode/blob/b56ecd7926aec633cc33450fe470509ca5b858dc/Workflow%20-%20CRIMES_NY_SP.png)

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
[Notion](https://www.notion.so/Mindful-Data-Consultoria-d495964059c34acb9c8fe3d21dbb5cf6)



</aside>
