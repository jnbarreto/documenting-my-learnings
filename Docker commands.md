*Docker commands:

permissão:
sudo usermod -aG docker $USER
sudo chown "$USER":"$USER" /home/"$USER"/.docker -R
sudo chmod g+rwx "$HOME/.docker" -R

docker run (container) = executa um container
docker ps = lista os containers.
docker ps -a = mostra todos os container que foram usado.
docker ps -a -q =lista somente os ids dos containers.
docker rm $(docker ps -a -q) -f = remove todos os containers.
--name = nomeia o container.
-d = deixa o container rodando desaclopado do terminal.
-p 8080:80 = define a porta sendo o primeiro parametro a porta a ser rodada e o segundo o padrão do container. obs: a porta tem que estar livre para ser usada.
docker rm (nome ou id container)= remove o container/ deleta.
-f = force.
docker exec -it (nome_container) (nome do commando, ex: bash)= escreve dentro do container.
docker run --mount type=bind,source="$(pwd)"/html,target=/user/share/nginx/html nginx = exemplo com nginx, monta uma pasta do seu computador para dentro do container.(bind mount)
-it = interage com o container

VOLUME
docker run -d -v "$(pwd)"/html:/user/share/nginx/html nginx = faz a mesma coisa que o --mount só q ue SE(if) não tiver a pasta no seu computador ele vai criar a pasta.
docker run --name nginx -d --mount type=volume,source=nameVolume,target=/app nginx =criando volumes.
docker run --name nginx -d -v nameVolume:/app nginx = criando volumes.
docker volume prune = remove todos os volumes.
docker system prune -fa --volumes

IMAGES
docker images = mostra todas as imagens docker baixadas.
docker rmi (imagem): (tag) = remove imagem. ex:docker rmi php:latest.
docker build -t leonejn/nginx-com-vim:latest . = constroi sua propria img.

DOCKERFILE
FROM (IMAGEM):LATEST = define qual imagem vc vai utilizar
WORKDIR /app = diretório que vai ser trabalhado dentro do container
RUN apt-get update = executa comandos dentro da img
COPY html/ /usr/share/nginx/html = copia o conteudo da pasta html para dentro da pasta html do container.
CMD - ENTRYPOINT = diferença entre eles é que o entrypoint é fixo não é alterado já o CMD pode ser trocado por outro "parametro"
ex:
 ENTRYPOINT ['echo', 'hello']
 CMD ['world']
run commando sem parametro
no terminal vai ser exibido hello world
mas se rodar com parametro vai retornar o parametro no lugar do cmd
run commando com parametro leone
no terminal vai ser exibido hello leone

NETWORK
formatos
-bridge -host -overlay -maclan -none.
ps: network default é a bridge.

docker network ls = lista todos os networks.
docker network inspect minharede = inspeciona a rede.
docker network prune = remove todos os networks.
docker network create --driver bridge minharede = Cria um network.
docker run -dit --name ubuntu --network minharede bash = roda o container com o network.
docker network connect minharede ubuntu = conecta o container em uma rede.
docker logs container = log do container.








