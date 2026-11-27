---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fahaliai-com-agent-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Agent API
  slug: fahaliai-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-agent-api-openapi.yml
- filename: fahaliai-com-alerts-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Alerts API
  slug: fahaliai-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-alerts-api-openapi.yml
- filename: fahaliai-com-billing-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Billing API
  slug: fahaliai-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-billing-api-openapi.yml
- filename: fahaliai-com-case-studies-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Case Studies API
  slug: fahaliai-com-case-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-case-studies-api-openapi.yml
- filename: fahaliai-com-engines-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Engines API
  slug: fahaliai-com-engines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-engines-api-openapi.yml
- filename: fahaliai-com-institutional-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Institutional API
  slug: fahaliai-com-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-institutional-api-openapi.yml
- filename: fahaliai-com-market-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Market API
  slug: fahaliai-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-market-api-openapi.yml
- filename: fahaliai-com-public-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Public API
  slug: fahaliai-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-public-api-openapi.yml
- filename: fahaliai-com-track-record-api-openapi.yml
  format: yaml
  label: Fahali Enterprise Track Record API
  slug: fahaliai-com-track-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fahaliai-com/openapi/fahaliai-com-track-record-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fahali Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fahali Enterprise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fahali Enterprise
provider_slug: fahaliai-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Firebase ID token (logged-in user) for billing and portfolio endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fahaliai-com-openapi.json
  type: http
slug: fahaliai-com-authentication
source_filename: fahaliai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fahaliai-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Firebase ID token (logged-in user) for billing and portfolio endpoints.\n  sources:\n  - openapi/fahaliai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fahaliai-com/authentication/fahaliai-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Risk Intelligence
- Family Offices
- Portfolio Management
- Market Data
---
