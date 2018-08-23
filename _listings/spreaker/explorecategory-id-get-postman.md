{
  "info": {
    "name": "Spreaker API Explore Category Items",
    "_postman_id": "bbf8ac62-4c0d-4986-8e2c-d90b791d99a8",
    "description": "This API returns information and items of a specific category. The response contains two properties at root level:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Explore",
      "item": [
        {
          "id": "654e939a-a45f-4025-a595-1fade1887c4a",
          "name": "getExploreCategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "explore/:category_id"
              ],
              "query": [
                {
                  "key": "explore_category",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "items",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category_id",
                  "value": "category_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API returns information and items of a specific category. The response contains two properties at root level:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f898cf30-c8ab-4366-918a-71a43e9fa2c0"
            }
          ]
        }
      ]
    }
  ]
}