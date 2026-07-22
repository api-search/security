---
api_key_in: []
api_specs:
- filename: stubhub-account-openapi.yml
  format: yaml
  label: StubHub Account API
  slug: stubhub-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-account-openapi.yml
- filename: stubhub-catalog-openapi.yml
  format: yaml
  label: StubHub Catalog API
  slug: stubhub-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-catalog-openapi.yml
- filename: stubhub-inventory-openapi.yml
  format: yaml
  label: StubHub Inventory API
  slug: stubhub-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-inventory-openapi.yml
- filename: stubhub-sales-openapi.yml
  format: yaml
  label: StubHub Sales API
  slug: stubhub-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-sales-openapi.yml
- filename: stubhub-webhooks-openapi.yml
  format: yaml
  label: StubHub Webhooks API
  slug: stubhub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-webhooks-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Stubhub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: StubHub secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: StubHub
provider_slug: stubhub
scheme_count: 1
schemes:
- description: OAuth2. All API requests must be authenticated.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://account.stubhub.com/oauth2/token
  - authorizationUrl: https://account.stubhub.com/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://account.stubhub.com/oauth2/token
  name: oauth2
  sources:
  - openapi/stubhub-account-openapi.yml
  - openapi/stubhub-catalog-openapi.yml
  - openapi/stubhub-inventory-openapi.yml
  - openapi/stubhub-sales-openapi.yml
  - openapi/stubhub-webhooks-openapi.yml
  type: oauth2
slug: stubhub-authentication
source_filename: stubhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/stubhub-account-openapi.yml, openapi/stubhub-catalog-openapi.yml, openapi/stubhub-inventory-openapi.yml,\n  openapi/stubhub-sales-openapi.yml, openapi/stubhub-webhooks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.stubhub.com/oauth2/token\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://account.stubhub.com/authorize\n    tokenUrl: https://account.stubhub.com/oauth2/token\n    scopes: 9\n  description: OAuth2. All API requests must be authenticated.\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/authentication/stubhub-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketplaces
- Tickets
- Events
- Ticketing
- Live Events
- Secondary Market
- E-commerce
- Sports
- Concerts
---
