---
api_key_in: []
api_specs:
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Customers API
  slug: vimeo-ott-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Products API
  slug: vimeo-ott-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Videos API
  slug: vimeo-ott-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Collections API
  slug: vimeo-ott-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Authorizations API
  slug: vimeo-ott-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
- filename: vimeo-ott-openapi.yml
  format: yaml
  label: Vimeo OTT Analytics API
  slug: vimeo-ott-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/openapi/vimeo-ott-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vimeo Ott Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vimeo OTT secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vimeo OTT
provider_slug: vimeo-ott
scheme_count: 1
schemes:
- description: HTTP Basic Auth. Supply your Vimeo OTT API key as the username and leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vimeo-ott-openapi.yml
  type: http
slug: vimeo-ott-authentication
source_filename: vimeo-ott-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vimeo-ott-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth. Supply your Vimeo OTT API key as the username and leave the\n    password blank.\n  sources:\n  - openapi/vimeo-ott-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vimeo-ott/refs/heads/main/authentication/vimeo-ott-authentication.yml
summary_line: http · 1 scheme
tags:
- OTT
- Video
- SVOD
- Streaming
- Media
- Subscriptions
- VHX
---
