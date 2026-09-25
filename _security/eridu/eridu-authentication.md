---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eridu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eridu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eridu
provider_slug: eridu
scheme_count: 1
schemes:
- description: 'WordPress application passwords (HTTP Basic: username + application password). Advertised by the site''s own API index at https://eridu.ai/wp-json/ under `authentication.application-passwords`. Required only for write methods and non-public contexts; every operation in this document is anonymously readable.'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/eridu-content-api-openapi.yml
  - openapi/eridu-discovery-api-openapi.yml
  - openapi/eridu-media-api-openapi.yml
  - openapi/eridu-oembed-api-openapi.yml
  - openapi/eridu-pages-api-openapi.yml
  - openapi/eridu-search-api-openapi.yml
  - openapi/eridu-taxonomy-api-openapi.yml
  type: http
slug: eridu-authentication
source_filename: eridu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/eridu-content-api-openapi.yml, openapi/eridu-discovery-api-openapi.yml, openapi/eridu-media-api-openapi.yml,\n  openapi/eridu-oembed-api-openapi.yml, openapi/eridu-pages-api-openapi.yml, openapi/eridu-search-api-openapi.yml,\n  openapi/eridu-taxonomy-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress application passwords (HTTP Basic: username + application password).\n    Advertised by the site''s own API index at https://eridu.ai/wp-json/ under `authentication.application-passwords`.\n    Required only for write methods and non-public contexts; every operation in this document\n    is anonymously readable.'\n  sources:\n  - openapi/eridu-content-api-openapi.yml\n  - openapi/eridu-discovery-api-openapi.yml\n  - openapi/eridu-media-api-openapi.yml\n  - openapi/eridu-oembed-api-openapi.yml\n  - openapi/eridu-pages-api-openapi.yml\n\
  \  - openapi/eridu-search-api-openapi.yml\n  - openapi/eridu-taxonomy-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/authentication/eridu-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Infrastructure
- Networking
- Semiconductors
- Data Center
- Silicon
- Network Switching
- Interconnect
- Hardware
- Content
---
