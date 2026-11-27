---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuance-labs-browser-api-openapi.yml
  format: yaml
  label: Nuance Labs Browser API
  slug: nuance-labs-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance-labs/openapi/nuance-labs-browser-api-openapi.yml
- filename: nuance-labs-server-api-openapi.yml
  format: yaml
  label: Nuance Labs Server API
  slug: nuance-labs-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance-labs/openapi/nuance-labs-server-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nuance Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuance Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nuance Labs
provider_slug: nuance-labs
scheme_count: 1
schemes:
- description: An API key from your organization's API keys page on the platform, `nk_…`. Server only.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/nuance-labs-openapi.yml
  type: http
slug: nuance-labs-authentication
source_filename: nuance-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/nuance-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: An API key from your organization's API keys page on the platform, `nk_…`. Server\n    only.\n  sources:\n  - openapi/nuance-labs-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/nuance-labs/authentication/nuance-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Foundation Models
- Emotional Intelligence
- Conversational AI
- Multi-Modal
- Real-Time
- Seattle
---
