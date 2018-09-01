---
swagger: "2.0"
info:
  title: System Award Management API
  description: sam.gov is the System for Award Management. It is the site on which
    all vendors, grantees, receivers of federal financial assistance, and other entities
    doing business with the government must register prior to receiving an award.  The
    Registrations API currently provides the publicly available data for a specific
    entity along with status and progress information for that registration.
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
      parameters:
      - in: query
        name: api_key
        description: An API Key from api
        type: string
      - in: path
        name: registrationId
        description: DUNS+4 number (no '-' sign) of the registration to be fetched
        type: string
      responses:
        200:
          description: Successful response
          schema:
            type: array
            items:
              $ref: '#/definitions/SAM Registration'
      tags:
      - ""
definitions:
  SAM Registration:
    properties:
      duns:
        description: This is a default description.
        type: string
      duns4:
        description: This is a default description.
        type: string
      cage:
        description: This is a default description.
        type: string
      ncage:
        description: This is a default description.
        type: string
      dodaac:
        description: This is a default description.
        type: string
      purposeOfRegistration:
        description: This is a default description.
        type: string
      registrationDate:
        description: This is a default description.
        type: string
      expirationDate:
        description: This is a default description.
        type: string
      activationDate:
        description: This is a default description.
        type: string
      lastUpdatedDate:
        description: This is a default description.
        type: string
  "":
    properties:
      firstName:
        description: This is a default description.
        type: string
      lastName:
        description: This is a default description.
        type: string
      middleInitial:
        description: This is a default description.
        type: string
      address:
        description: This is a default description.
        type: string
      usPhone:
        description: This is a default description.
        type: string
      usPhoneExt:
        description: This is a default description.
        type: string
      nonUsPhone:
        description: This is a default description.
        type: string
      nonUsPhoneExt:
        description: This is a default description.
        type: string
      email:
        description: This is a default description.
        type: string
      line1:
        description: This is a default description.
        type: string
x-collection-name: System Award Management
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