---
swagger: "2.0"
x-collection-name: System Award Management
x-complete: 0
info:
  title: System Award Management API Find a registration by its DUN+4 number
  description: If the entity only has a 9-digit DUNS number, pad the end to include
    4 zeros
  version: 1.0.0
host: api.data.gov
basePath: /sam/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /registrations/{registrationId}:
    get:
      summary: Find a registration by its DUN+4 number
      description: If the entity only has a 9-digit DUNS number, pad the end to include
        4 zeros
      operationId: getData
      x-api-path-slug: registrationsregistrationid-get
      parameters:
      - in: query
        name: api_key
        description: An API Key from api
        type: string
      - in: path
        name: registrationId
        description: DUNS+4 number (no - sign) of the registration to be fetched
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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