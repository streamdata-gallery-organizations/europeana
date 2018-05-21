---
swagger: "2.0"
x-collection-name: Europeana
x-complete: 0
info:
  title: Europeana get single record in JSON LD format
  description: Get single record in json ld format.
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
      x-api-path-slug: datasetidjson-get
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
      x-api-path-slug: datasetsjson-get
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
  /opensearch.rss:
    get:
      summary: basic search function following the OpenSearch specification
      description: Basic search function following the opensearch specification.
      operationId: openSearch
      x-api-path-slug: opensearchrss-get
      parameters:
      - in: query
        name: count
        description: count
      - in: query
        name: searchTerms
        description: searchTerms
      - in: query
        name: startIndex
        description: startIndex
      responses:
        200:
          description: OK
      tags:
      - Search
  /provider/{id}.json:
    get:
      summary: get information about a specific Europeana provider
      description: Get information about a specific europeana provider.
      operationId: getProvider
      x-api-path-slug: provideridjson-get
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
      - Provider
  /provider/{id}/datasets.json:
    get:
      summary: get the list of datasets provided by a specific provider
      description: Get the list of datasets provided by a specific provider.
      operationId: listProviderDatasets
      x-api-path-slug: provideriddatasetsjson-get
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
      - Providers
      - Datasets
  /providers.json:
    get:
      summary: get the list of Europeana data providers
      description: Get the list of europeana data providers.
      operationId: listProviders
      x-api-path-slug: providersjson-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: query
        name: countryCode
        description: countryCode
      - in: query
        name: offset
        description: offset
      - in: query
        name: pagesize
        description: pagesize
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Providers
  /record/{collectionId}/{recordId}.json:
    get:
      summary: get a single record in JSON format
      description: Get a single record in json format.
      operationId: getSingleRecordJson
      x-api-path-slug: recordcollectionidrecordidjson-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: path
        name: collectionId
        description: collectionId
      - in: query
        name: hierarchytimeout
        description: hierarchytimeout
      - in: query
        name: profile
        description: profile
      - in: path
        name: recordId
        description: recordId
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Collections
  /record/{collectionId}/{recordId}.jsonld:
    get:
      summary: get single record in JSON LD format
      description: Get single record in json ld format.
      operationId: getSingleRecordJsonLD
      x-api-path-slug: recordcollectionidrecordidjsonld-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: path
        name: collectionId
        description: collectionId
      - in: query
        name: format
        description: format
      - in: path
        name: recordId
        description: recordId
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Collections
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