swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  graph/embed/:embed_id/enable:
    get:
      summary: Get Graph Embed Embed  Enable
      description: Enable a specified embed.
      operationId: getGraphEmbedEmbedEnable
      x-api-path-slug: graphembedembed-idenable-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Graph
      - Embed
      - Embed
      - ""
      - Enable