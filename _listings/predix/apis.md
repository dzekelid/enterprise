---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Enterprise
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Analytics Catalog - Upload an artifact and attach it to an analytic catalog
    entry.
  x-api-slug: apiv1catalogartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an analytic catalog entry. The multipart MIME structure must have the catalog
    entry id tagged as 'catalogEntryId',  the file contents tagged as 'file',  the
    artifact type tagged as 'type', and  a description (under 1024 characters) tagged
    as 'description'. Artifact types can be any string.  Artifacts with the type 'executable'
    must contain the executable for the analytic.   An analytic can only have 1 artifact
    labelled as 'executable'(See the documentation for more information regarding
    these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/predix/apiv1catalogartifacts-post-openapi.md
- name: Analytics Framework - Upload an artifact and attach it to an analytic catalog
    entry.
  x-api-slug: apiv1catalogartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an analytic catalog entry. The multipart MIME structure must have the catalog
    entry id tagged as 'catalogEntryId',  the file contents tagged as 'file',  the
    artifact type tagged as 'type', and  a description (under 1024 characters) tagged
    as 'description'. Artifact types can be any string.  Artifacts with the type 'executable'
    must contain the executable for the analytic.   An analytic can only have 1 artifact
    labelled as 'executable'(See the documentation for more information regarding
    these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/predix/apiv1catalogartifacts-post-openapi.md
- name: Analytics Framework - Upload an artifact and attach it to an orchestration
    configuration entry.
  x-api-slug: apiv2configorchestrationsartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an orchestration configuration entry. The multipart MIME structure must
    have the orchestration entry id tagged as 'orchestrationEntryId',  the file contents
    tagged as 'file',  the artifact type tagged as 'type', and  the name of artifact
    tagged as 'name'.  A description (under 1024 characters) tagged as 'description'
    can be optionally specified. Artifact types can be either 'portToFieldMap', 'bpmn'
    or any.   If the artifact type is 'portToFieldMap', specify the orchestration
    step ID tagged as 'stepId'.   Otherwise, 'name' will be used as 'stepId'.  (See
    the documentation for more information regarding these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/predix/apiv2configorchestrationsartifacts-post-openapi.md
- name: Analytics Runtime - Upload an artifact and attach it to an orchestration configuration
    entry.
  x-api-slug: apiv2configorchestrationsartifacts-post
  description: Upload a single artifact file in a multipart MIME structure and attach
    it to an orchestration configuration entry. The multipart MIME structure must
    have the orchestration entry id tagged as 'orchestrationEntryId',  the file contents
    tagged as 'file',  the artifact type tagged as 'type', and  the name of artifact
    tagged as 'name'.  A description (under 1024 characters) tagged as 'description'
    can be optionally specified. Artifact types can be either 'portToFieldMap', 'bpmn'
    or any.   If the artifact type is 'portToFieldMap', specify the orchestration
    step ID tagged as 'stepId'.   Otherwise, 'name' will be used as 'stepId'.  (See
    the documentation for more information regarding these files.)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enterprise/master/_listings/predix/apiv2configorchestrationsartifacts-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---