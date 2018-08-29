---
swagger: "2.0"
info:
  title: Salesforce
  description: Explore the beta Salesforce REST API to integrate CRM.
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/sobjects/User/{id}/password:
    delete:
      summary: Delete Version Sobjects User  Password
      description: Resets an user password
      operationId: version.sobjects.User.id.password.delete
      responses:
        200:
          description: OK
      tags:
      - version
      - sobjects
      - user
      - ""
      - password
definitions: []
x-collection-name: Salesforce
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