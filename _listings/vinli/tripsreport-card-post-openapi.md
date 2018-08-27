---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 0
info:
  title: Vinli Report Card  for a Trip
  description: Report card  for a trip.
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trips/report_card:
    post:
      summary: Report Card  for a Trip
      description: Report card  for a trip.
      operationId: TripsReportCardPost
      x-api-path-slug: tripsreport-card-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Report
      - Card
      - Trip
  /report_cards/549d628c-48dc-412d-8087-44a9f82f187e:
    get:
      summary: Get a Specific Report Card
      description: Get a specific report card.
      operationId: ReportCards549d628c48dc412d808744a9f82f187eGet
      x-api-path-slug: report-cards549d628c48dc412d808744a9f82f187e-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Report
      - Card
  /devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/report_cards/overall:
    get:
      summary: Lifetime Report Card for a Device
      description: Lifetime report card for a device.
      operationId: Devices7eac0d62854f41c1A5b2Ba13c460058aReportCardsOverallGet
      x-api-path-slug: devices7eac0d62854f41c1a5b2ba13c460058areport-cardsoverall-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Lifetime
      - Report
      - Carda
      - Device
  /vehicles/8480c5b7-6f3e-40b3-a78e-3555617d44b0/report_cards:
    get:
      summary: Report Cards for a Vehicle
      description: Report cards for a vehicle.
      operationId: Vehicles8480c5b76f3e40b3A78e3555617d44b0ReportCardsGet
      x-api-path-slug: vehicles8480c5b76f3e40b3a78e3555617d44b0report-cards-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Report
      - Cardsa
      - Vehicle
  /devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/report_cards:
    get:
      summary: Report Cards for a Device
      description: Report cards for a device.
      operationId: Devices7eac0d62854f41c1A5b2Ba13c460058aReportCardsGet
      x-api-path-slug: devices7eac0d62854f41c1a5b2ba13c460058areport-cards-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Report
      - Cardsa
      - Device
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