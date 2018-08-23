{
  "info": {
    "name": "Spreaker API Delete Device",
    "_postman_id": "9e214a67-8f8a-4cc6-af4b-46dfce3f6dba",
    "description": "Delete the association from a mobile device and a registered user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "88f9c856-2fd4-40f1-959f-9beaaec1edfc",
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
              "id": "d807c5a4-387a-4d78-b4f5-4a084624984e"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "3076e4eb-9792-4c38-87a2-dc0ee097b353",
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
              "id": "5a2e8dc7-88ed-4dba-9aa0-662acbca9801"
            }
          ]
        }
      ]
    },
    {
      "name": "Episode",
      "item": [
        {
          "id": "639e9b33-9834-4f2f-9e2d-38fc22f099f4",
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
              "id": "f3478be5-cc04-4048-aa19-0f52d396dbc0"
            }
          ]
        },
        {
          "id": "27c0cbd2-f65b-479a-b2a9-339335d88b6a",
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
              "id": "ab54b08f-7adc-44da-8956-b4b039c44a9a"
            }
          ]
        },
        {
          "id": "21f4cb4f-3dc0-47d8-88d4-d2a73f76f1a2",
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
              "id": "27480665-8fd2-4bba-9564-e82389fc1c85"
            }
          ]
        },
        {
          "id": "08831dde-be6c-4b1d-bc8a-125d6618c5cd",
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
              "id": "4a6b3b5c-fe69-4928-b045-a446d938a8c7"
            }
          ]
        },
        {
          "id": "a8f3d93f-5993-4d6e-b617-87c41c16b1b0",
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
              "id": "4e124b91-c4a5-4499-8c05-5408aa04874e"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "b840be69-d81b-4824-b60c-383857e8f4bd",
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
              "id": "50905636-025d-49e3-98d5-099864035963"
            }
          ]
        },
        {
          "id": "d0555e59-2ada-43ce-a6b5-ad46d865dbc7",
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
              "id": "876d6c2c-0669-4187-8bfd-8b9d9733c4e1"
            }
          ]
        },
        {
          "id": "440b41bf-45eb-4f45-8d5c-bf9e4ed2ec96",
          "name": "putUserUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fullname",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gender",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "show_age",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit user info (eg. fullname, description aka biography, gender, birthday, ...)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "040f8f74-fea5-4482-a655-00faccef5114"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "01fa2558-0dbd-477f-a5f5-32cda4d4aa91",
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
              "id": "41a73f5c-9ef8-4589-8e1e-cb9a706ff7eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Explore",
      "item": [
        {
          "id": "e9fd06f6-96e8-4e94-a864-9ca5d71875be",
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
              "id": "980a8fd4-f60e-42f2-ae3f-172b5fdb58c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "cf7ec4c7-2979-4d9e-a90c-0788a2d1a519",
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
              "id": "28b0cb8b-54a4-4e02-9942-19cef1c7f919"
            }
          ]
        },
        {
          "id": "9d9a29b1-d9e6-4535-859b-40ff7d7592cc",
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
              "id": "41248a19-f074-4ccd-abea-7a68ea0ee698"
            }
          ]
        }
      ]
    },
    {
      "name": "Owned",
      "item": [
        {
          "id": "44ad01f7-2757-4213-8814-04d815495f84",
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
              "id": "37bcce23-93ae-4aa1-9327-ee7e475da026"
            }
          ]
        },
        {
          "id": "9194947d-bab7-40b3-b458-bc54748ef156",
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
              "id": "a355b2e1-9259-4141-a99a-8cbda789c3e3"
            }
          ]
        },
        {
          "id": "82e18356-b73a-4b3f-899d-c87f73cbd5a2",
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
              "id": "f2ebd194-1280-45b5-88c5-6cebff298680"
            }
          ]
        },
        {
          "id": "0f840cc9-9828-4e1f-8a2f-c0abc4474e25",
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
              "id": "77233967-86ca-4d2e-b285-dea3e508bdbe"
            }
          ]
        },
        {
          "id": "520f9ab0-e8aa-4594-97ad-0115f14e119d",
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
              "id": "de87238d-9e1e-4584-88c7-2b97701865c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "b6091a9b-1748-427c-a08b-e1239ceb094b",
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
              "id": "67d12ba5-b22e-48cf-b669-17545434cba9"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "53f653e4-4d1a-42b4-85be-394929bed04e",
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
              "id": "7f07765c-c6f5-493f-a116-209dffda26e3"
            }
          ]
        },
        {
          "id": "0b955d0f-65fa-4474-b97a-9325bc5f1410",
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
              "id": "a64b2659-9062-4035-b25b-e0e3e756a9b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "6b491087-d637-494a-857e-5b05f3d75f5a",
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
              "id": "26879fda-e311-45f4-a4db-398547076f24"
            }
          ]
        },
        {
          "id": "1cb78c74-8d3d-41ab-a92c-02623c7894db",
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
              "id": "8c8edc6b-cd8a-4a41-b188-440b6506900e"
            }
          ]
        },
        {
          "id": "4c29e86e-d2d3-4133-8862-8cd63bfeb67e",
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
              "id": "f8d06e15-6c6c-445b-bbbf-87ea4c707b91"
            }
          ]
        },
        {
          "id": "93bd526a-aa0f-4631-b4b2-9d04adc2fed5",
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
              "id": "f7ec426c-b8f5-4259-b81b-0c7c3ce3836e"
            }
          ]
        }
      ]
    },
    {
      "name": "Dele",
      "item": [
        {
          "id": "b6f31ab0-29e9-4a69-885d-b9ff65bccbfb",
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
              "id": "20d922bc-abdf-4239-872f-c219985295cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Podcast",
      "item": [
        {
          "id": "5bab207d-38ca-4183-a5d8-d846d740eb2e",
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
              "id": "4ee92946-a2ab-4b29-93f7-9a3c8ed7b432"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "f077cfc8-b311-43b3-911e-7c681c3bd4dd",
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
              "id": "9a37dc7b-7e12-43e5-9adf-ceb71ebd0c7a"
            }
          ]
        },
        {
          "id": "80e88dc0-22f5-445e-815d-7bb12263516d",
          "name": "getUserFollowerUsersFan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:follower_id/users/fan"
              ],
              "variable": [
                {
                  "id": "follower_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get List of Following"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe25f458-6ef5-4b50-a6a5-5e3e9b7a2177"
            }
          ]
        }
      ]
    },
    {
      "name": "Follow",
      "item": [
        {
          "id": "8da38d86-91d9-49cc-be13-940c1b2abf88",
          "name": "postUserFollowedFans",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Follow User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca774cb3-a29e-4296-8e8f-02c786286026"
            }
          ]
        }
      ]
    },
    {
      "name": "Unfollow",
      "item": [
        {
          "id": "6c31bcca-36f0-43d5-bf59-84fa953fe379",
          "name": "deleteUserFollowedFansFollower",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:followed_id/fans/:follower_id"
              ],
              "variable": [
                {
                  "id": "followed_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "follower_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unfollow User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30362be3-7742-4726-bae9-f532487ccfe3"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "855bfefa-d7be-4802-9155-9f01ec442c2b",
          "name": "getUserUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id"
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
            "description": "Retrieves an user by unique identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faca1858-2bce-4042-af73-20280fd26a25"
            }
          ]
        },
        {
          "id": "7c6fe0cf-c3d4-47b2-a742-221a6c056af5",
          "name": "getUserUserActions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/actions"
              ],
              "query": [
                {
                  "key": "EPISODE_BROADCAST",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "FACEBOOK",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_MESSAGE",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_MESSAGE",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "TWITTER",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "USER_FOLLOW",
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
            "description": "Retrieves the user actions settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "298b9228-50d7-41e4-87a8-d989ebc15b20"
            }
          ]
        }
      ]
    },
    {
      "name": "Facebook",
      "item": [
        {
          "id": "6fc3db34-44ef-4751-9879-2cd3a3a6602b",
          "name": "getUserUserActionsFacebook",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/actions/facebook"
              ],
              "query": [
                {
                  "key": "EPISODE_BROADCAST",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_MESSAGE",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_MESSAGE",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "USER_FOLLOW",
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
            "description": "Edit facebook share settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f7491f0-722a-46bc-937b-693f88c60f3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Twitter",
      "item": [
        {
          "id": "6fe00a4a-b763-492d-b595-1e5aebf25c18",
          "name": "putUserUserActionsTwitter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/actions/twitter"
              ],
              "query": [
                {
                  "key": "EPISODE_BROADCAST",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "RADIO_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "SHOW_FOLLOW",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "USER_FOLLOW",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit twitter share settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0d056d5-2b49-40d6-9b54-72f66d359082"
            }
          ]
        }
      ]
    },
    {
      "name": "Device",
      "item": [
        {
          "id": "17d0b1d9-fb7a-4111-9ff6-366680632417",
          "name": "deleteUserUserDeviceToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/device/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the association from a mobile device and a registered user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cf9a78a-5f62-49b0-a656-9a39d34b70b9"
            }
          ]
        }
      ]
    }
  ]
}