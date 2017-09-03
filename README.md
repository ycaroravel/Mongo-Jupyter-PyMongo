 

# **Mongo-Jupyter-PyMongo**
#### Interagindo com o Mongo DB usando Jupyter Notebook e PyMongo 


-----------

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
</br>
</br>
Esquema simplificado de um cluster Mongo DB (tirado [daqui](https://docs.mongodb.com/v3.0/core/sharding-introduction)):
</br>
</br>
<a href="https://docs.mongodb.com/v3.0/core/sharding-introduction"> 

<img src="https://docs.mongodb.com/v3.0/_images/sharded-collection.png" alt="Cluster Mongo DB" width="400" />

</a>

</br>
</br>
  
**{4}** O Mongo DB é escrito em C++ e [é possível acessar o seu código fonte através da web](https://github.com/mongodb/mongo).

#### Mais Informações:

- [Mongo DB - Documentação](https://docs.mongodb.com/manual/introduction/)

- [Manual de instalação do Mongo DB](https://docs.mongodb.com/manual/installation/)

- [Material de apoio: Mongo DB University](https://university.mongodb.com/) 

-----------

# Jupyter Notebook

O Jupyter Notebook provê uma interface web que nos permite criar documentos (chamados **notebooks**) que agregam texto, código e gráficos. Os códigos inseridos em notebooks do Jupyter podem ser executados na própria interface, através do seu **kernel**. Os notebooks são uma maneira elegante de documentar e explicar as etapas de preparação, processamento e extração de informações de um conjunto de dados.  Assim, ao agregar códigos e seus outputs e permitir a inserção de texto e visualização de gráficos, facilitando a interação com todas as dimensões do processo de análise de dados, o Jupyter tornou-se uma solução padrão para a área.

### Anaconda
O Jupyter Notebook está presente na instalação padrão do [Anaconda](https://docs.continuum.io/), um gerenciador de pacotes em Python que provê facilidades na obtenção e instalação de novos módulos. Instalar o Anaconda é a maneira mais comum de ter acesso ao Jupyter Notebook.

#### Mais Informações:

- [Project Jupyter](http://jupyter.org/)

- [Download e instalação do Anaconda](https://www.anaconda.com/download/)

-----------

# PyMongo

O acesso aos dados de um banco em Mongo pode ser feito diretamente através do **shell** do Mongo DB. Mas quando necessitarmos nos comunicar com o Mongo através de uma aplicação, inserindo, deletando ou consultando dados de nosso interesse, precisaremos utilizar um **driver**. Os drivers são responsáveis pela interação entre a linguagem da aplicação e o Mongo DB. Através deles nós conseguimos resgatar os dados armazenados em um banco de dados Mongo e fazê-los serem processados na nossa aplicação. Há drivers disponíveis para Mongo DB na maioria das linguagens de programação mais difundidas, dentre as quais está Python, comumente utilizada em aplicações de análise de dados em conjunto com o Jupyter Notebook. O driver de Python para Mongo é o PyMongo e ele pode ser instalado através do Anaconda.
<p>
[Instalação do módulo PyMongo através do Anaconda: ](https://anaconda.org/anaconda/pymongo)

    conda install -c anaconda pymongo 

<p>
O PyMongo consiste em um módulo com um conjunto de comandos que nos permite acessar um servidor Mongo DB, criar, editar e fazer consultas às suas bases de dados.



#### Mais Informações:

- [Mongo DB Drivers](https://docs.mongodb.com/ecosystem/drivers/)

- [PyMongo - Documentação](https://api.mongodb.com/python/current/)

-----------

### **A utilização dessas ferramentas provê um ambiente  flexível, de fácil interação e alta performance para a análise de dados.**

-----------
# Exemplos de Utilização

[IMPORTANTE] é necessário que o servidor Mongo esteja ativo. No Ubuntu, ele ser iniciado ao digitarmos o seguinte comando no terminal:

    sudo service mongod start

</br>

### - [Carregando um Cliente Mongo DB com o PyMongo](http://nbviewer.jupyter.org/github/ycaroravel/Mongo-Jupyter-PyMongo/blob/master/Example_Load_Client.ipynb)

### - [Consultas a um banco Mongo DB com o PyMongo](http://nbviewer.jupyter.org/github/ycaroravel/Mongo-Jupyter-PyMongo/blob/master/Example_Consulting.ipynb)

### - [Atualizando documentos de um banco Mongo DB com o PyMongo](http://nbviewer.jupyter.org/github/ycaroravel/Mongo-Jupyter-PyMongo/blob/master/Example_Att.ipynb)

### - [Analizando dados de um banco Mongo DB com o PyMongo](http://nbviewer.jupyter.org/github/ycaroravel/Mongo-Jupyter-PyMongo/blob/master/Example_Analytics.ipynb)


