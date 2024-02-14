# Elastic Stack

This is adapted from the excellent [elastdocker](https://github.com/sherifabdlnaby/elastdocker/tree/main) docker template.

## Quick start

If running locally, edit the `.env` file and add values for `ELASTIC_PASSWORD` and `ELASTIC_APM_SECRET_TOKEN`.

```sh

# Create data directory
mkdir -p data/elasticsearch

# Setup certs
docker-compose -f docker-compose.setup.yml run --rm certs
docker-compose -f docker-compose.setup.yml run --rm keystore

# Run
docker-compose up -d
```
