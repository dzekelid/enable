swagger: "2.0"
x-collection-name: RipaEx
x-complete: 1
info:
  title: RIPA Node Documentation
  description: this-is-a-documentation-for-ripanodehttpsgithub-comripaexripanode-built-with-swagger-ui-to-make-testing-a-breeze--if-you-find-any-issues-come-over-to-ripaexripanodetestapihttpsgithub-comripaexripanodetestapi-to-open-an-issue-or-even-better-send-a-pr-that-fixes-the-issue-the-community-ssl-public-api-used-as-test-host-is-provided-from-ripaex-iohttpswww-ripaex-io-
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/delegates/forging/enable:
    post:
      summary: Delegates Forging Enable
      description: Enable forging for a delegate.
      operationId: delegates.enableForging
      x-api-path-slug: apidelegatesforgingenable-post
      parameters:
      - in: query
        name: publicKey
        description: A valid RIPA Public Key
      - in: query
        name: secret
        description: A valid RIPA Passphrase
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Forging
      - Enable