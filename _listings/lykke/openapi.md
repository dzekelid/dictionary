---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Client/dictionary/{key}:
    get:
      summary: Get API Client Dictionary Key
      description: Get api client dictionary key.
      operationId: ApiClientDictionaryByKeyGet
      x-api-path-slug: apiclientdictionarykey-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
    delete:
      summary: Delete API Client Dictionary Key
      description: Delete api client dictionary key.
      operationId: ApiClientDictionaryByKeyDelete
      x-api-path-slug: apiclientdictionarykey-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
  /api/Client/dictionary:
    put:
      summary: Put API Client Dictionary
      description: Put api client dictionary.
      operationId: ApiClientDictionaryPut
      x-api-path-slug: apiclientdictionary-put
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: keyValue
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
    post:
      summary: Add API Client Dictionary
      description: Add api client dictionary.
      operationId: ApiClientDictionaryPost
      x-api-path-slug: apiclientdictionary-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: keyValue
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
  /api/Dictionary/{key}:
    get:
      summary: Get API Dictionary Key
      description: Get api dictionary key.
      operationId: ApiDictionaryByKeyGet
      x-api-path-slug: apidictionarykey-get
      parameters:
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Dictionary
      - Key
  /api/Dictionary:
    get:
      summary: Get API Dictionary
      description: Get api dictionary.
      operationId: ApiDictionaryGet
      x-api-path-slug: apidictionary-get
      responses:
        200:
          description: OK
      tags:
      - Dictionary
---