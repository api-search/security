---
api_key_in: []
api_specs:
- filename: horizoniq-compass-openapi-original.yml
  format: yaml
  label: HorizonIQ Compass API
  slug: horizoniq-compass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-compass-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Horizoniq Authentication
name_suffix: Authentication
oauth_flows: []
overview: HorizonIQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HorizonIQ
provider_slug: horizoniq
scheme_count: 1
schemes:
- description: 'API token issued from the Compass portal (Profile > API Tokens). Sent as `Authorization: Bearer <token>`. See https://compass-horizoniq.readme.io/reference/authentication'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/horizoniq-compass-openapi-original.yml
  type: http
slug: horizoniq-authentication
source_filename: horizoniq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/horizoniq-compass-openapi-original.yml + docs\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token issued from the Compass portal (Profile > API Tokens). Sent as `Authorization:\n    Bearer <token>`. See https://compass-horizoniq.readme.io/reference/authentication'\n  sources:\n  - openapi/horizoniq-compass-openapi-original.yml\ndocs: https://compass-horizoniq.readme.io/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/authentication/horizoniq-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Cloud
- Bare Metal
- Infrastructure
- Private Cloud
- Hosting
- Data Center
- Compute
- Storage
---
