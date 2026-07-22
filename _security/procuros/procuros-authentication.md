---
api_key_in: []
api_specs:
- filename: procuros-openapi-original.yml
  format: yaml
  label: Procuros API v2
  slug: procuros-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procuros/refs/heads/main/openapi/procuros-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Procuros Authentication
name_suffix: Authentication
oauth_flows: []
overview: Procuros secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Procuros
provider_slug: procuros
scheme_count: 1
schemes:
- description: The API Token of your ERP Connection.
  name: api_token
  scheme: bearer
  sources:
  - openapi/procuros-openapi-original.yml
  type: http
slug: procuros-authentication
source_filename: procuros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/procuros-openapi-original.yml\ndocs: https://docs.procuros.io/en/api/v2/concept-authentication\nnotes: >-\n  The Procuros API v2 authenticates every request with a static API token passed as an HTTP\n  Bearer token (`Authorization: Bearer <token>`). Tokens are issued per ERP Connection and\n  requested from Procuros support (no self-service key management or OAuth flow). All requests\n  must be over HTTPS; unauthenticated calls fail with 401. Separate tokens exist for the Staging\n  and Production environments. Test connectivity with `GET /v2/ping`.\nsummary:\n  types:\n  - http\nschemes:\n- name: api_token\n  type: http\n  scheme: bearer\n  description: The API Token of your ERP Connection.\n  sources:\n  - openapi/procuros-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procuros/refs/heads/main/authentication/procuros-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SaaS
- EDI
- E-Invoicing
- Supply Chain
- Procurement
- B2B Integration
- Logistics
- ERP Integration
---
