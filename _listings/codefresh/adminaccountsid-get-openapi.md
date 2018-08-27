---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Get Admin Accounts
  description: Get admin accounts.
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
    post:
      summary: Post Accounts Admin
      description: Post accounts admin.
      operationId: postAccountsAccountUserAdmin
      x-api-path-slug: accountsaccountiduseridadmin-post
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
  /admin/accounts/addpendinguser:
    post:
      summary: Post Admin Accounts Addpendinguser
      description: Post admin accounts addpendinguser.
      operationId: postAdminAccountsAddpendinguser
      x-api-path-slug: adminaccountsaddpendinguser-post
      parameters:
      - in: body
        name: newUser
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
      - Pendinguser
  /admin/accounts/{id}/update:
    post:
      summary: Post Admin Accounts Update
      description: Post admin accounts update.
      operationId: postAdminAccountsUpdate
      x-api-path-slug: adminaccountsidupdate-post
      parameters:
      - in: body
        name: accountDetails
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/{id}:
    delete:
      summary: Delete Admin Accounts
      description: Delete admin accounts.
      operationId: deleteAdminAccounts
      x-api-path-slug: adminaccountsid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
    get:
      summary: Get Admin Accounts
      description: Get admin accounts.
      operationId: getAdminAccounts
      x-api-path-slug: adminaccountsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
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