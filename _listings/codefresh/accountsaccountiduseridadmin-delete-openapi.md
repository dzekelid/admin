---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Delete Accounts Admin
  description: Delete accounts admin.
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/{userId}/admin:
    delete:
      summary: Delete Accounts Admin
      description: Delete accounts admin.
      operationId: deleteAccountsAccountUserAdmin
      x-api-path-slug: accountsaccountiduseridadmin-delete
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Admin
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