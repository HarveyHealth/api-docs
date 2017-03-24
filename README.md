Generate API Blueprint file from Postman Collection:
docker run --rm -it -v "$PWD:/opt" phillippohlandt/pmtoapib -collection Harvey.postman_collection.json

Run aglio server
aglio -i Harvey.apib --theme-template triple -o output.html --server
