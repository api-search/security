---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meuecommerce-com-br-rates-api-openapi.yml
  format: yaml
  label: Meu Ecommerce Rates API
  slug: meuecommerce-com-br-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meuecommerce-com-br/openapi/meuecommerce-com-br-rates-api-openapi.yml
- filename: meuecommerce-com-br-tracking-api-openapi.yml
  format: yaml
  label: Meu Ecommerce Tracking API
  slug: meuecommerce-com-br-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meuecommerce-com-br/openapi/meuecommerce-com-br-tracking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Meu Ecommerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meu Ecommerce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meu Ecommerce
provider_slug: meuecommerce-com-br
scheme_count: 1
schemes:
- description: Chave pública pk_... (quote-only).
  name: PublicKey
  scheme: bearer
  sources:
  - openapi/meuecommerce-com-br-dev-openapi.json
  - openapi/meuecommerce-com-br-openapi.json
  type: http
slug: meuecommerce-com-br-authentication
source_filename: meuecommerce-com-br-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meuecommerce-com-br-dev-openapi.json, openapi/meuecommerce-com-br-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: PublicKey\n  type: http\n  scheme: bearer\n  description: Chave pública pk_... (quote-only).\n  sources:\n  - openapi/meuecommerce-com-br-dev-openapi.json\n  - openapi/meuecommerce-com-br-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/meuecommerce-com-br/authentication/meuecommerce-com-br-authentication.yml
summary_line: http · 1 scheme
tags:
- Shipping
- Tracking
- Installments
- E‑commerce Apps
- AI Integration
---
