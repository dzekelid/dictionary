---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 0
info:
  title: Google Books API Get Dictionary
  description: Returns a list of offline dictionary metadata available
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dictionary/listOfflineMetadata:
    get:
      summary: Get Dictionary
      description: Returns a list of offline dictionary metadata available
      operationId: books.dictionary.listOfflineMetadata
      x-api-path-slug: dictionarylistofflinemetadata-get
      parameters:
      - in: query
        name: cpksver
        description: The device/version ID from which to request the data
      responses:
        200:
          description: OK
      tags:
      - Dictionary
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