# INTRODUÇÃO
Este projeto tem como objetivo desenvolver uma aplicação CRUD para gerenciar dados de clientes utilizando o banco de dados NoSQL MongoDB, a biblioteca Streamlit para criação de interface web interativa e o uso de Docker para conteinerização.

# FUNCIONALIDADES
- Visualizar clientes cadastrados
- Cadastrar novos clientes
- Atualizar informações (nome, e-mail e telefone)
- Deletar registros
- Geração automática de mais de 1 milhão de clientes com a biblioteca Faker

# TECNOLOGIAS USADAS
- Python 3.11
- MongoDB
- Streamlit
- Faker
- Docker e Docker Compose

# ESTRUTURA DO TRABALHO
- app.py
- docker.yml
- dockerfile
- gerar_dados.py
- requirements.txt

## EXECUÇÃO
# Clonagem do repositório no GitHub
git clone https://github.com/AlessandraEsser78/eshop_nosql.git
cd e-shop

# Gerar dados falsos
python gerar_dados.py

# Subir a Aplicação com Docker
docker-compose up --build
# Acessar a interface no navegador
http://localhost:8501

## Docker Compose
O arquivo docker-compose.yml sobe dois serviços:
mongo: container com MongoDB
streamlit-app: aplicação Streamlit conectada ao banco



