---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comunicate-top-api-articles-api-openapi.yml
  format: yaml
  label: Comunicate.top API Articles API
  slug: comunicate-top-api-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-articles-api-openapi.yml
- filename: comunicate-top-api-balance-and-reports-api-openapi.yml
  format: yaml
  label: Comunicate.top API Balance and reports API
  slug: comunicate-top-api-balance-and-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-balance-and-reports-api-openapi.yml
- filename: comunicate-top-api-campaigns-api-openapi.yml
  format: yaml
  label: Comunicate.top API Campaigns API
  slug: comunicate-top-api-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-campaigns-api-openapi.yml
- filename: comunicate-top-api-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.top API Catalogue API
  slug: comunicate-top-api-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-catalogue-api-openapi.yml
- filename: comunicate-top-api-checks-api-openapi.yml
  format: yaml
  label: Comunicate.top API Checks API
  slug: comunicate-top-api-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-checks-api-openapi.yml
- filename: comunicate-top-api-domain-audit-api-openapi.yml
  format: yaml
  label: Comunicate.top API Domain audit API
  slug: comunicate-top-api-domain-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-domain-audit-api-openapi.yml
- filename: comunicate-top-api-key-and-permissions-api-openapi.yml
  format: yaml
  label: Comunicate.top API Key and permissions API
  slug: comunicate-top-api-key-and-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-key-and-permissions-api-openapi.yml
- filename: comunicate-top-api-media-api-openapi.yml
  format: yaml
  label: Comunicate.top API Media API
  slug: comunicate-top-api-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-media-api-openapi.yml
- filename: comunicate-top-api-public-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.top API Public catalogue API
  slug: comunicate-top-api-public-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-public-catalogue-api-openapi.yml
- filename: comunicate-top-api-publications-api-openapi.yml
  format: yaml
  label: Comunicate.top API Publications API
  slug: comunicate-top-api-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-publications-api-openapi.yml
- filename: comunicate-top-api-writing-orders-api-openapi.yml
  format: yaml
  label: Comunicate.top API Writing orders API
  slug: comunicate-top-api-writing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-writing-orders-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Comunicate Top Api Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Comunicate.top API secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Comunicate.top API
provider_slug: comunicate-top-api
scheme_count: 2
schemes:
- description: API key from Integrations (bk_live_…)
  name: apiKey
  scheme: bearer
  sources:
  - openapi/comunicate-top-api-openapi-original.json
  type: http
- description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.top/api/v1/oauth/register. The access token is an API key and is accepted everywhere an API key is.
  flows:
  - authorizationUrl: https://app.comunicate.top/api/v1/oauth/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://app.comunicate.top/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/comunicate-top-api-openapi-original.json
  type: oauth2
slug: comunicate-top-api-authentication
source_filename: comunicate-top-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: derived\nsource: openapi/comunicate-top-api-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from Integrations (bk_live_…)\n  sources:\n  - openapi/comunicate-top-api-openapi-original.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.comunicate.top/api/v1/oauth/authorize\n    tokenUrl: https://app.comunicate.top/api/v1/oauth/token\n    scopes: 10\n  description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.top/api/v1/oauth/register.\n    The access token is an API key and is accepted everywhere an API key is.\n  sources:\n  - openapi/comunicate-top-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/authentication/comunicate-top-api-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Press Releases
- Advertorials
- PR
- Publishing
- Media
- SEO
- Link Building
- Content Marketing
- Romania
- MCP
- Open Data
- Webhook
- Authentication
---
