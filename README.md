# Avaliação P2

#### Nome: Patricia Honorato Moreira
#### Turma: 2° ano de engenharia da computação

### Configuração da Instância do frontend

A configuração da instância foi feita pelo terminal do computador no Ubuntu. Nela foi instalado o Apache Server e clonado o repositório do github com os códigos alterados. 
![EC2 front](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/instancia%20front.png)

### Configuração da Instância do backend

Para a configuração da instância do backend, foi-se necessário clonar o repositório do github, realizar a instalação do arquivo requirements.txt e uvicorn. 
![EC2 backend](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/instanci%20back.png)

### Configuração do Banco de Dados RDS

O Banco de dados em RDS foi criado em postgres.

![banco 1](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/instancia%20front.png)
![banco 2](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/rds.png)


### Alteração dos script

1) main.py
No código main.py foi-se alterado as credenciais e link para acesso do banco de dados

2) criar_banco.py

Nesse arquivo foi adicionado o trecho de código "con.commit()" para permitir a criação do banco de dados sem ser apenas manualmente pelo dbeaver. 

2) script.js

Foi alterado o IP da máquina (instância do frontend) em cada rota.

### Rodando a instância para ter acesso ao projeto

É necessário inicializar a instância do backend (ec2-52-90-245-186.compute-1.amazonaws.com) com o comando: `uvicorn main:app --host 0.0.0.0` após estar na pasta do repositório no terminal do ubuntu. A instância funciona na porta 8000. 

![Uvicorn](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/uvicorn%20running.png)

![Uvicorn](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/Untitled%20presentation.png)

Com a instância funcionando é so repetir o mesmo processo para a instância do front end (ec2-54-152-183-17.compute-1.amazonaws.com) 

Em seguida o projeto estará disponível conforme mostrado abaixo. Suas principais funcionalidades é permitir que o usuário apague e adicione notas na interface. 

![interface2](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/Untitled%20presentation%20(2).png)

![interface](https://github.com/ipatriciahonorato/Avaliacao-P2-M7-2023-EC/blob/main/media/Untitled%20presentation%20(1).png)




