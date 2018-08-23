{
  "info": {
    "name": "Spreaker API Get Top Live Episodes",
    "_postman_id": "3a757bb4-dc7a-446f-bf0a-15cfd8917afa",
    "description": "Retrieves live episodes sorted by rank",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Live",
      "item": [
        {
          "id": "f6656cd7-175c-48e3-8dfa-36d58a705245",
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
              "id": "f4a6b555-95b8-488e-a3ae-b0306447e58e"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "b7c4e75d-39bd-4c6c-aff8-f9e1cb7c7fa1",
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
              "id": "4ec9bd37-6fab-419c-bb8c-59f9a4d8b3ef"
            }
          ]
        }
      ]
    }
  ]
}