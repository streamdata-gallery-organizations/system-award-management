---
name: System Award Management
x-slug: system-award-management
description: The SAM API is a RESTful method of retrieving public information about
  the businesses or individuals (referred to as &ldquo;entities&rdquo;) within the
  SAM data set. The entities publicly available data set can currently be retrieved
  on an entity-by-entity basis.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/53aa67a8-caec-11e3-9248-37414d200130.gif
x-kinRank: "8"
x-alexaRank: ""
tags: System Award Management
created: "2018-05-22"
modified: "2018-05-22"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/system-award-management/master/_listings/system-award-management/apis.md
specificationVersion: "0.14"
apis:
- name: System Award Management API Find a registration by its DUN+4 number
  x-api-slug: system-award-management-api
  description: If the entity only has a 9-digit DUNS number, pad the end to include
    4 zeros
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/53aa67a8-caec-11e3-9248-37414d200130.gif
  humanURL: http://gsa.github.io/sam_api/sam/
  baseURL: https://api.data.gov//sam/v1//registrations/{registrationId}
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/system-award-management/master/_listings/system-award-management/registrationsregistrationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/system-award-management/master/_listings/system-award-management/registrationsregistrationid-get-openapi.md
- name: System Award Management API
  x-api-slug: system-award-management-api
  description: The SAM API is a RESTful method of retrieving public information about
    the businesses or individuals (referred to as &ldquo;entities&rdquo;) within the
    SAM data set. The entities publicly available data set can currently be retrieved
    on an entity-by-entity basis.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/53aa67a8-caec-11e3-9248-37414d200130.gif
  humanURL: http://gsa.github.io/sam_api/sam/
  baseURL: https://api.data.gov//sam/v1
  tags: System Award Management
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/system-award-management/master/_listings/system-award-management/openapi.md
x-common:
- type: x-website
  url: http://gsa.github.io/sam_api/sam/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---