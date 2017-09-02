 

# **Mongo-Jupyter-PyMongo**
#### Interagindo com o Mongo DB usando Jupyter Notebook e PyMongo 


Este repositório é dedicado à reunião de referências, material de apoio e exemplos relacionados à interação com Mongo DB utilizando o módulo PyMongo e Jupyter Notebook. 

-----------

# Mongo DB

Mongo DB é um banco de dados NoSQL (<i>Not only Sequence Query Language</i> ou Não somente SQL ou Não Relacional), orientado a documentos {1}, livre de <i>schema</i> {2}, passível de escalabilidade horizontal {3} e de código aberto {4}. Por sua flexibilidade, bom desempenho e simplicidade na construção das <i> querys </i>, o Mongo é uma ferramenta bem indicada à aplicação em análise de dados e <i> big data </i>. 

**{1}** No Mongo DB os dados são armazenados em **coleções** de **documentos**. Em analogia ao modelo relacional, a coleção equivale a uma tabela, o documento a uma linha da tabela e os **campos** do documento aos valores nas colunas dessa mesma tabela. Mongo DB utiliza documentos  em [**JSON**](http://www.json.org/) (o armazenamento é feito em [BSON](http://bsonspec.org/) - Binary JSON). Exemplo de documento em JSON:

    {
	    "_id": 1,
	    "name": "Joe",
	    "age": 32,
	    "job_area": ["IT", "engineering"],
	    "location": {
		    "city": "São Paulo",
		    "country": "Brazil"
	    }
    }

**{2}** Os documentos armazenados no Mongo DB podem ter campos distintos uns dos outros. É possível adicionar novos documentos com campos ainda não conhecidos pela coleção, o que não pode ser feito em bancos com <i> schema </i> rígido (bancos SQL).

**{3}** A performance de bancos em Mongo DB está associada à qualidade do hardware e tamanho do cluster. É possível melhorar o desempenho (velocidade das consultas) do banco ou aumentar o espaço disponível para armazenamento ao adicionarmos novas máquinas ao cluster (escalabilidade horizontal). A utilização do cluster Mongo DB também nos permite configurar esquemas de redundância, dando maior confiabilidade ao bancos de dados.

<a href="https://docs.mongodb.com/v3.0/core/sharding-introduction"> 
Cluster Mongo DB
<img src="https://docs.mongodb.com/v3.0/_images/sharded-collection.png" alt="Cluster Mongo DB">
</a>

 
**{4}** O Mongo DB é escrito em C++ e [é possível acessar o seu código fonte através da web](https://github.com/mongodb/mongo).

#### Mais Informações

- [Mongo DB: Documentação](https://docs.mongodb.com/manual/introduction/)

- [Manual de instalação do Mongo DB](https://docs.mongodb.com/manual/installation/)

- [Material de apoio: Mongo DB University](https://university.mongodb.com/) 

-----------

# Jupyter Notebook



#### Anaconda


- [Project Jupyter](http://jupyter.org/)

- [Download e instalação do Anaconda](https://www.anaconda.com/download/)

-----------

# PyMongo

 

- Instalação do módulo PyMongo através do Anaconda: https://anaconda.org/anaconda/pymongo

- Documentação: https://api.mongodb.com/python/current/

-----------

# Exemplos


