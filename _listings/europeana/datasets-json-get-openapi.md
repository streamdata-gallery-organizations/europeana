---
swagger: "2.0"
x-collection-name: Europeana
x-complete: 0
info:
  title: Europeana get the list of Europeana datasets
  description: Get the list of europeana datasets.
  termsOfService: http://www.europeana.eu/portal/en/rights.html
  contact:
    name: http://labs.europeana.eu/api
  version: 1.0.0
host: www.europeana.eu
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dataset/{id}.json:
    get:
      summary: get information about a specific dataset
      description: Get information about a specific dataset.
      operationId: getDataset
      x-api-path-slug: datasetid-json-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: path
        name: id
        description: id
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Dataset
      - Id
  /datasets.json:
    get:
      summary: get the list of Europeana datasets
      description: Get the list of europeana datasets.
      operationId: listDatasets
      x-api-path-slug: datasets-json-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: query
        name: countryCode
        description: countryCode
      - in: query
        name: edmDatasetName
        description: edmDatasetName
      - in: query
        name: offset
        description: offset
      - in: query
        name: pagesize
        description: pagesize
      - in: query
        name: status
        description: status
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Datasets
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---