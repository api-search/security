---
api_key_in: []
api_specs:
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Projects API
  slug: aurora-solar-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Designs API
  slug: aurora-solar-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Proposals API
  slug: aurora-solar-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Consumption Profiles API
  slug: aurora-solar-consumption-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Users & Tenants API
  slug: aurora-solar-users-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Webhooks API
  slug: aurora-solar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Financings API
  slug: aurora-solar-financings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Agreements API
  slug: aurora-solar-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aurora Solar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aurora Solar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aurora Solar
provider_slug: aurora-solar
scheme_count: 1
schemes:
- description: 'API-key bearer token. Standard keys are prefixed `sk_`, Restricted keys `rk_`; `sand_`/`prod_` denote sandbox vs production. Passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aurora-solar-openapi.yml
  type: http
slug: aurora-solar-authentication
source_filename: aurora-solar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aurora-solar-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API-key bearer token. Standard keys are prefixed `sk_`, Restricted keys `rk_`;\n    `sand_`/`prod_` denote sandbox vs production. Passed as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/aurora-solar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/authentication/aurora-solar-authentication.yml
summary_line: http · 1 scheme
tags:
- Solar
- Solar Design
- PV
- Proposals
- CleanTech
- Energy
- Sales Software
---
