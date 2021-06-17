# docker-assignment
 
apk add curl unzipFROM alpine:latest
apk add curl unzip
apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"
unzip awscli-bundle.zip
./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws



ENTRYPOINT ["aws","configure"]

