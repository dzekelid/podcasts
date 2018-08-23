---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Get List of Following
  version: v1
  description: Get List of Following
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
    get:
      summary: Get Show Episodes
      description: Retrieves all listenable episodes by show (both live and podcast,
        ordered by published_at DESC).
      operationId: getShowShowEpisodes
      x-api-path-slug: showshow-idepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
      - Episodes
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
  /library/{user_id}:
    post:
      summary: Create Media
      description: Upload a new Media in the specified user library
      operationId: postLibraryUser
      x-api-path-slug: libraryuser-id-post
      parameters:
      - in: path
        name: Filedata
        description: The file to upload, encoded multipart/form-data
      - in: query
        name: length
        description: The media length in milliseconds
      - in: query
        name: style_id
        description: The music style associated to this media
      - in: query
        name: type
        description: 'The media type: can be one of SONG, JINGLE, LOOP, UNKNOWN, EFFECT,
          EPISODE'
      - in: path
        name: user_id
        description: The unique user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Media
  /library/{user_id}/effects/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserEffectsOwned
      x-api-path-slug: libraryuser-ideffectsowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/jingles/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserJinglesOwned
      x-api-path-slug: libraryuser-idjinglesowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/loops/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserLoopsOwned
      x-api-path-slug: libraryuser-idloopsowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/songs/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserSongsOwned
      x-api-path-slug: libraryuser-idsongsowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: query
        name: user_id
        description: Users id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/soundtracks/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserSoundtracksOwned
      x-api-path-slug: libraryuser-idsoundtracksowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /lives/top:
    get:
      summary: Get Top Live Episodes
      description: Retrieves live episodes sorted by rank
      operationId: getLivesTop
      x-api-path-slug: livestop-get
      parameters:
      - in: query
        name: I
        description: The rank is language - based
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Top
      - Live
      - Episodes
  /media/{media_id}:
    get:
      summary: Get Media
      description: Retrieves a Media by unique identifier.
      operationId: getMediaMedia
      x-api-path-slug: mediamedia-id-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Media
  /search/{query}:
    get:
      summary: Search users, shows and episodes
      description: Search users, shows and episodes
      operationId: getSearchQuery
      x-api-path-slug: searchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Users
      - ""
      - Shows
      - Episodes
  /show/search/{query}:
    get:
      summary: Search Shows
      description: This API allows to find shows.
      operationId: getShowSearchQuery
      x-api-path-slug: showsearchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Shows
  /show/{show_id}:
    delete:
      summary: Dele Show
      description: Deletes a show. Theres no way to recover a deleted show. Only show
        without episodes in it can be deleted.
      operationId: deleteShowShow
      x-api-path-slug: showshow-id-delete
      parameters:
      - in: query
        name: description
        description: Show description
      - in: query
        name: email
        description: Shows email contact
      - in: query
        name: facebook_url
        description: Shows facebook page url
      - in: path
        name: show_id
        description: The show id
      - in: query
        name: skype_name
        description: Shows skypy account name
      - in: query
        name: sms_number
        description: Shows sms number (eg
      - in: query
        name: tel_number
        description: Shows telephone number (eg
      - in: query
        name: title
        description: Show title
      - in: query
        name: twitter_name
        description: Shows twitter account name
      - in: query
        name: website_url
        description: Shows website url
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Dele
      - Show
    get:
      summary: Get Show
      description: Retrieves show information.
      operationId: getShowShow
      x-api-path-slug: showshow-id-get
      parameters:
      - in: path
        name: show_id
        description: The show id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
    put:
      summary: Edit Show
      description: Edit show info (name, description and contacts).
      operationId: putShowShow
      x-api-path-slug: showshow-id-put
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Edit
      - Show
  /show/{show_id}/episodes/all:
    get:
      summary: Get All Show Episodes
      description: Retrieves all episodes by show (both live and podcast, ordered
        by published_at DESC).
      operationId: getShowShowEpisodesAll
      x-api-path-slug: showshow-idepisodesall-get
      parameters:
      - in: path
        name: show_id
        description: The unique show id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
      - Episodes
  /shows:
    post:
      summary: Create Show
      description: Create a new Show.
      operationId: postShows
      x-api-path-slug: shows-post
      parameters:
      - in: query
        name: title
        description: Show title
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
  /user/{followed_id}/fans:
    get:
      summary: Get List of Followers
      description: Get List of Followers
      operationId: getUserFollowedFans
      x-api-path-slug: userfollowed-idfans-get
      parameters:
      - in: path
        name: followed_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - List
      - Of
      - Followers
    post:
      summary: Follow User
      description: Follow User
      operationId: postUserFollowedFans
      x-api-path-slug: userfollowed-idfans-post
      parameters:
      - in: path
        name: followed_id
        description: Allows the authenticating user to follow the user specified in
          the  parameter
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Follow
      - User
  /user/{followed_id}/fans/{follower_id}:
    delete:
      summary: Unfollow User
      description: Unfollow User
      operationId: deleteUserFollowedFansFollower
      x-api-path-slug: userfollowed-idfansfollower-id-delete
      parameters:
      - in: path
        name: followed_id
      - in: path
        name: follower_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Unfollow
      - User
  /user/{follower_id}/users/fan:
    get:
      summary: Get List of Following
      description: Get List of Following
      operationId: getUserFollowerUsersFan
      x-api-path-slug: userfollower-idusersfan-get
      parameters:
      - in: path
        name: follower_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - List
      - Of
      - Following
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