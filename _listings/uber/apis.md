---
name: Uber
x-slug: uber
description: The Uber API exposes a set of RESTful endpoints that enable your application
  to GET information such as time and price estimates about the products offered in
  a given location, request rides on behalf of authenticated users, and create ride
  reminders for users to take a ride at a specific time in the future.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Uber
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/apis.md
specificationVersion: "0.14"
apis:
- name: Uber Product Types
  x-api-slug: uber
  description: The Products endpoint returns information about the Uber products offered
    at a given location. The response includes the display name and other details
    about each product, and lists the products in the proper display order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1//products
  tags: Transportation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/products-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/products-get-openapi.md
- name: Uber Price Estimates
  x-api-slug: uber
  description: The Price Estimates endpoint returns an estimated price range for each
    product offered at a given location. The price estimate is provided as a formatted
    string with the full price range and the localized currency symbol.<br><br>The
    response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217)
    currency code for situations requiring currency conversion. When surge is active
    for a particular product, its surge_multiplier will be greater than 1, but the
    price estimate already factors in this multiplier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1//estimates/price
  tags: Transportation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/estimatesprice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/estimatesprice-get-openapi.md
- name: Uber Time Estimates
  x-api-slug: uber
  description: The Time Estimates endpoint returns ETAs for all products offered at
    a given location, with the responses expressed as integers in seconds. We recommend
    that this endpoint be called every minute to provide the most accurate, up-to-date
    ETAs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1//estimates/time
  tags: Transportation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/estimatestime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/estimatestime-get-openapi.md
- name: Uber User Profile
  x-api-slug: uber
  description: The User Profile endpoint returns information about the Uber user that
    has authorized with the application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1//me
  tags: Transportation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/me-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/me-get-openapi.md
- name: Uber User Activity
  x-api-slug: uber
  description: The User Activity endpoint returns data about a user's lifetime activity
    with Uber. The response will include pickup locations and times, dropoff locations
    and times, the distance of past requests, and information about which products
    were requested.<br><br>The history array in the response will have a maximum length
    based on the limit parameter. The response value count may exceed limit, therefore
    subsequent API requests may be necessary.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1//history
  tags: Transportation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/history-get-openapi.md
- name: Uber
  x-api-slug: uber
  description: The Uber API exposes a set of RESTful endpoints that enable your application
    to GET information such as time and price estimates about the products offered
    in a given location, request rides on behalf of authenticated users, and create
    ride reminders for users to take a ride at a specific time in the future.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uber-logo.png
  humanURL: https://uber.com
  baseURL: https://api.uber.com//v1
  tags: Uber
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uber/master/_listings/uber/openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://raw.githubusercontent.com/picsoung/apis.json/master/uber.json
- type: x-blog
  url: https://medium.com/streamrblog
- type: x-blog
  url: https://medium.com/@UberPubPolicy
- type: x-blog
  url: https://devblog.uber.com/
- type: x-blog-rss
  url: https://medium.com/feed/@UberPubPolicy
- type: x-blog-rss
  url: https://devblog.uber.com/feed/
- type: x-developer
  url: https://developer.uber.com/
- type: x-github
  url: https://github.com/uber
- type: x-transparency-report
  url: https://transparencyreport.uber.com/
- type: x-twitter
  url: https://twitter.com/uber_api
- type: x-twitter
  url: https://twitter.com/UberPubPolicy
- type: x-website
  url: https://uber.com
- type: x-website
  url: http://medium.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---