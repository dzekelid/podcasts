{
  "info": {
    "name": "Spreaker API Get Episode Streams",
    "_postman_id": "272e20e2-e153-4fb0-9ff2-90180681bd9b",
    "description": "The response contains a collection of RTMP / RTMPT streams.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Episode",
      "item": [
        {
          "id": "71778526-1170-4c45-9d9c-32362ab93bcb",
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
              "id": "10fc2263-190d-47a5-8311-bbe484dfa0b4"
            }
          ]
        },
        {
          "id": "5e81ce96-f9dc-4bce-b9c0-7926bf4ff69c",
          "name": "getEpisodeEpisodeStreamsRtmp",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id/streams/rtmp"
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
            "description": "The response contains a collection of RTMP / RTMPT streams."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe3b7b39-d222-4b18-a2b1-d5c7315f029d"
            }
          ]
        }
      ]
    }
  ]
}