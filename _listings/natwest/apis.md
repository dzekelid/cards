---
name: NatWest
x-slug: natwest
description: National Westminster Bank, commonly known as NatWest, is a large retail
  and commercial bank in the United Kingdom. It was established in 1968 by the merger
  of National Provincial Bank (established 1833 as National Provincial Bank of England)
  and Westminster Bank (established 1834 as London County and Westminster Bank). Since
  2000 it has been part of the Royal Bank of Scotland Group. Following ring-fencing
  of the Groups core domestic business, the bank is a direct subsidiary of NatWest
  Holdings. NatWest Markets comprises its investment banking arm.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/natwest-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Cards
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/natwest/apis.md
specificationVersion: "0.14"
apis:
- name: NatWest Get Commercial Credit Cards
  x-api-slug: natwest
  description: This endpoint can contain multiple brands owned by a particular banking
    group. Each brand can own multiple SME Commercial Credit Card products.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/natwest-logo.png
  humanURL: https://personal.natwest.com/personal.html
  baseURL: https://openapi.natwest.com/open-banking/v2.1//commercial-credit-cards/
  tags: Commercial,Credit,Cards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/natwest/commercialcreditcards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/natwest/commercialcreditcards-get-openapi.md
- name: NatWest
  x-api-slug: natwest
  description: National Westminster Bank, commonly known as NatWest, is a large retail
    and commercial bank in the United Kingdom. It was established in 1968 by the merger
    of National Provincial Bank (established 1833 as National Provincial Bank of England)
    and Westminster Bank (established 1834 as London County and Westminster Bank).
    Since 2000 it has been part of the Royal Bank of Scotland Group. Following ring-fencing
    of the Groups core domestic business, the bank is a direct subsidiary of NatWest
    Holdings. NatWest Markets comprises its investment banking arm.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/natwest-logo.png
  humanURL: https://personal.natwest.com/personal.html
  baseURL: https://openapi.natwest.com/open-banking/v2.1/
  tags: Cards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cards/master/_listings/natwest/openapi.md
x-common:
- type: x-developer
  url: http://openbankingapis.io/uk/natwest
- type: x-documentation
  url: https://openbanking.atlassian.net/wiki/spaces/DZ/pages/54919225/Open+Data+API+Dashboard#
- type: x-twitter
  url: https://twitter.com/natwest_help
- type: x-website
  url: https://personal.natwest.com/personal.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---