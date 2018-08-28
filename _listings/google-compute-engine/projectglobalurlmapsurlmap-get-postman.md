{
  "info": {
    "name": "Google Compute Engine API Get URL Map",
    "_postman_id": "e30303f7-1a95-43a6-a5f6-e16840705912",
    "description": "Returns the specified UrlMap resource. Get a list of available URL maps by making a list() request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "url map",
      "item": [
        {
          "id": "fefbf661-18f2-44eb-8172-4f0d7c2cabe3",
          "name": "compute.urlMaps.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "compute",
                "v1",
                "projects",
                ":project/global/urlMaps/:urlMap"
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "urlMap",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the specified UrlMap resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff6e1cc8-067e-43db-b219-503e0adcf857"
            }
          ]
        }
      ]
    }
  ]
}