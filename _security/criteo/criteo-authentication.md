---
api_key_in: []
api_specs:
- filename: criteo-accounts-api-openapi.yml
  format: yaml
  label: Criteo Accounts API
  slug: criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-accounts-api-openapi.yml
- filename: criteo-audiences-api-openapi.yml
  format: yaml
  label: Criteo Audiences API
  slug: criteo-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-audiences-api-openapi.yml
- filename: criteo-authentication-api-openapi.yml
  format: yaml
  label: Criteo Authentication API
  slug: criteo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-authentication-api-openapi.yml
- filename: criteo-balances-api-openapi.yml
  format: yaml
  label: Criteo Balances API
  slug: criteo-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-balances-api-openapi.yml
- filename: criteo-campaigns-api-openapi.yml
  format: yaml
  label: Criteo Campaigns API
  slug: criteo-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-campaigns-api-openapi.yml
- filename: criteo-catalogs-api-openapi.yml
  format: yaml
  label: Criteo Catalogs API
  slug: criteo-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-catalogs-api-openapi.yml
- filename: criteo-categories-api-openapi.yml
  format: yaml
  label: Criteo Categories API
  slug: criteo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-categories-api-openapi.yml
- filename: criteo-keywords-api-openapi.yml
  format: yaml
  label: Criteo Keywords API
  slug: criteo-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-keywords-api-openapi.yml
- filename: criteo-lineitems-api-openapi.yml
  format: yaml
  label: Criteo LineItems API
  slug: criteo-lineitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-lineitems-api-openapi.yml
- filename: criteo-products-api-openapi.yml
  format: yaml
  label: Criteo Products API
  slug: criteo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-products-api-openapi.yml
- filename: criteo-reports-api-openapi.yml
  format: yaml
  label: Criteo Reports API
  slug: criteo-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-reports-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Criteo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Criteo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Criteo
provider_slug: criteo
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://consent.criteo.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.criteo.com/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/criteo-openapi.yml
  type: oauth2
slug: criteo-authentication
source_filename: criteo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/criteo-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://consent.criteo.com/authorize\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/criteo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/authentication/criteo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Audiences
- Campaigns
- Catalog
- Commerce
- Display Advertising
- Marketing
- Media
- OAuth 2.0
- Reporting
- Retail
- Retail Media
---
