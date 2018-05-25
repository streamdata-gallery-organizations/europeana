{
  "info": {
    "name": "Europeana get autocompletion recommendations for search queries",
    "_postman_id": "8a95850b-ea3f-4273-9625-1c8739374b4b",
    "description": "Get autocompletion recommendations for search queries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dataset",
      "item": [
        {
          "id": "edf48651-acb7-472b-8d72-e98fe429f7cf",
          "name": "getDataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "dataset/:id.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac06797b-c408-448f-98e3-91f5045667ca"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "e86beb48-c387-43be-b772-4ad7ba71fdfb",
          "name": "listDatasets",
          "request": {
            "url": "http://www.europeana.eu/v2/datasets.json?callback=%7B%7D&countryCode=%7B%7D&edmDatasetName=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&status=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of europeana datasets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e98f048b-0a7d-46c2-be9b-b8cca64d467e"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "0223fc30-cce3-4119-a817-d1d6edf5894a",
          "name": "openSearch",
          "request": {
            "url": "http://www.europeana.eu/v2/opensearch.rss?count=%7B%7D&searchTerms=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Basic search function following the opensearch specification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5a0bd71-4815-4469-9e80-2e0340235ba2"
            }
          ]
        },
        {
          "id": "87ce6db7-4fd6-4ecf-b151-4488642939bf",
          "name": "searchRecords",
          "request": {
            "url": "http://www.europeana.eu/v2/search.json?callback=%7B%7D&colourpalette=%7B%7D&cursor=%7B%7D&facet=%7B%7D&landingpage=%7B%7D&media=%7B%7D&profile=%7B%7D&qf=%7B%7D&query=%7B%7D&reusability=%7B%7D&rows=%7B%7D&sort=%7B%7D&start=%7B%7D&text_fulltext=%7B%7D&thumbnail=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for records."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09b24cfa-c74a-4bf2-aef4-50292a37e235"
            }
          ]
        },
        {
          "id": "931331fc-0773-4857-895d-b37a7c34ff25",
          "name": "fieldTrip",
          "request": {
            "url": "http://www.europeana.eu/v2/search.rss?language=%7B%7D&limit=%7B%7D&offset=%7B%7D&profile=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Google fieldtrip formatted rss of selected collections."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f97e750-e24a-4b25-af27-609b64611c05"
            }
          ]
        }
      ]
    },
    {
      "name": "Provider",
      "item": [
        {
          "id": "356315d5-7130-473a-a2f3-72aecd5de37b",
          "name": "getProvider",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "provider/:id.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific europeana provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95fa091d-0c01-45a5-8357-6fbce38b1e48"
            }
          ]
        }
      ]
    },
    {
      "name": "Providers",
      "item": [
        {
          "id": "d50315f9-463b-4c36-b93c-2a1e9a9dc183",
          "name": "listProviderDatasets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "provider/:id/datasets.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of datasets provided by a specific provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ccb57b1-91ef-437f-9469-c9afae270b30"
            }
          ]
        },
        {
          "id": "5ca22d37-b94b-4243-8a53-b4eeedbeecea",
          "name": "listProviders",
          "request": {
            "url": "http://www.europeana.eu/v2/providers.json?callback=%7B%7D&countryCode=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of europeana data providers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0d681b8-cc39-4742-aa68-c53001b7959d"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "e160f624-3a39-4068-bc90-c38ba296a106",
          "name": "getSingleRecordJson",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "hierarchytimeout",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "profile",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single record in json format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb0cb3c3-87ce-45fa-bf56-f7ac70d5b96f"
            }
          ]
        },
        {
          "id": "dce552e6-3070-46d5-a8ae-1ca4319d1ff5",
          "name": "getSingleRecordJsonLD",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.jsonld"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single record in json ld format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02d96907-d2e9-46f3-8663-45d71838d979"
            }
          ]
        },
        {
          "id": "aa3cfaa7-9c29-4ed7-8c36-fef15bf4280f",
          "name": "getSingleRecordRDF",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.rdf"
              ],
              "query": [
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single record in rdf format)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fda9bb7-5c5f-4b85-b0ef-4f1c0f039a7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggestions",
      "item": [
        {
          "id": "37750ea8-95c9-4f83-a72c-34a66b9f1bbc",
          "name": "suggestions",
          "request": {
            "url": "http://www.europeana.eu/v2/suggestions.json?callback=%7B%7D&phrases=%7B%7D&query=%7B%7D&rows=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get autocompletion recommendations for search queries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ae71159-269f-495e-afe3-0f783ad0be62"
            }
          ]
        }
      ]
    }
  ]
}