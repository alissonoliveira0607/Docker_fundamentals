FROM alpine

#expondo a porta para a aplicação
EXPOSE 5000 

#IRÁ EXECUTAR OS COMANDO DURANTE A CRIAÇÃO DA IMAGEM PARA INSTALAR AS DEPENDÊNCIAS
RUN apk add py3-pip


#copia os arquivos do diretório atual para /opt/app
COPY . /opt/app


#instala as dependências para a aplicação
RUN pip3 install -r /opt/app/requirements.txt

#seta um diretório padrão para a imagem 
WORKDIR /opt/app

#define o comando principal do container
CMD flask run -h 0.0.0.0