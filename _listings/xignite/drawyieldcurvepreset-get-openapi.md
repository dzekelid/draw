---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Draw Yield Curve Preset
  description: Draw a yield curve for a rate family.
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  Draw, Rate, , Custom:
    get:
      summary: Draw Rate Chart Custom
      description: Draw a custom rate chart for a date range.
      operationId: postDrawratechartcustom
      x-api-path-slug: draw-rate--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Custom
  'Draw, Rate, ':
    get:
      summary: Draw Rate Chart
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechart
      x-api-path-slug: draw-rate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
  Draw, Rate, , Preset:
    get:
      summary: Draw Rate Chart Preset
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechartpreset
      x-api-path-slug: draw-rate--preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Preset
  /DrawYieldCurve:
    get:
      summary: Draw Yield Curve
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurve
      x-api-path-slug: drawyieldcurve-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
  /DrawYieldCurvePreset:
    get:
      summary: Draw Yield Curve Preset
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurvepreset
      x-api-path-slug: drawyieldcurvepreset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
      - Preset
  /DrawYieldCurveCustom:
    get:
      summary: Draw Yield Curve Custom
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurvecustom
      x-api-path-slug: drawyieldcurvecustom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
      - Custom
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