# algolia-docsearch-indexer
POC for Running own crawlers using Docsearch and Algolia

## Pre-requisites

Follow the instructions as specified here: https://docsearch.algolia.com/docs/run-your-own/

## Run the indexer

Run `docker run -it --env-file=.env -e "CONFIG=$(cat config.json | jq -r tostring)" algolia/docsearch-scraper`