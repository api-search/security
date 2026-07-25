---
api_key_in: []
api_specs:
- filename: snov-authentication-api-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-authentication-api-openapi.yml
- filename: snov-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snov-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-campaigns-api-openapi.yml
- filename: snov-domain-search-api-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-domain-search-api-openapi.yml
- filename: snov-email-finder-api-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-email-finder-api-openapi.yml
- filename: snov-email-verifier-api-openapi.yml
  format: yaml
  label: Snov.io Email Verifier API
  slug: snov-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-email-verifier-api-openapi.yml
- filename: snov-enrichment-api-openapi.yml
  format: yaml
  label: Snov.io Enrichment API
  slug: snov-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-enrichment-api-openapi.yml
- filename: snov-prospects-api-openapi.yml
  format: yaml
  label: Snov.io Prospects API
  slug: snov-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-prospects-api-openapi.yml
- filename: snov-sender-accounts-api-openapi.yml
  format: yaml
  label: Snov.io Sender Accounts API
  slug: snov-sender-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-sender-accounts-api-openapi.yml
- filename: snov-user-api-openapi.yml
  format: yaml
  label: Snov.io User API
  slug: snov-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-user-api-openapi.yml
- filename: snov-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Warm-up API
  slug: snov-warm-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-warm-up-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Snov Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Snov.io secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Snov.io
provider_slug: snov
scheme_count: 1
schemes:
- description: OAuth2 client_credentials flow. POST client_id and client_secret to /v1/oauth/access_token to obtain a Bearer token, then send it in the Authorization header.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.snov.io/v1/oauth/access_token
  name: OAuth2
  sources:
  - openapi/snov-openapi.yml
  type: oauth2
slug: snov-authentication
source_filename: snov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snov-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.snov.io/v1/oauth/access_token\n    scopes: 0\n  description: OAuth2 client_credentials flow. POST client_id and client_secret to /v1/oauth/access_token\n    to obtain a Bearer token, then send it in the Authorization header.\n  sources:\n  - openapi/snov-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/authentication/snov-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Sales Engagement
- Email Finder
- Email Verification
- Prospecting
- Drip Campaigns
- CRM
- Lead Generation
---
