---
api_key_in:
- header
api_specs:
- filename: swagger
  format: yaml
  label: Getty Images API
  slug: platform
  spec_type: OpenAPI
  url: https://api.gettyimages.com/swagger
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Getty Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Getty Images secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Getty Images
provider_slug: getty
scheme_count: 2
schemes:
- description: API consumer key, sent as the api-key header.
  in: header
  name: apiKey
  parameter: Api-Key
  sources:
  - openapi/getty-openapi.yml
  type: apiKey
- description: OAuth 2.0 client credentials for elevated operations.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.gettyimages.com/oauth2/token
  name: oauth2
  sources:
  - openapi/getty-openapi.yml
  type: oauth2
slug: getty-authentication
source_filename: getty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/getty-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: API consumer key, sent as the api-key header.\n  sources:\n  - openapi/getty-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.gettyimages.com/oauth2/token\n    scopes: 2\n  description: OAuth 2.0 client credentials for elevated operations.\n  sources:\n  - openapi/getty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getty/refs/heads/main/authentication/getty-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Stock Media
- Images
- Editorial
- Video
- Music
- Licensing
---
