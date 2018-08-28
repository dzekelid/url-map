{
  "info": {
    "name": "Google Compute Engine API Get URL Maps",
    "_postman_id": "408a45b0-c34f-451a-9489-d0b9d157bcbf",
    "description": "Retrieves the list of UrlMap resources available to the specified project.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "url map",
      "item": [
        {
          "id": "6ed54676-341f-46b8-9a73-9954757b40ae",
          "name": "compute.urlMaps.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "compute",
                "v1",
                "projects",
                ":project/global/urlMaps"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the list of UrlMap resources available to the specified project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25779cf2-9039-4ddb-ad3e-e7a209a0fbda"
            }
          ]
        }
      ]
    }
  ]
}