---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "443"
tags: Templates
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box Create Metadata Template
  x-api-slug: box
  description: Used to create a new metadata template with the specified schema.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//metadata_templates/schema
  tags: Documents,Metadata, Templates, Schema
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/metadata-templatesschema-post-openapi.md
- name: Box Get Enterprise Metadata
  x-api-slug: box
  description: Used to retrieve all metadata templates within a user's enterprise.
    Currently only the enterprise scope is supported.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//metadata_templates/{SCOPE}
  tags: Documents,Metadata, Templates, Scope
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/metadata-templatesscope-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/metadata-templatesscope-get-openapi.md
- name: Box Get Metadata Template
  x-api-slug: box
  description: Used to retrieve the schema for a given metadata template.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//metadata_templates/{SCOPE}/{TEMPLATE}/schema
  tags: Documents,Metadata, Templates, Scope, Template, Schema
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/metadata-templatesscopetemplateschema-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/metadata-templatesscopetemplateschema-get-openapi.md
- name: Box Update Metadata Template
  x-api-slug: box
  description: Used to update the schema of an existing template.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//metadata_templates/{SCOPE}/{TEMPLATE}/schema
  tags: Documents,Metadata, Templates, Scope, Template, Schema
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/metadata-templatesscopetemplateschema-put-openapi.md
- name: Box
  x-api-slug: box
  description: Box.net provides a sophisticated API for their online document sharing
    and collaboration web application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/box/openapi.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---