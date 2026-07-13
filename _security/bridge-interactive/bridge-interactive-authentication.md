---
api_key_in: []
api_specs:
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Listings and Properties API
  slug: listings-properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Agents API
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Offices API
  slug: offices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Open Houses API
  slug: open-houses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
- filename: bridge-interactive-openapi.yml
  format: yaml
  label: Bridge RESO Web API
  slug: reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/openapi/bridge-interactive-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bridge Interactive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bridge Interactive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bridge Interactive
provider_slug: bridge-interactive
scheme_count: 1
schemes:
- description: 'Server access token issued from the Bridge Dashboard under Data Access > API Access Tokens. Sent as "Authorization: Bearer <token>" or as an access_token query parameter.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bridge-interactive-openapi.yml
  type: http
slug: bridge-interactive-authentication
source_filename: bridge-interactive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bridge-interactive-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Server access token issued from the Bridge Dashboard under Data Access > API\n    Access Tokens. Sent as \"Authorization: Bearer <token>\" or as an access_token query parameter.'\n  sources:\n  - openapi/bridge-interactive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge-interactive/refs/heads/main/authentication/bridge-interactive-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- MLS
- RESO
- Listings
- Property Data
---
