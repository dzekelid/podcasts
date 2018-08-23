{
  "info": {
    "name": "Spreaker API Get Show Episodes",
    "_postman_id": "5324a612-e981-4c8f-b9f4-1f7f9b3d622a",
    "description": "Retrieves all listenable episodes by show (both live and podcast, ordered by published_at DESC).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "969a0618-68d9-40fa-8aff-6ec0ba77fa29",
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
              "id": "3bfc0921-c5cc-409f-b283-c314cece584c"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "72785e43-3fb4-471b-975b-ef10de2e6729",
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
              "id": "7ca7b928-d22c-40f1-8412-b3f1868f1b9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Episode",
      "item": [
        {
          "id": "bd8df940-84b5-46c1-93f1-3d47f8484ea6",
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
              "id": "fe0260e4-32ac-40aa-be3d-9ca5a5556b8c"
            }
          ]
        },
        {
          "id": "702c435f-c9eb-479e-9504-b28af8bf93ca",
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
              "id": "21f0dd3f-8f3d-4672-a3ab-a3ee24f00eff"
            }
          ]
        },
        {
          "id": "8efbc02d-9106-4330-a4de-fdb471ac88e4",
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
              "id": "51eb0201-e488-4a39-b1cf-573a07dd4a33"
            }
          ]
        },
        {
          "id": "8a97f11e-2c52-4b95-aa6e-d6c5e2caa0a7",
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
              "id": "ab899224-66c6-4297-97be-951e44ced070"
            }
          ]
        },
        {
          "id": "d9b133dc-52fe-4114-bbf2-2ac922d6486e",
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
              "id": "404643a6-c242-4908-bc38-005c90077c9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "5d55b917-ecfe-4f8d-9b8e-064f9ae890a4",
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
              "id": "2b845580-fde6-44f6-8962-b4dbb7ef6f73"
            }
          ]
        },
        {
          "id": "1dda3058-40d5-4766-802f-cb724c7a32b8",
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
              "id": "e6d0a7ae-5462-4fda-aefb-7d12d5fbed66"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "c8428266-85f1-41c9-b5d6-91e00b0348f0",
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
              "id": "cd9003f6-3750-4d40-82f7-453a5a989668"
            }
          ]
        }
      ]
    },
    {
      "name": "Explore",
      "item": [
        {
          "id": "c02af8a8-e269-4ac1-bb6c-ac616e0fbca8",
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
              "id": "1bc57033-8625-4085-b464-581469f6a073"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "7b979aa2-2dc2-4ba7-b39c-afbd421721d0",
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
              "id": "28ff826e-f965-4a5a-8117-66215e450ad8"
            }
          ]
        },
        {
          "id": "a622a1dc-b4d0-46f9-bb22-90dd0b7352a4",
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
              "id": "a08424f7-8ea5-4611-a880-dccb921933be"
            }
          ]
        }
      ]
    },
    {
      "name": "Owned",
      "item": [
        {
          "id": "d463d08a-f928-43ca-81e4-80007e6dcedf",
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
              "id": "336a66c9-deca-4172-8a97-2703b126c523"
            }
          ]
        },
        {
          "id": "d5e4f281-7342-4caf-9070-5e75a8633158",
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
              "id": "5195670f-9618-403e-ae10-22b2ebfa3dee"
            }
          ]
        },
        {
          "id": "713705b0-11b3-40c2-aada-0797836e8b75",
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
              "id": "d61f05a0-e7b7-45a0-90ff-a9525f349c0c"
            }
          ]
        },
        {
          "id": "2a3e5b69-daeb-4fd7-a91b-a189c3627ff3",
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
              "id": "468477be-441a-4068-9d73-baed8c5dc6f1"
            }
          ]
        },
        {
          "id": "a04777ff-e0f7-43ee-bfb1-ee405aa3b66e",
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
              "id": "f5227b57-a40f-4842-a4c4-5f2bdb1aaef3"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "74848f57-9ff7-4864-8d25-521587bf9ea6",
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
              "id": "3d02aa9f-1049-4b66-b8a8-6e683df8c864"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "725a450d-eeba-4ba7-99ae-bbb0e11f5f13",
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
              "id": "c51f3a80-4bb8-474e-8eb3-7eae5044e771"
            }
          ]
        },
        {
          "id": "ada487f4-0bb9-42ed-893c-c525ae0ca927",
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
              "id": "51778418-9203-4555-b483-a8bb6e7e9a9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "662efb97-5558-4251-8d01-d3686cf6b406",
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
              "id": "b62c90c9-6da1-4322-b159-69cc949c9d46"
            }
          ]
        },
        {
          "id": "9be6af7b-dc82-4418-8207-dd0008dfab99",
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
              "id": "71eb6e05-e8be-4704-9c11-4e042dd1a62b"
            }
          ]
        }
      ]
    },
    {
      "name": "Dele",
      "item": [
        {
          "id": "5d41260b-1b4c-4695-b45d-fa670e76c29a",
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
              "id": "67adef63-3891-43c4-9ec0-1bee3394deac"
            }
          ]
        }
      ]
    }
  ]
}