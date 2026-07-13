---
api_key_in: []
api_specs:
- filename: midjourney-image-generation-openapi.yml
  format: yaml
  label: Midjourney Image Generation API
  slug: image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midjourney/refs/heads/main/openapi/midjourney-image-generation-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Midjourney Authentication
name_suffix: Authentication
oauth_flows: []
overview: midjourney secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: midjourney
provider_slug: midjourney
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: API key obtained from the Midjourney Enterprise dashboard. Include in the Authorization header as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/midjourney-image-generation-openapi.yml
  type: http
slug: midjourney-authentication
source_filename: midjourney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/midjourney-image-generation-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: API key obtained from the Midjourney Enterprise dashboard. Include in the Authorization\n    header as a Bearer token.\n  sources:\n  - openapi/midjourney-image-generation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midjourney/refs/heads/main/authentication/midjourney-authentication.yml
summary_line: http · 1 scheme
tags: []
---
