{
  "info": {
    "name": "Europeana get the list of datasets provided by a specific provider",
    "_postman_id": "b88c413f-de2f-49ac-87ba-ca381f4e0ece",
    "description": "Get the list of datasets provided by a specific provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dataset",
      "item": [
        {
          "id": "378114e5-37a3-4245-92a0-8e7a422b441a",
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
              "id": "84bbf2b5-092b-4e46-bb3e-0ad7509b1037"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "498601be-5448-40e4-b1b1-cb5e2f3dc361",
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
              "id": "ecc666ff-a8e0-4107-a703-3877a48b2e40"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "03d40465-1484-4315-b596-c704731f5123",
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
              "id": "641b5fc6-6a95-41cd-86a0-b18cec07e42e"
            }
          ]
        }
      ]
    },
    {
      "name": "Provider",
      "item": [
        {
          "id": "782007fe-d22a-4cb0-afa2-a20fa5a81650",
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
              "id": "d64afc24-08aa-4159-8635-97857c962538"
            }
          ]
        }
      ]
    },
    {
      "name": "Providers",
      "item": [
        {
          "id": "16754c21-9ee6-4173-8741-ddb0007e2cf3",
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
              "id": "0d4ee5e3-1a84-4c64-84a6-e04ab38417bf"
            }
          ]
        }
      ]
    }
  ]
}