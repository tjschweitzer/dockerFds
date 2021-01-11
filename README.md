# dockerFds


docker rm -f $(docker ps -aq)


docker build -t tjschweitzer/landfirefds .
docker run --name test --rm  -it --network=host   tjschweitzer/landfirefds

docker push tjschweitzer/landfirefds

