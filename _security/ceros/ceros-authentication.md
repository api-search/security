---
api_key_in: []
api_specs:
- filename: ceros-accounts-api-openapi.yml
  format: yaml
  label: Ceros Accounts API
  slug: ceros-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-accounts-api-openapi.yml
- filename: ceros-embedcodes-api-openapi.yml
  format: yaml
  label: Ceros Embed Codes API
  slug: ceros-embedcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-embedcodes-api-openapi.yml
- filename: ceros-experience-api-openapi.yml
  format: yaml
  label: Ceros Experience API
  slug: ceros-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-experience-api-openapi.yml
- filename: ceros-experiencepage-api-openapi.yml
  format: yaml
  label: Ceros Experience Page API
  slug: ceros-experiencepage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-experiencepage-api-openapi.yml
- filename: ceros-folders-api-openapi.yml
  format: yaml
  label: Ceros Folders API
  slug: ceros-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-folders-api-openapi.yml
- filename: ceros-oembed-api-openapi.yml
  format: yaml
  label: Ceros Oembed API
  slug: ceros-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-oembed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ceros Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ceros secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ceros
provider_slug: ceros
scheme_count: 1
schemes:
- bearerFormat: API_KEY
  description: API Key authentication using Bearer token format
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ceros-public-api-2026-02-25-openapi.yml
  - openapi/ceros-public-api-openapi.yml
  type: http
slug: ceros-authentication
source_filename: ceros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/ceros-public-api-2026-02-25-openapi.yml, openapi/ceros-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API_KEY\n  description: API Key authentication using Bearer token format\n  sources:\n  - openapi/ceros-public-api-2026-02-25-openapi.yml\n  - openapi/ceros-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/authentication/ceros-authentication.yml
summary_line: http · 1 scheme
tags:
- Content Management
- Interactive Content
- Digital Experience
- Embed
- oEmbed
- CMS Integration
- Marketing
- Design
- No-Code
- Content Delivery
- Media and Publishing
- SDK
---
