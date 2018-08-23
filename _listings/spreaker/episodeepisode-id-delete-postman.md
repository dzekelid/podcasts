{
  "info": {
    "name": "Spreaker API Delete Episode",
    "_postman_id": "6b337d61-fa3e-4841-8421-f8d4c9afd0e9",
    "description": "Deletes an episode. Theres no way to recover a deleted episode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "3ecdaff0-6396-4edd-8ba0-b479ed955605",
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
              "id": "700e1028-6865-4c9e-b8db-e245f99492a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "7665d246-c305-44e4-b2b0-87ddca4bcc50",
          "name": "putEpisode<episode>Image",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id/image"
              ],
              "query": [
                {
                  "key": "image_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "episode_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Change Episode Image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e60af667-dc70-4173-83b5-a52e28055be6"
            }
          ]
        }
      ]
    },
    {
      "name": "Episode",
      "item": [
        {
          "id": "29788987-29fb-4a01-b87a-864c6a860075",
          "name": "deleteEpisodeEpisode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id"
              ],
              "variable": [
                {
                  "id": "episode_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an episode. Theres no way to recover a deleted episode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "702af63b-f6ef-4a93-821e-ca47561013a8"
            }
          ]
        }
      ]
    }
  ]
}