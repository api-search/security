---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comunicate-eu-public-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.eu Public catalogue API
  slug: comunicate-eu-public-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-public-catalogue-api-openapi.yml
- filename: comunicate-eu-publications-api-openapi.yml
  format: yaml
  label: Comunicate.eu Publications API
  slug: comunicate-eu-publications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-publications-api-openapi.yml
- filename: comunicate-eu-writing-orders-api-openapi.yml
  format: yaml
  label: Comunicate.eu Writing orders API
  slug: comunicate-eu-writing-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-writing-orders-api-openapi.yml
- filename: comunicate-eu-articles-api-openapi.yml
  format: yaml
  label: Comunicate.eu Articles API
  slug: comunicate-eu-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-articles-api-openapi.yml
- filename: comunicate-eu-balance-and-reports-api-openapi.yml
  format: yaml
  label: Comunicate.eu Balance and reports API
  slug: comunicate-eu-balance-and-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-balance-and-reports-api-openapi.yml
- filename: comunicate-eu-campaigns-api-openapi.yml
  format: yaml
  label: Comunicate.eu Campaigns API
  slug: comunicate-eu-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-campaigns-api-openapi.yml
- filename: comunicate-eu-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.eu Catalogue API
  slug: comunicate-eu-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-catalogue-api-openapi.yml
- filename: comunicate-eu-checks-api-openapi.yml
  format: yaml
  label: Comunicate.eu Checks API
  slug: comunicate-eu-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-checks-api-openapi.yml
- filename: comunicate-eu-domain-audit-api-openapi.yml
  format: yaml
  label: Comunicate.eu Domain audit API
  slug: comunicate-eu-domain-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-domain-audit-api-openapi.yml
- filename: comunicate-eu-key-and-permissions-api-openapi.yml
  format: yaml
  label: Comunicate.eu Key and permissions API
  slug: comunicate-eu-key-and-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-key-and-permissions-api-openapi.yml
- filename: comunicate-eu-media-api-openapi.yml
  format: yaml
  label: Comunicate.eu Media API
  slug: comunicate-eu-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-media-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Comunicate.eu Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Comunicate.eu secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Comunicate.eu
provider_slug: comunicate-eu
scheme_count: 2
schemes:
- description: API key from Integrations (bk_live_…)
  name: apiKey
  scheme: bearer
  sources:
  - openapi/comunicate-eu-openapi.yml
  type: http
- description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.eu/api/v1/oauth/register. The access token is an API key and is accepted everywhere an API key is.
  flows:
  - authorizationUrl: https://app.comunicate.eu/api/v1/oauth/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://app.comunicate.eu/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/comunicate-eu-openapi.yml
  type: oauth2
slug: comunicate-eu-authentication
source_filename: comunicate-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comunicate.eu/ro/documentatie-api\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from Integrations (bk_live_…)\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.comunicate.eu/api/v1/oauth/authorize\n    tokenUrl: https://app.comunicate.eu/api/v1/oauth/token\n    scopes: 10\n  description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.eu/api/v1/oauth/register.\n    The access token is an API key and is accepted everywhere an API key is.\n  sources:\n  - openapi/comunicate-eu-openapi.yml\ndocs: https://comunicate.eu/ro/documentatie-api\nheader: 'Authorization: Bearer bk_live_…'\nkey_prefix: bk_live_\nkey_issuance: Keys are issued from the Integrations page and shown\
  \ once; the provider\n  stores only a hash (\"se vede o singură dată — noi păstrăm doar amprenta ei, exact\n  ca la parole\").\nunauthenticated_routes: '/public/* routes need no key; in openapi.json they carry\n  security: [] and the document has no global security.'\ntest_keys: 'None documented: only the bk_live_ prefix appears in the docs.'\noauth_docs_note: OAuth 2.1 + PKCE and dynamic client registration are stated in the\n  OpenAPI securitySchemes description; the HTML docs page describes only API-key auth.\nidentity_endpoint: GET /partner/me (operationId get_me) returns the organization,\n  the key scopes and the aiPublishing toggle; requires no scope.\n"
source_yaml_url: https://artifacts.apis.io/comunicate-eu/authentication/comunicate-eu-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Press Releases
- Advertorials
- Content Marketing
- SEO
- Publishing
- Media Marketplace
- Romania
- MCP
- PR
- Media
- Link Building
- Open Data
- Webhook
- Authentication
---
