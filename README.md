Copy of Mohit Arora's code to manage docker containers
https://medium.com/@mohitarora/manage-docker-containers-using-coreos-part-4-b292841c207f

# Build Docker image by [Packer](http://www.packer.io/)

## How to run

Install Docker and Packer and execute the following commands

```
$ packer validate ubuntu-base.json
$ packer build -var 'version=v1.0.0' ubuntu-base.json
```
Once packer creates the container, ansible provisions the container. Once container is provisioned, an image is created and pushed to docker index.



