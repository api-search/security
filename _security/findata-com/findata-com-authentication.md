---
anonymous_access: false
api_key_in: []
api_specs:
- filename: findata-com-companies-api-openapi.yml
  format: yaml
  label: FinData Companies API
  slug: findata-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-companies-api-openapi.yml
- filename: findata-com-corporate-actions-api-openapi.yml
  format: yaml
  label: FinData Corporate actions API
  slug: findata-com-corporate-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-corporate-actions-api-openapi.yml
- filename: findata-com-fundamentals-api-openapi.yml
  format: yaml
  label: FinData Fundamentals API
  slug: findata-com-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-fundamentals-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: FinData Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FinData secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FinData
provider_slug: findata-com
scheme_count: 2
schemes:
- description: Authorization code with PKCE. Include resource=https://api.findata.com in both authorization and token requests.
  flows:
  - authorizationUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/token
  name: OAuth
  sources:
  - openapi/findata-com-openapi.json
  type: oauth2
- description: Legacy operator key, when configured.
  name: BearerKey
  scheme: bearer
  sources:
  - openapi/findata-com-openapi.json
  type: http
slug: findata-com-authentication
source_filename: findata-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/findata-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/authorize\n    tokenUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/token\n    scopes: 1\n  description: Authorization code with PKCE. Include resource=https://api.findata.com in both\n    authorization and token requests.\n  sources:\n  - openapi/findata-com-openapi.json\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: Legacy operator key, when configured.\n  sources:\n  - openapi/findata-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/findata-com/authentication/findata-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Financial Data
- SEC Fundamentals
- Market Data
- Research
---
