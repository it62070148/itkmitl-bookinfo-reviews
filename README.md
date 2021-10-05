# How to run product page

## Prerequisite

* Java

```bash
/opt/ibm/wlp/bin/installUtility install  --acceptLicense /opt/ibm/wlp/usr/servers/defaultServer/server.xml
```

## How to run with Docker

```bash
# Build Docker Image for reviews service
docker build -t reviews .

# Run reviews service on port 8082
docker run -d --name reviews -p 8082:9080 -e ENABLE_RATINGS=true reviews
```

* Test with with path /reviews/1 and `/health`