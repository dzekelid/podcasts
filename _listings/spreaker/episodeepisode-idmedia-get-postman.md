{
  "info": {
    "name": "Spreaker API Get Episode Media List",
    "_postman_id": "bad283a7-6fc9-43ed-b541-75744b5a8e72",
    "description": "Get Episode Media List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Episode",
      "item": [
        {
          "id": "bd55b59b-5a4e-43a8-bf80-752bfb654b9b",
          "name": "getEpisodeEpisodeMedia",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id/media"
              ],
              "variable": [
                {
                  "id": "episode_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Episode Media List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cdf4b38-9745-4c91-bbf6-7a6b9174c5fa"
            }
          ]
        }
      ]
    }
  ]
}