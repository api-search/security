---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inboxguard-io-account-api-openapi.yml
  format: yaml
  label: InboxGuard Account API
  slug: inboxguard-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-account-api-openapi.yml
- filename: inboxguard-io-alerts-api-openapi.yml
  format: yaml
  label: InboxGuard Alerts API
  slug: inboxguard-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-alerts-api-openapi.yml
- filename: inboxguard-io-domains-api-openapi.yml
  format: yaml
  label: InboxGuard Domains API
  slug: inboxguard-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-domains-api-openapi.yml
- filename: inboxguard-io-integrations-api-openapi.yml
  format: yaml
  label: InboxGuard Integrations API
  slug: inboxguard-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-integrations-api-openapi.yml
- filename: inboxguard-io-portfolio-api-openapi.yml
  format: yaml
  label: InboxGuard Portfolio API
  slug: inboxguard-io-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-portfolio-api-openapi.yml
- filename: inboxguard-io-reports-api-openapi.yml
  format: yaml
  label: InboxGuard Reports API
  slug: inboxguard-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-reports-api-openapi.yml
- filename: inboxguard-io-scanning-api-openapi.yml
  format: yaml
  label: InboxGuard Scanning API
  slug: inboxguard-io-scanning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-scanning-api-openapi.yml
- filename: inboxguard-io-system-api-openapi.yml
  format: yaml
  label: InboxGuard System API
  slug: inboxguard-io-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-system-api-openapi.yml
- filename: inboxguard-io-webhooks-api-openapi.yml
  format: yaml
  label: InboxGuard Webhooks API
  slug: inboxguard-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: InboxGuard Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: InboxGuard secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: InboxGuard
provider_slug: inboxguard-io
scheme_count: 2
schemes:
- bearerFormat: InboxGuard API key (ig_live_… / ig_test_…)
  description: 'PRIMARY auth: send an InboxGuard API key as a bearer token (`Authorization: Bearer ig_live_…`). Scopes: `read` (GET) and `full` (all methods). Mint a key at https://inboxguard.io/settings or per https://inboxguard.io/auth.md.'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/inboxguard-io-openapi.json
  type: http
- description: 'OAuth-shaped wrapper around the same API key. The ONLY grant is client_credentials at POST https://api.inboxguard.io/oauth/token, where the client_secret IS an InboxGuard API key (HTTP Basic or body); the returned access_token is that same key. There is NO authorization_code flow, NO PKCE, and NO /oauth/authorize endpoint. Discovery: /.well-known/oauth-authorization-server and /.well-known/oauth-p'
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.inboxguard.io/oauth/token
  name: OAuth2
  sources:
  - openapi/inboxguard-io-openapi.json
  type: oauth2
slug: inboxguard-io-authentication
source_filename: inboxguard-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/inboxguard-io-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: InboxGuard API key (ig_live_… / ig_test_…)\n  description: 'PRIMARY auth: send an InboxGuard API key as a bearer token (`Authorization:\n    Bearer ig_live_…`). Scopes: `read` (GET) and `full` (all methods). Mint a key at https://inboxguard.io/settings\n    or per https://inboxguard.io/auth.md.'\n  sources:\n  - openapi/inboxguard-io-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.inboxguard.io/oauth/token\n    scopes: 2\n  description: 'OAuth-shaped wrapper around the same API key. The ONLY grant is client_credentials\n    at POST https://api.inboxguard.io/oauth/token, where the client_secret IS an InboxGuard\n    API key (HTTP Basic or body); the returned access_token\
  \ is that same key. There is NO authorization_code\n    flow, NO PKCE, and NO /oauth/authorize endpoint. Discovery: /.well-known/oauth-authorization-server\n    and /.well-known/oauth-p'\n  sources:\n  - openapi/inboxguard-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/inboxguard-io/authentication/inboxguard-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Email Deliverability
- DMARC
- DNS Monitoring
- Authentication
- Security
---
