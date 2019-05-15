# riskidentchallenge
This Repository contains Docker file for nginx server hosting a sample hello world kind of page. Docker file is written and index.html file is being copied inside the docker image.
Steps to build Docker Image:-
 -> docker build -f Dockerfile .
 -> docker tag <imageid> rr07/nginx:riskidentchallenge

Then the image has been pushed to my docker hub repository.

# Deployment.yaml
1. This is to deploy this nginx server inside Kubernetes, and use the above docker image created,
2. we can also use configmap to invoke custom welcome page but for now i have copied the desired default web page directly inside docker image.

# Service.yaml

This is to access the nginx server running as a pod inside kubernetes.
