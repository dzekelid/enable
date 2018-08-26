---
swagger: "2.0"
x-collection-name: Viddler
x-complete: 1
info:
  title: Viddler  API
  description: the-viddler-api-exposes-viddleru2019s-key-features-to-those-that-would-like-to-build-custom-solutions-on-top-of-viddleru2019s-video-platform-
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.videos.enableAds:
    post:
      summary: Videos EnableAds
      description: Turn ads off for specified videos.
      operationId: videos-enableads
      x-api-path-slug: viddler-videos-enableads-post
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: video_ids
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - EnableAds
---