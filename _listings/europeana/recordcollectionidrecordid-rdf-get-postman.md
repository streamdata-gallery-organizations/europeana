{
  "info": {
    "name": "Europeana get single record in RDF format)",
    "_postman_id": "b8d44af1-9ae6-46f2-8533-ba37befa005d",
    "description": "Get single record in rdf format).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collections",
      "item": [
        {
          "id": "41544c0b-9ce7-40d9-aa72-580e41300ac2",
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
              "id": "09676f4b-3e86-41c8-915b-65ad76e50a6e"
            }
          ]
        },
        {
          "id": "e8829650-88d2-4cfe-9987-9703a9571c44",
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
              "id": "4c8f1e40-5772-4be9-b676-2650172d9ccb"
            }
          ]
        },
        {
          "id": "05646a21-a7ca-4341-bee0-e118279fba3a",
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
              "id": "dfcb4b55-53e8-43f9-996f-cd058ae4d9c6"
            }
          ]
        }
      ]
    }
  ]
}