---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kovatools-com-authentication-api-openapi.yml
  format: yaml
  label: Kova Authentication API
  slug: kovatools-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-authentication-api-openapi.yml
- filename: kovatools-com-briefs-api-openapi.yml
  format: yaml
  label: Kova Briefs API
  slug: kovatools-com-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-briefs-api-openapi.yml
- filename: kovatools-com-journal-api-openapi.yml
  format: yaml
  label: Kova Journal API
  slug: kovatools-com-journal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-journal-api-openapi.yml
- filename: kovatools-com-portfolio-api-openapi.yml
  format: yaml
  label: Kova Portfolio API
  slug: kovatools-com-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-portfolio-api-openapi.yml
- filename: kovatools-com-simulations-api-openapi.yml
  format: yaml
  label: Kova Simulations API
  slug: kovatools-com-simulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-simulations-api-openapi.yml
- filename: kovatools-com-strategies-api-openapi.yml
  format: yaml
  label: Kova Strategies API
  slug: kovatools-com-strategies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-strategies-api-openapi.yml
- filename: kovatools-com-strategy-intelligence-api-openapi.yml
  format: yaml
  label: Kova Strategy Intelligence API
  slug: kovatools-com-strategy-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-strategy-intelligence-api-openapi.yml
- filename: kovatools-com-versions-api-openapi.yml
  format: yaml
  label: Kova Versions API
  slug: kovatools-com-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kovatools-com/openapi/kovatools-com-versions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kova Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kova secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kova
provider_slug: kovatools-com
scheme_count: 1
schemes:
- description: 'API token prefixed with `kova_tk_`. Example: `Bearer kova_tk_a3f2b1c4d5e6f7a8b9c0d1e2f3a4b5c6`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kovatools-com-openapi.yml
  - openapi/openapi.yaml
  type: http
slug: kovatools-com-authentication
source_filename: kovatools-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/kovatools-com-openapi.yml, openapi/openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token prefixed with `kova_tk_`. Example: `Bearer kova_tk_a3f2b1c4d5e6f7a8b9c0d1e2f3a4b5c6`'\n  sources:\n  - openapi/kovatools-com-openapi.yml\n  - openapi/openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/kovatools-com/authentication/kovatools-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Investment
- Portfolio
- Alignment
- Software-as-a-Service
- Artificial Intelligence
---
