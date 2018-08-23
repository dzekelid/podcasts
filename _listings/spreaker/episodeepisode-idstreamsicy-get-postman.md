{
  "info": {
    "name": "Spreaker API Get Episode Streams",
    "_postman_id": "dc7ed042-b157-45b8-855d-1edd329bc3b0",
    "description": "The response contains a collection of ICY streams.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Episode",
      "item": [
        {
          "id": "3591343d-0ae0-4f2d-8b0f-ce5927779e87",
          "name": "getEpisodeEpisodeStreamsIcy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id/streams/icy"
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
            "description": "The response contains a collection of ICY streams."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aa6ea06-bf7a-450d-acc5-e4076553b686"
            }
          ]
        }
      ]
    }
  ]
}