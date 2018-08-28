---
name: AWS Lightsale
x-slug: aws-lightsale
description: Amazon Lightsail is the easiest way to get started with AWS for developers
  who just need virtual private servers. Lightsail includes everything you need to
  launch your project quickly - a virtual machine, SSD-based storage, data transfer,
  DNS management, and a static IP - for a low, predictable price. You manage those
  Lightsail servers through the Lightsail console or by using the API or command-line
  interface (CLI).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Enterprise
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/aws-lightsale/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Lightsale API - Create Domain Entry
  x-api-slug: actioncreatedomainentry-get
  description: |-
    Creates one of the following entry records associated with the domain: A record, CNAME
          record, TXT record, or MX record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/aws-lightsale/actioncreatedomainentry-get-openapi.md
- name: AWS Lightsale API - Delete Domain Entry
  x-api-slug: actiondeletedomainentry-get
  description: Deletes a specific domain entry.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/aws-lightsale/actiondeletedomainentry-get-openapi.md
- name: AWS Lightsale API - Update Domain Entry
  x-api-slug: actionupdatedomainentry-get
  description: Updates a domain recordset after it is created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/aws-lightsale/actionupdatedomainentry-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.lambda.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.lightsale.stack.network
- type: x-documentation
  url: https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/Welcome.html?fid=6DDA37DF97F08F8B-23761D4A79F7B1E
- type: x-pricing
  url: https://amazonlightsail.com/pricing/
- type: x-website
  url: https://amazonlightsail.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---