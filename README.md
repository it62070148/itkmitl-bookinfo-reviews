# How to run Reviews service

## Prerequisite

* Java lastest



## How to run with Docker

```bash
# Build Docker Image for reviews service
docker build -t reviews .

# Run reviews service on port 8082
docker run -d --name reviews -p 8082:9080 -e ENABLE_RATINGS=true reviews
```

* Test with with path /reviews/1 and `/health`