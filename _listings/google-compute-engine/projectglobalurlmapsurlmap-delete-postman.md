{
  "info": {
    "name": "Google Compute Engine API Delete URL Map",
    "_postman_id": "9f139bd7-f451-40a0-8e72-def81a857be9",
    "description": "Deletes the specified UrlMap resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "url map",
      "item": [
        {
          "id": "17ee88b9-66c3-49e5-9f52-f7bec8f35cc7",
          "name": "compute.urlMaps.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified UrlMap resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1c24232-57ac-4a03-bbfa-30095aeda14a"
            }
          ]
        }
      ]
    }
  ]
}