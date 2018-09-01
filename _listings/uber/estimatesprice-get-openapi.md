---
swagger: "2.0"
x-collection-name: Uber
x-complete: 0
info:
  title: Uber Price Estimates
  description: The Price Estimates endpoint returns an estimated price range for each
    product offered at a given location. The price estimate is provided as a formatted
    string with the full price range and the localized currency symbol.<br><br>The
    response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217)
    currency code for situations requiring currency conversion. When surge is active
    for a particular product, its surge_multiplier will be greater than 1, but the
    price estimate already factors in this multiplier.
  version: 1.0.0
host: api.uber.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products:
    get:
      summary: Product Types
      description: The Products endpoint returns information about the Uber products
        offered at a given location. The response includes the display name and other
        details about each product, and lists the products in the proper display order.
      operationId: the-products-endpoint-returns-information-about-the-uber-products-offered-at-a-given-location-the-re
      x-api-path-slug: products-get
      parameters:
      - in: query
        name: latitude
        description: Latitude component of location
      - in: query
        name: longitude
        description: Longitude component of location
      responses:
        200:
          description: OK
      tags:
      - Transportation
  /estimates/price:
    get:
      summary: Price Estimates
      description: The Price Estimates endpoint returns an estimated price range for
        each product offered at a given location. The price estimate is provided as
        a formatted string with the full price range and the localized currency symbol.<br><br>The
        response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217)
        currency code for situations requiring currency conversion. When surge is
        active for a particular product, its surge_multiplier will be greater than
        1, but the price estimate already factors in this multiplier.
      operationId: the-price-estimates-endpoint-returns-an-estimated-price-range-for-each-product-offered-at-a-given-lo
      x-api-path-slug: estimatesprice-get
      parameters:
      - in: query
        name: end_latitude
        description: Latitude component of end location
      - in: query
        name: end_longitude
        description: Longitude component of end location
      - in: query
        name: start_latitude
        description: Latitude component of start location
      - in: query
        name: start_longitude
        description: Longitude component of start location
      responses:
        200:
          description: OK
      tags:
      - Transportation
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---