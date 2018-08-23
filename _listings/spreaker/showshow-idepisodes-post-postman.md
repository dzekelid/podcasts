{
  "info": {
    "name": "Spreaker API Create podcast",
    "_postman_id": "71d8660c-ea3d-4ece-b403-6e21470a9d99",
    "description": "Creates new podcast episode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "89453c3b-f3de-4bd1-830a-78519d7a7f4d",
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
              "id": "afa31ded-e79a-4822-b593-e0e9c59bdbd2"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "a8d534b8-6f67-43ef-975c-a58678516264",
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
              "id": "eb00aade-3908-4caa-9868-f36235ccb279"
            }
          ]
        }
      ]
    },
    {
      "name": "Episode",
      "item": [
        {
          "id": "8a250315-b317-4cdf-b657-5826532b370f",
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
              "id": "e1adcbca-f21b-47ff-8679-b3bb26ef2842"
            }
          ]
        },
        {
          "id": "06a44b7f-85e6-49e3-92fb-ccac5f281f3b",
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
              "id": "c757f03f-5f3a-4f75-86ac-3320d78b61fd"
            }
          ]
        },
        {
          "id": "7b21e8c6-f4aa-4872-af85-152c077232d5",
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
              "id": "827d6b13-d48b-41b3-97ca-ccf623271b94"
            }
          ]
        },
        {
          "id": "0e9c1600-e4a7-4f22-97e5-692c74b5bd9b",
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
              "id": "c00442f3-f666-409a-9c19-5ad1b2921fa3"
            }
          ]
        },
        {
          "id": "1c147c51-91eb-4809-aeda-73fa6d35560d",
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
              "id": "d851b8b2-2864-4aa5-b98b-9826c0b84779"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "ccd8ac77-e2cc-4446-9e95-2b1042160335",
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
              "id": "f80e3a77-30de-453a-8ca1-35a527cdf47a"
            }
          ]
        },
        {
          "id": "cb7801a8-7d13-4c6a-be1a-65a89b777881",
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
              "id": "0a6d2f4f-5bcc-45ae-a290-0ed952cd10eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "139cd956-50e7-452a-ba9b-4081889e90d6",
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
              "id": "c54ea934-5d92-411a-9e98-4ca1ff9551e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Explore",
      "item": [
        {
          "id": "17a0c7e6-83a4-4264-a1b6-20bf01520d16",
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
              "id": "9fcdc0e1-cbae-466b-8e69-5c7c6ee6b297"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "622b84b2-0ba7-4086-83a8-85068988b280",
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
              "id": "b7aafc8f-8a12-4653-a6e6-b6f84eba3e7f"
            }
          ]
        },
        {
          "id": "e84499cb-f25b-4184-9c5d-e573334144d8",
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
              "id": "25d2ebdf-e05e-48d1-9ae7-33f60b7e0f6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Owned",
      "item": [
        {
          "id": "960ca475-12dc-47bb-93ee-95ef3134892a",
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
              "id": "3bfed538-7607-4c61-97c6-acddaf73662a"
            }
          ]
        },
        {
          "id": "d5753ed3-600d-4dfa-ba1d-27ee8f3d6ed2",
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
              "id": "11d91922-8ae9-4fc3-829f-8537c517ae19"
            }
          ]
        },
        {
          "id": "af8aa7bd-eca1-4481-adf3-f97df1d263c1",
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
              "id": "3e389d79-174f-4a75-96a5-5322470c5bab"
            }
          ]
        },
        {
          "id": "fbefcf62-fb85-4e94-bc6a-fdbfcf45e1b0",
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
              "id": "0e693a0f-837b-45d8-acc6-d7425dd986b5"
            }
          ]
        },
        {
          "id": "478c5c62-2ed8-4260-a523-4c7ad3a14634",
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
              "id": "cd72fadb-3713-4320-9b25-094f5d347e07"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "3adfe269-bcc6-4b48-815c-dffe24c26b41",
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
              "id": "6867452a-ab13-4b29-af5a-768a53df045b"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "fdc864de-92a1-4d7e-badd-8351d9872cc6",
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
              "id": "e1d16fc0-9066-4530-b4b3-02f91a67c6a3"
            }
          ]
        },
        {
          "id": "310515d7-0775-44e3-a418-929a1eb3eaae",
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
              "id": "985364fb-0825-4b0b-aaff-4f854b4d3fac"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "6cf35b7e-fc87-4d8b-bfd7-176b1b7c8214",
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
              "id": "7128cc74-fa1d-4521-80b6-3610f3b658c2"
            }
          ]
        },
        {
          "id": "56da6ddd-74b1-421b-84fa-69d05fa13f66",
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
              "id": "a1acc977-4374-4889-971c-54c53bab509a"
            }
          ]
        }
      ]
    },
    {
      "name": "Dele",
      "item": [
        {
          "id": "d6478fae-b450-44b6-acd2-1d9792e82d74",
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
              "id": "4f77ac5d-afad-4300-93dd-46529f8831dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Podcast",
      "item": [
        {
          "id": "d8860b15-a684-420c-8b7d-aa83e7e58928",
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
              "id": "f046a122-0e45-4349-abb5-97a6f0749ee0"
            }
          ]
        }
      ]
    }
  ]
}