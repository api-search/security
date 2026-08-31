---
api_key_in: []
api_specs:
- filename: enrich-so-email-finder-api-openapi.yml
  format: yaml
  label: Enrich Email Finder API
  slug: enrich-so-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-email-finder-api-openapi.yml
- filename: enrich-so-lead-finder-api-openapi.yml
  format: yaml
  label: Enrich Lead Finder API
  slug: enrich-so-lead-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-lead-finder-api-openapi.yml
- filename: enrich-so-phone-finder-api-openapi.yml
  format: yaml
  label: Enrich Phone Finder API
  slug: enrich-so-phone-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-phone-finder-api-openapi.yml
- filename: enrich-so-teams-api-openapi.yml
  format: yaml
  label: Enrich Teams API
  slug: enrich-so-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-teams-api-openapi.yml
- filename: enrich-so-people-search-api-openapi.yml
  format: yaml
  label: Enrich People Search API
  slug: enrich-so-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-people-search-api-openapi.yml
- filename: enrich-so-authentication-api-openapi.yml
  format: yaml
  label: Enrich Authentication API
  slug: enrich-so-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-authentication-api-openapi.yml
- filename: enrich-so-company-followers-api-openapi.yml
  format: yaml
  label: Enrich Company Followers API
  slug: enrich-so-company-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-company-followers-api-openapi.yml
- filename: enrich-so-company-followers-count-estimation-api-openapi.yml
  format: yaml
  label: Enrich Company Followers/Count Estimation API
  slug: enrich-so-company-followers-count-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-company-followers-count-estimation-api-openapi.yml
- filename: enrich-so-email-validation-api-openapi.yml
  format: yaml
  label: Enrich Email Validation API
  slug: enrich-so-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-email-validation-api-openapi.yml
- filename: enrich-so-enrich-api-openapi.yml
  format: yaml
  label: Enrich Enrich API
  slug: enrich-so-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-enrich-api-openapi.yml
- filename: enrich-so-ip-to-company-api-openapi.yml
  format: yaml
  label: Enrich IP to Company API
  slug: enrich-so-ip-to-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-ip-to-company-api-openapi.yml
- filename: enrich-so-reverse-email-lookup-api-openapi.yml
  format: yaml
  label: Enrich Reverse Email Lookup API
  slug: enrich-so-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-reverse-email-lookup-api-openapi.yml
- filename: enrich-so-wallets-api-openapi.yml
  format: yaml
  label: Enrich Wallets API
  slug: enrich-so-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-wallets-api-openapi.yml
- filename: enrich-so-account-api-openapi.yml
  format: yaml
  label: Enrich Account API
  slug: enrich-so-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-account-api-openapi.yml
- filename: enrich-so-company-intelligence-api-openapi.yml
  format: yaml
  label: Enrich Company Intelligence API
  slug: enrich-so-company-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-company-intelligence-api-openapi.yml
- filename: enrich-so-email-verification-api-openapi.yml
  format: yaml
  label: Enrich Email Verification API
  slug: enrich-so-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-email-verification-api-openapi.yml
- filename: enrich-so-person-enrichment-api-openapi.yml
  format: yaml
  label: Enrich Person Enrichment API
  slug: enrich-so-person-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-person-enrichment-api-openapi.yml
- filename: enrich-so-webhooks-api-openapi.yml
  format: yaml
  label: Enrich Webhooks API
  slug: enrich-so-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: Enrich authenticates the REST API v3 with a single static, organization-scoped API key, accepted in either the x-api-key header (recommended) or as an Authorization Bearer token. There are no scopes, no per-key permissions and no OAuth on the REST API. OAuth 2.0 exists only on the separate MCP surface at mcp.enrich.so — see scopes/enrich-so-scopes.yml.
kind: authentication
layout: security
method: searched
name: Enrich So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enrich secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enrich
provider_slug: enrich-so
scheme_count: 2
schemes:
- description: API key passed in the x-api-key header. Keys are created and revoked in the Enrich dashboard at https://dash.enrich.so/dashboard/api-keys, are scoped to the organization (team) behind the account, and carry member-level permissions. The key is shown once at creation.
  in: header
  keyName: x-api-key
  key_prefix: sk_
  name: ApiKeyHeader
  prefix_note: Enrich publishes two different key formats. The authentication documentation page shows "sk_prod_a1b2c3d4e5f6..." while the securityScheme descriptions inside the OpenAPI fragments Enrich embeds in its own endpoint pages say "sk_live_ (64 characters)". A consumer cannot tell which prefix a live key carries from the docs alone. Reported as an inconsistency, not resolved here.
  recommended: true
  sources:
  - https://doc.enrich.so/authentication-1951026m0
  - openapi/_original/enrich-so-v3-harvested-openapi.yml
  type: apiKey
- description: 'The same API key may be sent as an Authorization Bearer token ("Authorization: Bearer sk_..."). This is HTTP Bearer transport of a static key, not an OAuth access token — no token endpoint, no expiry, no refresh, and no WWW-Authenticate challenge is returned on 401.'
  name: BearerToken
  scheme: bearer
  sources:
  - https://doc.enrich.so/authentication-1951026m0
  - openapi/_original/enrich-so-v3-harvested-openapi.yml
  type: http
slug: enrich-so-authentication
source_filename: enrich-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://doc.enrich.so/authentication-1951026m0\ndocs: https://doc.enrich.so/authentication-1951026m0\nderived_from: openapi/_original/enrich-so-v3-harvested-openapi.yml\nprobed: '2026-08-14'\nprovider: Enrich\nproviderId: enrich-so\ndescription: >-\n  Enrich authenticates the REST API v3 with a single static, organization-scoped API key,\n  accepted in either the x-api-key header (recommended) or as an Authorization Bearer\n  token. There are no scopes, no per-key permissions and no OAuth on the REST API. OAuth\n  2.0 exists only on the separate MCP surface at mcp.enrich.so — see\n  scopes/enrich-so-scopes.yml.\nsummary:\n  types:\n  - apiKey\n  - http\n  oauth2: false\n  scopes: false\n  mtls: false\n  key_rotation: supported\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  keyName: x-api-key\n  recommended: true\n  description: >-\n    API key passed in the x-api-key header. Keys are created and revoked in\
  \ the Enrich\n    dashboard at https://dash.enrich.so/dashboard/api-keys, are scoped to the organization\n    (team) behind the account, and carry member-level permissions. The key is shown once\n    at creation.\n  key_prefix: sk_\n  prefix_note: >-\n    Enrich publishes two different key formats. The authentication documentation page\n    shows \"sk_prod_a1b2c3d4e5f6...\" while the securityScheme descriptions inside the\n    OpenAPI fragments Enrich embeds in its own endpoint pages say \"sk_live_ (64\n    characters)\". A consumer cannot tell which prefix a live key carries from the docs\n    alone. Reported as an inconsistency, not resolved here.\n  sources:\n  - https://doc.enrich.so/authentication-1951026m0\n  - openapi/_original/enrich-so-v3-harvested-openapi.yml\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    The same API key may be sent as an Authorization Bearer token\n    (\"Authorization: Bearer sk_...\"). This is HTTP Bearer transport of a static\
  \ key, not\n    an OAuth access token — no token endpoint, no expiry, no refresh, and no\n    WWW-Authenticate challenge is returned on 401.\n  sources:\n  - https://doc.enrich.so/authentication-1951026m0\n  - openapi/_original/enrich-so-v3-harvested-openapi.yml\napplied_to:\n  operations: 51\n  every_operation_requires_auth: true\n  anonymous_endpoints: none\nlive_probe:\n  url: https://dev.enrich.so/api/v3/wallets/balance\n  method: GET\n  credentials: none\n  http_status: 401\n  content_type: application/problem+json\n  body: >-\n    {\"type\":\"https://dev.enrich.so/errors/unauthorized\",\"title\":\"Unauthorized\",\"status\":401,\n    \"detail\":\"This endpoint requires API key authentication. Provide key via x-api-key\n    header or Authorization: Bearer sk_*\"}\n  date: '2026-08-14'\nfailure_modes:\n- status: 401\n  cause: No key supplied, key does not start with sk_, or key is invalid.\n- status: 401\n  cause: Key has been disabled in the dashboard.\n  remediation: Re-enable it\
  \ from https://dash.enrich.so/dashboard/api-keys.\n- status: 403\n  cause: Account suspended.\n- status: 403\n  cause: The organization linked to the API key no longer exists.\n- status: 429\n  cause: The API key exceeded its rate limit.\nkey_management:\n  console: https://dash.enrich.so/dashboard/api-keys\n  rotation: >-\n    Keys rotate from the dashboard without downtime — the old key stays active until it is\n    explicitly revoked.\n  per_environment_keys: recommended by Enrich (separate development and production keys)\n  scoping: >-\n    No per-key scoping is available. Every key can call every endpoint the organization\n    has access to, including the 500-credit phone lookup and the 575-credit lead reveal.\n    Separate keys per workload are the only cost-attribution mechanism.\n  secret_handling: >-\n    Enrich's own guidance: never commit keys, use environment variables or a secrets\n    manager, rotate regularly, revoke compromised keys immediately.\nmcp_surface:\n  endpoint:\
  \ https://mcp.enrich.so/mcp\n  oauth: true\n  scopes:\n  - mcp:tools\n  api_key_accepted: true\n  note: >-\n    The MCP server accepts either an OAuth token (authorization_code + PKCE, dynamic\n    client registration) or the same Enrich API key via Bearer/x-api-key. Detail in\n    mcp/enrich-so-mcp.yml and scopes/enrich-so-scopes.yml.\nlegacy_surface:\n  endpoint: https://api.enrich.so\n  scheme: http bearer\n  bearer_format: JWT\n  note: >-\n    The legacy v1/v2 Enrich Labs API declares bearerAuth with bearerFormat JWT — a\n    different credential model from the v3 API key. Spec at\n    openapi/enrich-so-legacy-api-openapi.json.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/authentication/enrich-so-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Enrichment
- Contact Discovery
- Web Intelligence
- B2B Data
- Lead Enrichment
- Email Finder
- Email Verification
- Phone Numbers
- People Search
- IP Intelligence
- LinkedIn
- Reference Data
- MCP
---
