---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contrie-com-account-api-openapi.yml
  format: yaml
  label: Contrie Account API
  slug: contrie-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-account-api-openapi.yml
- filename: contrie-com-evidence-api-openapi.yml
  format: yaml
  label: Contrie Evidence API
  slug: contrie-com-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-evidence-api-openapi.yml
- filename: contrie-com-extract-api-openapi.yml
  format: yaml
  label: Contrie Extract API
  slug: contrie-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-extract-api-openapi.yml
- filename: contrie-com-health-api-openapi.yml
  format: yaml
  label: Contrie Health API
  slug: contrie-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-health-api-openapi.yml
- filename: contrie-com-mcp-api-openapi.yml
  format: yaml
  label: Contrie MCP API
  slug: contrie-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-mcp-api-openapi.yml
- filename: contrie-com-monitors-api-openapi.yml
  format: yaml
  label: Contrie Monitors API
  slug: contrie-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-monitors-api-openapi.yml
- filename: contrie-com-scrape-api-openapi.yml
  format: yaml
  label: Contrie Scrape API
  slug: contrie-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-scrape-api-openapi.yml
- filename: contrie-com-search-api-openapi.yml
  format: yaml
  label: Contrie Search API
  slug: contrie-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-search-api-openapi.yml
- filename: contrie-com-verification-api-openapi.yml
  format: yaml
  label: Contrie Verification API
  slug: contrie-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-verification-api-openapi.yml
- filename: contrie-com-verify-api-openapi.yml
  format: yaml
  label: Contrie Verify API
  slug: contrie-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-verify-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Contrie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contrie secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Contrie
provider_slug: contrie-com
scheme_count: 2
schemes:
- bearerFormat: Contrie API key or resource-bound OAuth access JWT
  description: API key created at https://www.contrie.com/dashboard/keys (human sign-up in a browser; there is no programmatic key issuance), or an OAuth access token from the advertised Contrie sign-in flow. OAuth needs no additional API key.
  header: 'Authorization: Bearer ck_live_...'
  key_format:
    length: 40 characters
    note: Contrie currently issues only ck_live_ keys. The prefix does not select a testing environment or Stripe billing mode.
    prefix: ck_live_
  key_management: You can create up to 20 keys, name them, and delete them from the API Keys page in your dashboard. Keys are hashed on our servers.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/contrie-com-openapi.yml
  - https://www.contrie.com/docs/authentication
  type: http
- audience: https://www.contrie.com/mcp
  description: The hosted MCP server at https://www.contrie.com/mcp supports browser sign-in (OAuth). The OAuth boundary accepts only Clerk-issued JWTs for the configured issuer and the audience https://www.contrie.com/mcp, with the explicit contrie:account permission. Opaque OAuth tokens are unsupported. JWTs are checked for signature and expiry; immediate revocation of an issued JWT is not guaranteed. Not declared as a securityScheme in the OpenAPI; documented only.
  issuer: Clerk
  name: mcpOAuth
  scopes:
  - contrie:account
  - offline_access
  sources:
  - https://www.contrie.com/docs/authentication
  - https://www.contrie.com/docs/mcp
  type: oauth2
slug: contrie-com-authentication
source_filename: contrie-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.contrie.com/docs/authentication\ndocs: https://www.contrie.com/docs/authentication\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Contrie API key or resource-bound OAuth access JWT\n  description: API key created at https://www.contrie.com/dashboard/keys (human sign-up in a\n    browser; there is no programmatic key issuance), or an OAuth access token from the advertised\n    Contrie sign-in flow. OAuth needs no additional API key.\n  header: 'Authorization: Bearer ck_live_...'\n  key_format:\n    prefix: ck_live_\n    length: 40 characters\n    note: Contrie currently issues only ck_live_ keys. The prefix does not select a testing environment or Stripe billing mode.\n  key_management: You can create up to 20 keys, name them, and delete them from the API Keys page in your dashboard. Keys are hashed on our servers.\n  sources:\n  - openapi/contrie-com-openapi.yml\n\
  \  - https://www.contrie.com/docs/authentication\n- name: mcpOAuth\n  type: oauth2\n  description: The hosted MCP server at https://www.contrie.com/mcp supports browser sign-in (OAuth). The OAuth boundary accepts only Clerk-issued JWTs for the configured issuer and the audience https://www.contrie.com/mcp, with the explicit contrie:account permission. Opaque OAuth tokens are unsupported. JWTs are checked for signature and expiry; immediate revocation of an issued JWT is not guaranteed. Not declared as a securityScheme in the OpenAPI; documented only.\n  audience: https://www.contrie.com/mcp\n  issuer: Clerk\n  scopes:\n  - contrie:account\n  - offline_access\n  sources:\n  - https://www.contrie.com/docs/authentication\n  - https://www.contrie.com/docs/mcp\nkeyless_access: Exact recorded sample requests listed in /llms.txt need no credential.\nfailed_auth_limit: About 20 failed authentication attempts a minute from one client return RATE_LIMITED (429) with Retry-After 60 instead of 401.\n"
source_yaml_url: https://artifacts.apis.io/contrie-com/authentication/contrie-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Web Scraping
- Data Extraction
- AI Agents
- MCP
- Structured Data
- Markdown
---
