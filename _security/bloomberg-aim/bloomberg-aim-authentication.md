---
api_key_in: []
api_specs:
- filename: bloomberg-aim-broker-strategies-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Broker Strategies API
  slug: bloomberg-aim-broker-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-broker-strategies-api-openapi.yml
- filename: bloomberg-aim-catalogs-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Catalogs API
  slug: bloomberg-aim-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-catalogs-api-openapi.yml
- filename: bloomberg-aim-distributions-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Distributions API
  slug: bloomberg-aim-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-distributions-api-openapi.yml
- filename: bloomberg-aim-field-lists-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Field Lists API
  slug: bloomberg-aim-field-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-field-lists-api-openapi.yml
- filename: bloomberg-aim-field-search-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Field Search API
  slug: bloomberg-aim-field-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-field-search-api-openapi.yml
- filename: bloomberg-aim-fills-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Fills API
  slug: bloomberg-aim-fills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-fills-api-openapi.yml
- filename: bloomberg-aim-historical-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Historical Data API
  slug: bloomberg-aim-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-historical-data-api-openapi.yml
- filename: bloomberg-aim-instruments-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Instruments API
  slug: bloomberg-aim-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-instruments-api-openapi.yml
- filename: bloomberg-aim-intraday-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Intraday Data API
  slug: bloomberg-aim-intraday-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-intraday-data-api-openapi.yml
- filename: bloomberg-aim-orders-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Orders API
  slug: bloomberg-aim-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-orders-api-openapi.yml
- filename: bloomberg-aim-reference-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Reference Data API
  slug: bloomberg-aim-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-reference-data-api-openapi.yml
- filename: bloomberg-aim-replies-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Replies API
  slug: bloomberg-aim-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-replies-api-openapi.yml
- filename: bloomberg-aim-requests-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Requests API
  slug: bloomberg-aim-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-requests-api-openapi.yml
- filename: bloomberg-aim-routes-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Routes API
  slug: bloomberg-aim-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-routes-api-openapi.yml
- filename: bloomberg-aim-teams-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Teams API
  slug: bloomberg-aim-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-teams-api-openapi.yml
- filename: bloomberg-aim-triggers-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Triggers API
  slug: bloomberg-aim-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-triggers-api-openapi.yml
- filename: bloomberg-aim-universes-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Universes API
  slug: bloomberg-aim-universes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-universes-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bloomberg Aim Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bloomberg AIM secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Bloomberg-issued JWT credential obtained from the Bloomberg Console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bloomberg-data-license-api.yml
  - openapi/bloomberg-emsx-api.yml
  type: http
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2
  name: oauth2
  sources:
  - openapi/bloomberg-data-license-api.yml
  type: oauth2
- description: HTTP Basic authentication for the local API server
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bloomberg-http-api.yml
  type: http
slug: bloomberg-aim-authentication
source_filename: bloomberg-aim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomberg-data-license-api.yml, openapi/bloomberg-emsx-api.yml, openapi/bloomberg-http-api.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bloomberg-issued JWT credential obtained from the Bloomberg Console.\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n  - openapi/bloomberg-emsx-api.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2\n    scopes: 3\n  description: OAuth 2.0 client credentials flow\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication for the local API server\n  sources:\n  - openapi/bloomberg-http-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/authentication/bloomberg-aim-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
---
