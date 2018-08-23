{
  "info": {
    "name": "Spreaker API Get Categories",
    "_postman_id": "bb9cda5c-ac41-427c-a982-af60719cbce3",
    "description": "Retrieves all categories in Spreaker",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "73012d38-ba89-42b8-bd6d-5408baa7038f",
          "name": "getCategoriesFlat",
          "request": {
            "url": "http://api.spreaker.com/categories/flat",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all categories in Spreaker"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1c7e5b9-6f5c-486f-9257-1aa83e55b921"
            }
          ]
        }
      ]
    }
  ]
}