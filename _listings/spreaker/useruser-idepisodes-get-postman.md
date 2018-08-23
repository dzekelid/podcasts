{
  "info": {
    "name": "Spreaker API Get User Episodes",
    "_postman_id": "37423bdf-4498-498a-9ef4-60635db796e3",
    "description": "Retrieves all listenable episodes by user (both live and podcast, ordered by published_at DESC).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "0934c75a-e28d-4dff-8612-e7191837b584",
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
              "id": "11913369-47cc-4360-9196-ce6b1bd0deba"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "9d3ef782-594f-4955-a080-2f4100f83bb6",
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
              "id": "71ea33b5-778d-4324-a0be-71cf4959e5a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Episode",
      "item": [
        {
          "id": "97fe10d2-efd6-444e-b0f9-08a8a523ded5",
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
              "id": "26e6fa3b-3ed5-4a1f-b063-dad23186d471"
            }
          ]
        },
        {
          "id": "ea67d489-cf33-40c5-9462-30c07c2e3b50",
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
              "id": "d017a8f9-8be7-4f2d-931e-d67d77cd0d95"
            }
          ]
        },
        {
          "id": "4ea2c401-e962-4c3b-865c-50fb539da39a",
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
              "id": "d6487e13-6207-4a11-8007-4956a45701df"
            }
          ]
        },
        {
          "id": "17d00cb0-fb84-4d20-9343-63848b1c8866",
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
              "id": "34641bc2-870b-42db-8d1f-553079c0bf46"
            }
          ]
        },
        {
          "id": "6dfd3d4e-7a57-40b0-80d3-9b3f32ae2658",
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
              "id": "00359e74-b707-4264-8aa9-7989da1532d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "3acfcc9d-2413-4cd7-ad2d-80d31281e122",
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
              "id": "29ae24ab-ee42-4f22-80ad-c40b276d2bf2"
            }
          ]
        },
        {
          "id": "60c734f5-4d2d-4a4c-a327-5c8722a40a21",
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
              "id": "21c877ab-eea6-4072-97b1-d9b46f431f75"
            }
          ]
        },
        {
          "id": "99bfeee7-c82a-416f-a7da-fcc638f58c60",
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
              "id": "a905595b-34ab-45c9-b45f-ea24a312c4c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "409adbb4-31cf-4e33-840c-9853aee433d1",
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
              "id": "f8694fad-f275-4d37-90a6-fc9dad2a9d14"
            }
          ]
        }
      ]
    },
    {
      "name": "Explore",
      "item": [
        {
          "id": "82b835c5-b8a3-43f3-8b7e-03806c81282f",
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
              "id": "6d88a91f-77cd-413d-9fbc-4ed3ae1825a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "b33e4152-fc23-431d-952c-835dc0dec72f",
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
              "id": "bc9f22f2-bb57-410b-b9bd-22a7b418159e"
            }
          ]
        },
        {
          "id": "34657fa3-f47a-4465-8d93-3ab022c53a45",
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
              "id": "dda6e4a7-0914-4b01-95bf-8251964428ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Owned",
      "item": [
        {
          "id": "b11e4d27-86d4-4ada-8f91-884453f01e5d",
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
              "id": "23287a3a-043b-4948-86b7-d8db979747a4"
            }
          ]
        },
        {
          "id": "e98846b7-8a4d-40fd-ad23-e2bf288a2344",
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
              "id": "28f7843b-6ddf-42c1-b75e-193d4ca204d4"
            }
          ]
        },
        {
          "id": "7046fb22-a6a4-4dde-a626-1878379ca06b",
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
              "id": "c9964dba-d364-4f89-b2e3-626e3b62e89c"
            }
          ]
        },
        {
          "id": "8aee5556-986b-42c2-88fe-edadb86db671",
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
              "id": "e91b7aa0-0332-496d-9e08-161a7578ff22"
            }
          ]
        },
        {
          "id": "ab55506c-9d99-4d5f-9590-b4193c53cb1b",
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
              "id": "ef9a84a2-c80a-4f46-81b9-4df51c5c7571"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "955d2e48-8cea-4aae-9bd7-3b4d7e26c8ed",
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
              "id": "16481f8f-4139-46f3-8672-400921f33f93"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "b17ac41c-00e1-4f59-b6f4-287ad27d9407",
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
              "id": "d1227d57-d214-4e8d-8a92-dd914570b82d"
            }
          ]
        },
        {
          "id": "61496548-dad0-4ae8-8cae-aa6c8ea2fd2f",
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
              "id": "ad603890-eebe-4812-898f-d8daa79f0ef7"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "2ae938c8-cf57-4261-a073-681f3f085fe3",
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
              "id": "009d84b7-e6cc-4a9b-a3af-b1baaaded4b0"
            }
          ]
        },
        {
          "id": "33dee265-d0a5-486d-9be6-eea5b6543a78",
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
              "id": "7e673a47-f5d6-4511-baa7-37bda5f4570c"
            }
          ]
        },
        {
          "id": "4754cfed-2a75-4875-a0d0-89572645d5f1",
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
              "id": "dfe7f69a-b851-43cc-8dde-0f5cdda44ac7"
            }
          ]
        },
        {
          "id": "5be27609-c2b4-47e3-bf08-bbfb57a27a38",
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
              "id": "3cea48b3-8e06-41e9-9aad-452cf159117c"
            }
          ]
        }
      ]
    },
    {
      "name": "Dele",
      "item": [
        {
          "id": "1f29b1a2-2d0e-434d-8869-1d20f8de1605",
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
              "id": "4f6c347d-5029-4f35-98f2-25b6b2994b6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Podcast",
      "item": [
        {
          "id": "6cd5e2a1-ae65-42de-be6e-169d87dbda7f",
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
              "id": "4dab67ba-06fb-4fb7-9c01-87f00fc99868"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "348798eb-a0a8-460a-93b5-e14a011fec3c",
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
              "id": "bca70ff2-edcb-45a7-8e34-91ebcb7c9463"
            }
          ]
        },
        {
          "id": "1d139be1-c666-4bbd-bd7c-63f0efa56a82",
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
              "id": "4e8d70a6-4480-4547-88b1-629adacaee21"
            }
          ]
        }
      ]
    },
    {
      "name": "Follow",
      "item": [
        {
          "id": "ac5276fc-f5b8-40f3-83aa-102b324a6fa0",
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
              "id": "c02d586c-6e56-42da-8be2-b89de1cfb08c"
            }
          ]
        }
      ]
    },
    {
      "name": "Unfollow",
      "item": [
        {
          "id": "8e16d41b-8279-4a68-b21c-1cc185da1bad",
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
              "id": "b69a6360-4a18-41a0-ae7f-f0b5cc368571"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "d4139251-2289-4544-b82b-c75764e5de35",
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
              "id": "c4101872-a37e-4159-8986-397c60485af0"
            }
          ]
        },
        {
          "id": "5f13fa51-39c9-4382-b8aa-eb7dad4844d5",
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
              "id": "7e34bff3-b757-4733-8aac-75752c8cd0ff"
            }
          ]
        },
        {
          "id": "39564150-9710-4473-aa75-fd5888966419",
          "name": "getUserUserEpisodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/episodes"
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
            "description": "Retrieves all listenable episodes by user (both live and podcast, ordered by published_at DESC)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "549bfda0-5ba7-4402-81d0-9c2d3aa0a74e"
            }
          ]
        }
      ]
    },
    {
      "name": "Facebook",
      "item": [
        {
          "id": "ab454fa0-33be-4c99-99fb-3df33d4aa19f",
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
              "id": "72f3ccb3-1645-4ede-a714-4838b630877f"
            }
          ]
        }
      ]
    },
    {
      "name": "Twitter",
      "item": [
        {
          "id": "719dc48b-d86d-45aa-902a-f82ca66d36b5",
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
              "id": "0a86a58f-2c22-424a-8332-6fd67b7c2708"
            }
          ]
        }
      ]
    },
    {
      "name": "Device",
      "item": [
        {
          "id": "20edb99c-c456-49d2-b03d-f7178cb2928e",
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
              "id": "f0f94c65-ed81-448d-a3b2-986b12bcb188"
            }
          ]
        },
        {
          "id": "038b50c7-185c-4dd3-a402-33d491a243e8",
          "name": "getUserUserDevices",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spreaker.com",
              "path": [
                "user/:user_id/devices"
              ],
              "query": [
                {
                  "key": "application_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Delete Device",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "device_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "device_token",
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
            "description": "Creates a new device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15e36417-a1cd-4f79-b3e6-d65d012d81b8"
            }
          ]
        }
      ]
    }
  ]
}