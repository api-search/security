---
api_key_in:
- header
- query
api_specs:
- filename: similarweb-account-api-openapi.yml
  format: yaml
  label: SimilarWeb Account API
  slug: similarweb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-account-api-openapi.yml
- filename: similarweb-app-intelligence-api-openapi.yml
  format: yaml
  label: SimilarWeb App Intelligence API
  slug: similarweb-app-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-app-intelligence-api-openapi.yml
- filename: similarweb-credits-api-openapi.yml
  format: yaml
  label: SimilarWeb Credits API
  slug: similarweb-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-credits-api-openapi.yml
- filename: similarweb-geography-api-openapi.yml
  format: yaml
  label: SimilarWeb Geography API
  slug: similarweb-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-geography-api-openapi.yml
- filename: similarweb-integrations-api-openapi.yml
  format: yaml
  label: SimilarWeb Integrations API
  slug: similarweb-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-integrations-api-openapi.yml
- filename: similarweb-keywords-api-openapi.yml
  format: yaml
  label: SimilarWeb Keywords API
  slug: similarweb-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-keywords-api-openapi.yml
- filename: similarweb-lead-enrichment-api-openapi.yml
  format: yaml
  label: SimilarWeb Lead Enrichment API
  slug: similarweb-lead-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-lead-enrichment-api-openapi.yml
- filename: similarweb-rankings-api-openapi.yml
  format: yaml
  label: SimilarWeb Rankings API
  slug: similarweb-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-rankings-api-openapi.yml
- filename: similarweb-reports-api-openapi.yml
  format: yaml
  label: SimilarWeb Reports API
  slug: similarweb-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-reports-api-openapi.yml
- filename: similarweb-similar-sites-api-openapi.yml
  format: yaml
  label: SimilarWeb Similar Sites API
  slug: similarweb-similar-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-similar-sites-api-openapi.yml
- filename: similarweb-traffic-and-engagement-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic and Engagement API
  slug: similarweb-traffic-and-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-and-engagement-api-openapi.yml
- filename: similarweb-traffic-sources-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic Sources API
  slug: similarweb-traffic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-sources-api-openapi.yml
- filename: similarweb-webhooks-api-openapi.yml
  format: yaml
  label: SimilarWeb Webhooks API
  slug: similarweb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: 'Similarweb authenticates its REST and Batch APIs with a single long-lived API key — no OAuth, no OIDC, no mTLS. The hosted MCP server is the one exception: it accepts the same API key in an `api-key` header OR an OAuth 2.1 bearer token from its own authorization server. Derived from the OpenAPI securitySchemes and upgraded from the provider''s authentication guide, which documents the key lifecycle the specs cannot express.'
kind: authentication
layout: security
method: searched
name: Similarweb Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SimilarWeb secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SimilarWeb
provider_slug: similarweb
scheme_count: 3
schemes:
- applies_to:
  - rest
  - batch
  - mcp
  description: Similarweb API key passed as a request header. The form used in every doc example.
  in: header
  name: apiKeyHeader
  parameter: api-key
  sources:
  - openapi/similarweb-account-api-openapi.yml
  - openapi/similarweb-app-intelligence-api-openapi.yml
  - openapi/similarweb-credits-api-openapi.yml
  - openapi/similarweb-geography-api-openapi.yml
  - openapi/similarweb-integrations-api-openapi.yml
  - openapi/similarweb-keywords-api-openapi.yml
  - openapi/similarweb-lead-enrichment-api-openapi.yml
  - openapi/similarweb-rankings-api-openapi.yml
  - openapi/similarweb-reports-api-openapi.yml
  - openapi/similarweb-similar-sites-api-openapi.yml
  - openapi/similarweb-traffic-and-engagement-api-openapi.yml
  - openapi/similarweb-traffic-sources-api-openapi.yml
  - openapi/similarweb-webhooks-api-openapi.yml
  type: apiKey
- applies_to:
  - rest
  description: Similarweb API key passed as a query parameter. Accepted, but it puts the credential in URLs, logs and referrers — prefer the header.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/_original/similarweb-rest-api-openapi.yml
  type: apiKey
- applies_to:
  - mcp
  description: OAuth 2.1 bearer token accepted by the hosted MCP server as an alternative to the api-key header. Issued by https://mcp-auth.similarweb.com.
  name: mcpBearer
  scheme: bearer
  sources:
  - well-known/similarweb-oauth-protected-resource.json
  type: http
slug: similarweb-authentication
source_filename: similarweb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/*.yml\ndocs: https://docs.similarweb.com/api-v5/getting-started/authentication\nalso_documented_at:\n- https://developers.similarweb.com/docs/authentication\n- https://docs.similarweb.com/api-v5/similarweb-mcp/mcp-setup\ndescription: >-\n  Similarweb authenticates its REST and Batch APIs with a single long-lived API key — no\n  OAuth, no OIDC, no mTLS. The hosted MCP server is the one exception: it accepts the same\n  API key in an `api-key` header OR an OAuth 2.1 bearer token from its own authorization\n  server. Derived from the OpenAPI securitySchemes and upgraded from the provider's\n  authentication guide, which documents the key lifecycle the specs cannot express.\n\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\n  oauth2_scope: MCP surface only\n\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Similarweb\
  \ API key passed as a request header. The form used in every doc example.\n  applies_to: [rest, batch, mcp]\n  sources:\n  - openapi/similarweb-account-api-openapi.yml\n  - openapi/similarweb-app-intelligence-api-openapi.yml\n  - openapi/similarweb-credits-api-openapi.yml\n  - openapi/similarweb-geography-api-openapi.yml\n  - openapi/similarweb-integrations-api-openapi.yml\n  - openapi/similarweb-keywords-api-openapi.yml\n  - openapi/similarweb-lead-enrichment-api-openapi.yml\n  - openapi/similarweb-rankings-api-openapi.yml\n  - openapi/similarweb-reports-api-openapi.yml\n  - openapi/similarweb-similar-sites-api-openapi.yml\n  - openapi/similarweb-traffic-and-engagement-api-openapi.yml\n  - openapi/similarweb-traffic-sources-api-openapi.yml\n  - openapi/similarweb-webhooks-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    Similarweb API key passed as a query parameter. Accepted, but it puts the credential in\n    URLs, logs\
  \ and referrers — prefer the header.\n  applies_to: [rest]\n  sources: [openapi/_original/similarweb-rest-api-openapi.yml]\n- name: mcpBearer\n  type: http\n  scheme: bearer\n  description: >-\n    OAuth 2.1 bearer token accepted by the hosted MCP server as an alternative to the\n    api-key header. Issued by https://mcp-auth.similarweb.com.\n  applies_to: [mcp]\n  sources: [well-known/similarweb-oauth-protected-resource.json]\n\nkey_lifecycle:\n  issued_by: account administrators only\n  console: https://account.similarweb.com/standard-api\n  platform_path: Settings > Account > Data Tools > REST API / Batch API\n  max_active_keys_per_user: 3\n  expiry: none\n  activation_required: true\n  activation_note: >-\n    A newly created key must have its Activation toggle switched on. An inactive key returns\n    \"Invalid API key\" errors, which reads identically to a wrong key.\n  scoped_key: false\n  unified_key: >-\n    As of API V5, ONE key works across both REST and Batch. API V4 required\
  \ separate keys\n    for the two surfaces — a migration detail that breaks V4-era integrations silently.\n  credit_limits: >-\n    Admins can set per-user credit limits per API (for example 10K on REST and 10K on\n    Batch). Limits are per user, not per key.\n  revocation: >-\n    Removing a user from the account revokes their keys; keys can also be transferred to\n    another active user or disabled individually.\n\nfailure_modes:\n- {status: 401, meaning: 'invalid or inactive key (observed body: `invalid API key`) — also returned for a malformed domain'}\n- {status: 403, meaning: invalid API key or exhausted data credits (REST, per the error guide)}\n\ngaps:\n- No OAuth, OIDC or mTLS on the REST/Batch surface\n- No key rotation API — keys are managed only through the platform UI\n- No scoping: a key carries the whole subscription entitlement\n- 401 is overloaded across authentication failure and data-not-found\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: https://docs.similarweb.com/api-v5/getting-started/authentication.md,\
  \ http_status: 200}\n  - {url: https://developers.similarweb.com/docs/authentication.md, http_status: 200}\n  - {url: 'https://api.similarweb.com/v1/website/cnn.com/total-traffic-and-engagement/visits (invalid key)', http_status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/authentication/similarweb-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-Commerce
- SEO
---
