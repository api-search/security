---
api_key_in:
- header
- query
api_specs:
- filename: outbrain-amplify-api-openapi.yml
  format: yaml
  label: Outbrain Amplify API
  slug: outbrain-amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-amplify-api-openapi.yml
- filename: outbrain-engage-api-openapi.yml
  format: yaml
  label: Outbrain Engage API
  slug: outbrain-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-engage-api-openapi.yml
- filename: outbrain-teads-conversion-api-openapi.yml
  format: yaml
  label: Teads / Outbrain Conversion API
  slug: outbrain-teads-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-teads-conversion-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Outbrain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outbrain secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Outbrain
provider_slug: outbrain
scheme_count: 4
schemes:
- description: Token returned from /login. Send on all authenticated requests.
  in: header
  name: OBTokenAuth
  parameter: OB-TOKEN-V1
  sources:
  - openapi/outbrain-amplify-api-openapi.yml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/outbrain-amplify-api-openapi.yml
  type: http
- in: query
  name: PublisherKeyAuth
  parameter: publisherKey
  sources:
  - openapi/outbrain-engage-api-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/outbrain-teads-conversion-api-openapi.yml
  type: http
slug: outbrain-authentication
source_filename: outbrain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/outbrain-amplify-api-openapi.yml, openapi/outbrain-engage-api-openapi.yml, openapi/outbrain-teads-conversion-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: OBTokenAuth\n  type: apiKey\n  in: header\n  parameter: OB-TOKEN-V1\n  description: Token returned from /login. Send on all authenticated requests.\n  sources:\n  - openapi/outbrain-amplify-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/outbrain-amplify-api-openapi.yml\n- name: PublisherKeyAuth\n  type: apiKey\n  in: query\n  parameter: publisherKey\n  sources:\n  - openapi/outbrain-engage-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/outbrain-teads-conversion-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/authentication/outbrain-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Advertising
- Native Advertising
- Open Web
- CTV
- Connected TV
- Video Advertising
- Content Discovery
- Programmatic
- Performance Marketing
- AdTech
- Teads
---
