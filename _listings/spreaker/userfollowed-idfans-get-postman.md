{
  "info": {
    "name": "Spreaker API Get List of Followers",
    "_postman_id": "a3c86c85-b95a-47ce-a3ef-8d92cfa593dc",
    "description": "Get List of Followers",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "77548e31-de6a-4f85-8b8b-8b29311b0539",
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
              "id": "7a4fcc5d-078d-4197-b42f-791e85d37a7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "07a730ce-fa01-493f-80ff-bbd007deaaf0",
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
              "id": "1450d598-9cf4-453c-b002-b88a3c45f3ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Episode",
      "item": [
        {
          "id": "4bc04b93-7aec-443b-bdf2-b3fdcb9ece13",
          "name": "getEpisodeEpisode",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an episode by unique identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "090bf0b4-d278-4308-a77b-46ff6b2178fa"
            }
          ]
        },
        {
          "id": "b2024d40-548c-4b3d-b1a8-f22e6cf535b3",
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
              "id": "10dd85da-4d3a-4c83-b409-80c5ffe41371"
            }
          ]
        },
        {
          "id": "2b60a728-5abf-4ddb-9c3f-76af05987852",
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
              "id": "438ac23e-7956-422c-a40f-f7231d0baeab"
            }
          ]
        },
        {
          "id": "cc9127ac-2997-4e71-91e2-aa0ddf032fb2",
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
              "id": "b3691ff2-6b57-4b53-97cf-877037782428"
            }
          ]
        },
        {
          "id": "20c918e5-21a6-47d5-8b19-72676987229e",
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
              "id": "b021585a-ad4a-4ca0-9529-25ab7c9cc565"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "dceada7f-73f4-40f8-bd0f-a3ebc4b639af",
          "name": "putEpisodeEpisode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "episode/:episode_id"
              ],
              "query": [
                {
                  "key": "category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
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
            "description": "Edit episode info (eg. title, description, category, tags, ...)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6356f48b-1b1b-4ec6-9403-f1f6bbe500d7"
            }
          ]
        },
        {
          "id": "f578f713-6e40-4bdf-8568-66a876cb34ca",
          "name": "putShowShow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/:show_id"
              ],
              "variable": [
                {
                  "id": "show_id",
                  "value": "show_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit show info (name, description and contacts)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3718ec3a-32f3-4503-b19e-8c0d2d9f5f2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "59edd428-a6a5-4e6d-b5a3-4eef59ba9778",
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
              "id": "873919a5-8912-4b17-b9e4-765c61c8dd4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Explore",
      "item": [
        {
          "id": "479af907-b6af-4809-836c-3f8225eb4a62",
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
              "id": "08e3b1c0-fb0f-4a21-ad13-8408da66d229"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "91718a10-c7ee-4840-9c3c-d54ef4cac9bd",
          "name": "postLibraryUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id"
              ],
              "query": [
                {
                  "key": "Filedata",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "length",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "style_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new Media in the specified user library"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5062b701-f737-4cd2-8007-2222a04d92a0"
            }
          ]
        },
        {
          "id": "5874b124-94c7-4f4a-90d7-1ed9bf202d99",
          "name": "getMediaMedia",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "media/:media_id"
              ],
              "variable": [
                {
                  "id": "media_id",
                  "value": "media_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Media by unique identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3893347-176c-4bd3-abd4-7021139312db"
            }
          ]
        }
      ]
    },
    {
      "name": "Owned",
      "item": [
        {
          "id": "e26c8b1c-4ce7-4df2-b0e2-c38bfa5ebc46",
          "name": "getLibraryUserEffectsOwned",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id/effects/owned"
              ],
              "query": [
                {
                  "key": "sort_col",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_dir",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paginated list of media owned by <user_id> filtered by type:."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81384ed0-cb16-429e-ad9b-e224a2a94c9e"
            }
          ]
        },
        {
          "id": "27ff685d-ceac-4475-a99c-b119361f12d0",
          "name": "getLibraryUserJinglesOwned",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id/jingles/owned"
              ],
              "query": [
                {
                  "key": "sort_col",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_dir",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paginated list of media owned by <user_id> filtered by type:."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09a7178d-e289-4a9e-ba81-a297e00e2d2c"
            }
          ]
        },
        {
          "id": "4aecc76a-6d17-4642-ba9b-f4c2e1067183",
          "name": "getLibraryUserLoopsOwned",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id/loops/owned"
              ],
              "query": [
                {
                  "key": "sort_col",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_dir",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paginated list of media owned by <user_id> filtered by type:."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4900b56-f60a-4aae-a5e7-73f044ff1fed"
            }
          ]
        },
        {
          "id": "da1e7c98-9eec-485d-8ad8-9f41663fbcef",
          "name": "getLibraryUserSongsOwned",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id/songs/owned"
              ],
              "query": [
                {
                  "key": "sort_col",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_dir",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paginated list of media owned by <user_id> filtered by type:."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e777ab51-ad41-4978-aea2-2c83ee3df8ae"
            }
          ]
        },
        {
          "id": "2853ffef-83da-4c5f-9b7d-03bd43547b19",
          "name": "getLibraryUserSoundtracksOwned",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "library/:user_id/soundtracks/owned"
              ],
              "query": [
                {
                  "key": "sort_col",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_dir",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paginated list of media owned by <user_id> filtered by type:."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd1ad88-22b9-4e88-91f8-869332e03c5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "307220af-16a8-4e77-9846-f23e07b27730",
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
              "id": "c8c5ae62-2374-4ef9-9b70-1c686ffb8f6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "750e91a7-30db-4d3b-a53f-f32a86f34eb7",
          "name": "getSearchQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "search/:query"
              ],
              "variable": [
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search users, shows and episodes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2cce20d-e2aa-4013-832d-e59228261539"
            }
          ]
        },
        {
          "id": "e95a7fc6-6381-4c57-ada5-2e8388ec8562",
          "name": "getShowSearchQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/search/:query"
              ],
              "variable": [
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows to find shows."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3f25fe0-0d66-4160-8339-d67406fa6c78"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "bad1db45-1b4c-44ec-9238-a0f827132d9d",
          "name": "getShowShow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/:show_id"
              ],
              "variable": [
                {
                  "id": "show_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves show information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "145462df-9abd-4ee0-a12e-787ea6ba3f6c"
            }
          ]
        },
        {
          "id": "2bec6e07-fb7a-468b-962b-d9a88db39851",
          "name": "getShowShowEpisodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/:show_id/episodes"
              ],
              "variable": [
                {
                  "id": "show_id",
                  "value": "show_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all listenable episodes by show (both live and podcast, ordered by published_at DESC)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7194bb0e-bb5c-4b34-bb0c-71e92f124dfe"
            }
          ]
        },
        {
          "id": "a8f06a1b-c345-4c70-ad88-9b00aa331d60",
          "name": "getShowShowEpisodesAll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/:show_id/episodes/all"
              ],
              "variable": [
                {
                  "id": "show_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all episodes by show (both live and podcast, ordered by published_at DESC)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e630319-1ccf-4826-9888-31b789cf7662"
            }
          ]
        },
        {
          "id": "4153e985-bfbd-431b-83dc-b8e91da8e349",
          "name": "postShows",
          "request": {
            "url": "http://api.spreaker.com/shows?title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Show."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccbbd9f1-cbdb-4786-943c-89c4d7469434"
            }
          ]
        }
      ]
    },
    {
      "name": "Dele",
      "item": [
        {
          "id": "644cab12-145b-418e-a66b-38f937031eff",
          "name": "deleteShowShow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/:show_id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "facebook_url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skype_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sms_number",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tel_number",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "twitter_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "website_url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "show_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a show. Theres no way to recover a deleted show. Only show without episodes in it can be deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fc2d4b9-2bf0-445a-b5b0-4e630e958695"
            }
          ]
        }
      ]
    },
    {
      "name": "Podcast",
      "item": [
        {
          "id": "8c777a16-5164-4b63-8773-d1bc65b3426d",
          "name": "postShowShowEpisodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "show/:show_id/episodes"
              ],
              "query": [
                {
                  "key": "category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "download_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "explicit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "hidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "media_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "shares",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "show_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates new podcast episode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "697edb15-449a-41e6-8874-61a0338a8de8"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "23ff0c90-5320-4c1f-944c-2832c5df9944",
          "name": "getUserFollowedFans",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:followed_id/fans"
              ],
              "variable": [
                {
                  "id": "followed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get List of Followers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b38499ed-1955-448d-b717-9863834a79ec"
            }
          ]
        }
      ]
    }
  ]
}