---
api_key_in: []
api_specs:
- filename: contentful-openapi.yml
  format: yaml
  label: Contentful Content Delivery API
  slug: contentful-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/openapi/contentful-openapi.yml
- filename: contentful-webhooks-asyncapi.yml
  format: yaml
  label: Contentful Webhooks
  slug: contentful-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/openapi/contentful-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Contentful Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contentful secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contentful
provider_slug: contentful
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/contentful-openapi.yml
  type: http
slug: contentful-authentication
source_filename: contentful-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contentful-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/contentful-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/authentication/contentful-authentication.yml
summary_line: http · 1 scheme
tags:
- CMS
- Content
---
