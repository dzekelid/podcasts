---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Explore Category Items
  version: v1
  description: 'This API returns information and items of a specific category. The
    response contains two properties at root level:'
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /show/{show_id}/episodes:
    post:
      summary: Create podcast
      description: Creates new podcast episode.
      operationId: postShowShowEpisodes
      x-api-path-slug: showshow-idepisodes-post
      parameters:
      - in: query
        name: category_id
        description: Episode category
      - in: query
        name: description
        description: Episode description
      - in: query
        name: download_enabled
        description: Enable / disable download (defaults to true)
      - in: query
        name: explicit
        description: True if the episode contains explicit content (defaults to false)
      - in: query
        name: hidden
        description: True if the episode should be private (defaults to false)
      - in: query
        name: media_id
        description: The single media_id or ordered list of media_id that compose
          the episode
      - in: query
        name: shares
        description: The channels on which this episode has to be shared
      - in: path
        name: show_id
        description: Unique show id
      - in: query
        name: tags
        description: Episode tags (comma separated)
      - in: query
        name: title
        description: Episode title
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Podcast
  /categories/flat:
    get:
      summary: Get Categories
      description: Retrieves all categories in Spreaker
      operationId: getCategoriesFlat
      x-api-path-slug: categoriesflat-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Categories
  /episode/<episode_id>/image:
    put:
      summary: Change Episode Image
      description: Change Episode Image
      operationId: putEpisode<episode>Image
      x-api-path-slug: episodeepisode-idimage-put
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      - in: query
        name: image_id
        description: The id of the image to set to the episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - Episode
      - Image
  /episode/{episode_id}:
    delete:
      summary: Delete Episode
      description: Deletes an episode. Theres no way to recover a deleted episode.
      operationId: deleteEpisodeEpisode
      x-api-path-slug: episodeepisode-id-delete
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
    get:
      summary: Get Episode
      description: Retrieves an episode by unique identifier.
      operationId: getEpisodeEpisode
      x-api-path-slug: episodeepisode-id-get
      parameters:
      - in: path
        name: episode_id
        description: The episode unique id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
    put:
      summary: Edit Episode
      description: Edit episode info (eg. title, description, category, tags, ...)
      operationId: putEpisodeEpisode
      x-api-path-slug: episodeepisode-id-put
      parameters:
      - in: query
        name: category_id
        description: Episode category
      - in: query
        name: description
        description: Episode description, max length 10k chars
      - in: path
        name: episode_id
        description: the episode id
      - in: query
        name: tags
        description: Episode tags (comma separated)
      - in: query
        name: title
        description: Episode title, max length 40 chars
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Edit
      - Episode
  /episode/{episode_id}/media:
    get:
      summary: Get Episode Media List
      description: Get Episode Media List
      operationId: getEpisodeEpisodeMedia
      x-api-path-slug: episodeepisode-idmedia-get
      parameters:
      - in: path
        name: episode_id
        description: Unique id of episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Media
      - List
  /episode/{episode_id}/streams/icy:
    get:
      summary: Get Episode Streams
      description: The response contains a collection of ICY streams.
      operationId: getEpisodeEpisodeStreamsIcy
      x-api-path-slug: episodeepisode-idstreamsicy-get
      parameters:
      - in: query
        name: episode_id
        description: The episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Streams
  /episode/{episode_id}/streams/rtmp:
    get:
      summary: Get Episode Streams
      description: The response contains a collection of RTMP / RTMPT streams.
      operationId: getEpisodeEpisodeStreamsRtmp
      x-api-path-slug: episodeepisode-idstreamsrtmp-get
      parameters:
      - in: path
        name: episode_id
        description: The episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Streams
  /episodes/live:
    get:
      summary: Get Live Episodes
      description: Retrieves all live episodes at the moment of the request
      operationId: getEpisodesLive
      x-api-path-slug: episodeslive-get
      parameters:
      - in: query
        name: show_id
        description: An list of show_id applied as a filter
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Live
      - Episodes
  /explore/{category_id}:
    get:
      summary: Explore Category Items
      description: 'This API returns information and items of a specific category.
        The response contains two properties at root level:'
      operationId: getExploreCategory
      x-api-path-slug: explorecategory-id-get
      parameters:
      - in: query
        name: explore_category
        description: contains category information, the exact same information exported
          by /explore/categories API
      - in: query
        name: items
        description: contains a sorted list of shows or episodes, depending on the
          category type (type 1 and 3 contain episodes, type 2 contains shows)
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Explore
      - Category
      - Items
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---