# algolia-docsearch-indexer
POC for Running own crawlers using Docsearch and Algolia

## Pre-requisites

Follow the instructions as specified here: https://docsearch.algolia.com/docs/run-your-own/

## Run the indexer

Run `docker run -it --env-file=.env -e "CONFIG=$(cat config.json | jq -r tostring)" algolia/docsearch-scraper`


## For running projects separately (not required)

Run `docker run -it --env-file=.env -e "CONFIG=$(cat graphql-tools.json | jq -r tostring)" algolia/docsearch-scraper`

Run `docker run -it --env-file=.env -e "CONFIG=$(cat graphql-mesh.json | jq -r tostring)" algolia/docsearch-scraper`