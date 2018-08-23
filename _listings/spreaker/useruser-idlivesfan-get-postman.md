{
  "info": {
    "name": "Spreaker API Get Favorite Live Episodes",
    "_postman_id": "7198dd8c-e4ba-4ee8-acc2-482d1f3d0f2d",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Live",
      "item": [
        {
          "id": "d0625be3-08fb-412d-b73e-6a7c538aa4a4",
          "name": "getEpisodesLive",
          "request": {
            "url": "http://api.spreaker.com/episodes/live?show_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all live episodes at the moment of the request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b08fda19-7ba8-4cdf-94f8-f34dec4f7c6a"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "0b585754-7b0a-4f8f-937a-6d956392cb3b",
          "name": "getLivesTop",
          "request": {
            "url": "http://api.spreaker.com/lives/top?I=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves live episodes sorted by rank"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d27cc1b3-e25a-40bc-aaae-4a7237d1a5c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorite",
      "item": [
        {
          "id": "cd234439-a3cc-446a-bddb-1a939d5143d8",
          "name": "getUserUserLivesFan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/lives/fan"
              ],
              "query": [
                {
                  "key": "/user/{user_id}/lives/fan",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Favorite Live Episodes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "049aa919-a5f2-4a36-baa3-dec935a512cd"
            }
          ]
        }
      ]
    }
  ]
}