docker login
docker build -t vogsy/datastore-viewer --file dockerfile.vogsy .

docker tag vogsy/datastore-viewer vogsy/datastore-viewer:latest

docker push vogsy/datastore-viewer:latest

docker run -it vogsy/datastore-viewer /bin/bash