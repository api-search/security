---
api_key_in: []
api_specs:
- filename: tango-card-accounts-api-openapi.yml
  format: yaml
  label: Tango Card Accounts API
  slug: tango-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-accounts-api-openapi.yml
- filename: tango-card-brand-categories-api-openapi.yml
  format: yaml
  label: Tango Card Brand Categories API
  slug: tango-card-brand-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-brand-categories-api-openapi.yml
- filename: tango-card-catalog-api-openapi.yml
  format: yaml
  label: Tango Card Catalog API
  slug: tango-card-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-catalog-api-openapi.yml
- filename: tango-card-choice-products-api-openapi.yml
  format: yaml
  label: Tango Card Choice Products API
  slug: tango-card-choice-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-choice-products-api-openapi.yml
- filename: tango-card-countries-currencies-api-openapi.yml
  format: yaml
  label: Tango Card Countries & Currencies API
  slug: tango-card-countries-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-countries-currencies-api-openapi.yml
- filename: tango-card-credential-types-api-openapi.yml
  format: yaml
  label: Tango Card Credential Types API
  slug: tango-card-credential-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-credential-types-api-openapi.yml
- filename: tango-card-customers-api-openapi.yml
  format: yaml
  label: Tango Card Customers API
  slug: tango-card-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-customers-api-openapi.yml
- filename: tango-card-digital-templates-api-openapi.yml
  format: yaml
  label: Tango Card Digital Templates API
  slug: tango-card-digital-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-digital-templates-api-openapi.yml
- filename: tango-card-exchange-rates-api-openapi.yml
  format: yaml
  label: Tango Card Exchange Rates API
  slug: tango-card-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-exchange-rates-api-openapi.yml
- filename: tango-card-fund-management-api-openapi.yml
  format: yaml
  label: Tango Card Fund Management API
  slug: tango-card-fund-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-fund-management-api-openapi.yml
- filename: tango-card-line-items-api-openapi.yml
  format: yaml
  label: Tango Card Line Items API
  slug: tango-card-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-line-items-api-openapi.yml
- filename: tango-card-low-balance-alerts-api-openapi.yml
  format: yaml
  label: Tango Card Low Balance Alerts API
  slug: tango-card-low-balance-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-low-balance-alerts-api-openapi.yml
- filename: tango-card-orders-api-openapi.yml
  format: yaml
  label: Tango Card Orders API
  slug: tango-card-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-orders-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tango Card Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tango Card secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tango Card
provider_slug: tango-card
scheme_count: 2
schemes:
- description: HTTP Basic Auth using platform name and API key
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tango-raas-api-openapi.yml
  type: http
- description: OAuth 2.0 client credentials flow for more secure integrations
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.tangocard.com/oauth/token
  name: oAuth2
  sources:
  - openapi/tango-raas-api-openapi.yml
  type: oauth2
slug: tango-card-authentication
source_filename: tango-card-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tango-raas-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using platform name and API key\n  sources:\n  - openapi/tango-raas-api-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tangocard.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials flow for more secure integrations\n  sources:\n  - openapi/tango-raas-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/authentication/tango-card-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Gift Cards
- Rewards
- Incentives
- Digital Rewards
- Prepaid Cards
- Payments
---
