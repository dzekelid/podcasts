{
  "info": {
    "name": "Spreaker API Get Live Episodes",
    "_postman_id": "e5b589cf-d0a7-487d-9287-fef3a3b8729e",
    "description": "Retrieves all live episodes at the moment of the request",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Live",
      "item": [
        {
          "id": "58c0d57d-028e-4864-9aaf-1be9178bbe63",
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
              "id": "573ef1fa-64e4-409d-b1d6-a2787505aa2a"
            }
          ]
        }
      ]
    }
  ]
}