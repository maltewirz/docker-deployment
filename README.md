```shell
# Local:
docker build -t node-dep-example .

docker run -d --rm --name node-dep -p 80:80 node-dep-example

docker tag node-dep-example maltewirz/node-example

docker push maltewirz/node-example

# Remote:
# Update Images:
sudo docker pull maltewirz/node-example
# Run Images
sudo docker run -d --rm -p 80:80 maltewirz/node-example
 
 ```