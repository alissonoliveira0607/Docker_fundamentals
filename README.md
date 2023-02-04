# Containers - Aplicações

Criando um ambiente virtual no Linux

Se o pip não estiver no seu sistema

$ sudo apt-get install python-pip
Em seguida, instale virtualenv


$ pip install virtualenv
Agora verifique sua instalação

$ virtualenv --version
Crie um ambiente virtual agora,

$ virtualenv virtualenv_name
Após este comando, uma pasta chamada virtualenv_name será criada. Você pode nomear qualquer coisa para ele. Se você deseja criar um virtualenv para uma versão específica do python, digite

$ virtualenv -p /usr/bin/python3 virtualenv_name
ou

$ virtualenv -p /usr/bin/python2.7 virtualenv_name
Agora, finalmente, só precisamos ativá-lo, usando o comando

$ source virtualenv_name/bin/activate
Agora você está em um ambiente virtual Python

Você pode desativar usando

$ deactivate

instalando os requirements
- pip install -r requirements.txt


Dependências gerenciador de pacotes do python
- apt install python3-pip -y
- pip3 install -r requirements.txt


Para executar o flask para que escute em todas as interfaces de rede basta passar os seguintes parametros -h
- flask run -h 0.0.0.0

Setando as variaveis e iniciando aplicação
DB_HOST=172.17.0.2 DB_USER=devops DB_PASS=4linux DB_NAME=container flask run -h 0.0.0.0


