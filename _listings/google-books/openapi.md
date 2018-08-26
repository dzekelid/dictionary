---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
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
---