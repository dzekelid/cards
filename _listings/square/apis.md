---
name: Square
x-slug: square
description: Square helps millions of sellers run their business- from secure credit
  card processing to point of sale solutions. Get paid faster with Square and sign
  up today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
x-kinRank: "9"
x-alexaRank: "2436"
tags: Cards
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Provides summary information for all of a business's employee
    timecards.
  x-api-slug: square-connect-api
  description: Provides summary information for all of a business's employee timecards.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/me/timecards
  tags: Provides,Summary,Information,Of,Businesss,Employee,Timecards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/square/v1metimecards-get-openapi.md
- name: Square Connect API Deletes a timecard. Deleted timecards are still accessible
    from Connect API endpoints, but the value of their deleted field is set to true.
    See Handling deleted timecards for more information.
  x-api-slug: square-connect-api
  description: Deletes a timecard. Deleted timecards are still accessible from Connect
    API endpoints, but the value of their deleted field is set to true. See Handling
    deleted timecards for more information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/me/timecards/{timecard_id}
  tags: S,Timecard,,D,Timecards,Are,Still,Accessible,From,Connect,Endpoints,,But,Value,Of,Their,Deleted,Field,Is,Set,To,True,,See,Handling,Deleted,Timecardsmore,Information
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/square/v1metimecardstimecard-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/square/v1metimecardstimecard-id-delete-openapi.md
- name: Square Connect API Modifies a timecard's details. This creates an API_EDIT
    event for the timecard. You can view a timecard's event history with the List
    Timecard Events endpoint.
  x-api-slug: square-connect-api
  description: Modifies a timecard's details. This creates an API_EDIT event for the
    timecard. You can view a timecard's event history with the List Timecard Events
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/me/timecards/{timecard_id}
  tags: Modifies,Timecards,Details,,This,Creates,EDIT,Eventthe,Timecard,,You,Can,View,Timecards,Event,History,List,Timecard,Events,Endpoint
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/square/v1metimecardstimecard-id-put-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Square helps millions of sellers run their business- from secure credit
    card processing to point of sale solutions. Get paid faster with Square and sign
    up today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com//
  tags: Cards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-crunchbase
  url: https://crunchbase.com/organization/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-email
  url: press@squareup.com
- type: x-email
  url: security@squareup.com
- type: x-email
  url: lawenforcement@squareup.com
- type: x-email
  url: redemption@squareup.com
- type: x-email
  url: privacy@squareup.com
- type: x-email
  url: community@squareup.com
- type: x-email
  url: noreply@messaging.squareup.com
- type: x-email
  url: ir@squareup.com
- type: x-email
  url: takedowns@squareup.com
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: http://squareup.com
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---