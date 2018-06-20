---
name: Europeana
x-slug: europeana
description: Explore 51,990,182 artworks, artefacts, books, videos and sounds from
  more than 3,500 museums, galleries, libraries and archives across Europe.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
x-kinRank: "9"
x-alexaRank: "68066"
tags: Europeana
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/apis.md
specificationVersion: "0.14"
apis:
- name: Europeana get information about a specific dataset
  x-api-slug: europeana
  description: Get information about a specific dataset.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///dataset/{id}.json
  tags: Dataset,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/datasetid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/datasetid-json-get-openapi.md
- name: Europeana get the list of Europeana datasets
  x-api-slug: europeana
  description: Get the list of europeana datasets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///datasets.json
  tags: Datasets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/datasets-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/datasets-json-get-openapi.md
- name: Europeana basic search function following the OpenSearch specification
  x-api-slug: europeana
  description: Basic search function following the opensearch specification.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///opensearch.rss
  tags: Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/opensearch-rss-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/opensearch-rss-get-openapi.md
- name: Europeana get information about a specific Europeana provider
  x-api-slug: europeana
  description: Get information about a specific europeana provider.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///provider/{id}.json
  tags: Provider
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/providerid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/providerid-json-get-openapi.md
- name: Europeana get the list of datasets provided by a specific provider
  x-api-slug: europeana
  description: Get the list of datasets provided by a specific provider.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///provider/{id}/datasets.json
  tags: Providers,Datasets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/provideriddatasets-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/provideriddatasets-json-get-openapi.md
- name: Europeana get the list of Europeana data providers
  x-api-slug: europeana
  description: Get the list of europeana data providers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///providers.json
  tags: Providers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/providers-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/providers-json-get-openapi.md
- name: Europeana get a single record in JSON format
  x-api-slug: europeana
  description: Get a single record in json format.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///record/{collectionId}/{recordId}.json
  tags: Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/recordcollectionidrecordid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/recordcollectionidrecordid-json-get-openapi.md
- name: Europeana get single record in JSON LD format
  x-api-slug: europeana
  description: Get single record in json ld format.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///record/{collectionId}/{recordId}.jsonld
  tags: Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/recordcollectionidrecordid-jsonld-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/recordcollectionidrecordid-jsonld-get-openapi.md
- name: Europeana get single record in RDF format)
  x-api-slug: europeana
  description: Get single record in rdf format).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///record/{collectionId}/{recordId}.rdf
  tags: Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/recordcollectionidrecordid-rdf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/recordcollectionidrecordid-rdf-get-openapi.md
- name: Europeana search for records
  x-api-slug: europeana
  description: Search for records.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///search.json
  tags: Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/search-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/search-json-get-openapi.md
- name: Europeana Google Fieldtrip formatted RSS of selected collections
  x-api-slug: europeana
  description: Google fieldtrip formatted rss of selected collections.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///search.rss
  tags: Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/search-rss-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/search-rss-get-openapi.md
- name: Europeana get autocompletion recommendations for search queries
  x-api-slug: europeana
  description: Get autocompletion recommendations for search queries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///suggestions.json
  tags: Suggestions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/suggestions-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/suggestions-json-get-openapi.md
- name: Europeana translate a term to different languages
  x-api-slug: europeana
  description: Translate a term to different languages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2///translateQuery.json
  tags: Translations,Query
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/translatequery-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/translatequery-json-get-openapi.md
- name: Europeana
  x-api-slug: europeana
  description: Explore 51,990,182 artworks, artefacts, books, videos and sounds from
    more than 3,500 museums, galleries, libraries and archives across Europe.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/777-europeana.jpg
  humanURL: http://europeana.eu/portal/
  baseURL: https://www.europeana.eu/v2/
  tags: Europeana
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/europeana/master/_listings/europeana/openapi.md
x-common:
- type: x-base
  url: http://www.europeana.eu/api/
- type: x-blog
  url: http://blog.europeana.eu/
- type: x-blog-rss
  url: http://blog.europeana.eu/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/europeana
- type: x-developer
  url: http://europeana.eu/portal/api-introduction.html
- type: x-github
  url: https://github.com/europeana
- type: x-twitter
  url: https://twitter.com/EuropeanaEU
- type: x-website
  url: http://europeana.eu/portal/
- type: x-website
  url: http://europeana.eu
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---