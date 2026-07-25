---
api_key_in: []
api_specs:
- filename: hooklogic-criteo-accounts-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Accounts API
  slug: hooklogic-criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-accounts-api-openapi.yml
- filename: hooklogic-criteo-analytics-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Analytics API
  slug: hooklogic-criteo-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-analytics-api-openapi.yml
- filename: hooklogic-criteo-audience-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Audience API
  slug: hooklogic-criteo-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-audience-api-openapi.yml
- filename: hooklogic-criteo-balance-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Balance API
  slug: hooklogic-criteo-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-balance-api-openapi.yml
- filename: hooklogic-criteo-billing-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Billing API
  slug: hooklogic-criteo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-billing-api-openapi.yml
- filename: hooklogic-criteo-campaign-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Campaign API
  slug: hooklogic-criteo-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-campaign-api-openapi.yml
- filename: hooklogic-criteo-catalog-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Catalog API
  slug: hooklogic-criteo-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-catalog-api-openapi.yml
- filename: hooklogic-criteo-gateway-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Gateway API
  slug: hooklogic-criteo-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-gateway-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hooklogic Criteo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: HookLogic (Criteo) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: HookLogic (Criteo)
provider_slug: hooklogic-criteo
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  sources:
  - openapi/hooklogic-criteo-retailmedia-openapi-original.json
  type: oauth2
slug: hooklogic-criteo-authentication
source_filename: hooklogic-criteo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hooklogic-criteo-retailmedia-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/hooklogic-criteo-retailmedia-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/authentication/hooklogic-criteo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Commerce
- Retail Media
- Advertising
- E-commerce
- Marketing
- Retail
- APIs
---
