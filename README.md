# Concourse Example

An attempt to build out a simple but well-featured Concourse example

## Installing Locally

1. Download and install a Concourse instance:
```
wget https://concourse-ci.org/docker-compose.yml
docker-compose up -d
```

2. Visit http://localhost:8080
3. Download `fly` from this page

## Setting up sample pipelines

* `fly -t test set-pipeline --config ci/pipelines/production-monitoring.yml --load-vars-from ci/secrets.yml --pipeline production-monitoring`