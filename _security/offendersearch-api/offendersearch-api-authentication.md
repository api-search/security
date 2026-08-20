---
api_key_in:
- header
- query
api_specs:
- filename: offendersearch-api-account-api-openapi.yml
  format: yaml
  label: Offendersearch API Account API
  slug: offendersearch-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-account-api-openapi.yml
- filename: offendersearch-api-admin-api-openapi.yml
  format: yaml
  label: Offendersearch API Admin API
  slug: offendersearch-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-admin-api-openapi.yml
- filename: offendersearch-api-auth-api-openapi.yml
  format: yaml
  label: Offendersearch API Auth API
  slug: offendersearch-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-auth-api-openapi.yml
- filename: offendersearch-api-batch-api-openapi.yml
  format: yaml
  label: Offendersearch API Batch API
  slug: offendersearch-api-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-batch-api-openapi.yml
- filename: offendersearch-api-billing-api-openapi.yml
  format: yaml
  label: Offendersearch API Billing API
  slug: offendersearch-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-billing-api-openapi.yml
- filename: offendersearch-api-compat-api-openapi.yml
  format: yaml
  label: Offendersearch API Compat API
  slug: offendersearch-api-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-compat-api-openapi.yml
- filename: offendersearch-api-keys-api-openapi.yml
  format: yaml
  label: Offendersearch API Keys API
  slug: offendersearch-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-keys-api-openapi.yml
- filename: offendersearch-api-proof-docs-api-openapi.yml
  format: yaml
  label: Offendersearch API Proof Docs API
  slug: offendersearch-api-proof-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-proof-docs-api-openapi.yml
- filename: offendersearch-api-records-api-openapi.yml
  format: yaml
  label: Offendersearch API Records API
  slug: offendersearch-api-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-records-api-openapi.yml
- filename: offendersearch-api-report-api-openapi.yml
  format: yaml
  label: Offendersearch API Report API
  slug: offendersearch-api-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-report-api-openapi.yml
- filename: offendersearch-api-search-api-openapi.yml
  format: yaml
  label: Offendersearch API Search API
  slug: offendersearch-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-search-api-openapi.yml
- filename: offendersearch-api-searches-api-openapi.yml
  format: yaml
  label: Offendersearch API Searches API
  slug: offendersearch-api-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-searches-api-openapi.yml
- filename: offendersearch-api-sources-api-openapi.yml
  format: yaml
  label: Offendersearch API Sources API
  slug: offendersearch-api-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-sources-api-openapi.yml
- filename: offendersearch-api-support-api-openapi.yml
  format: yaml
  label: Offendersearch API Support API
  slug: offendersearch-api-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-support-api-openapi.yml
- filename: offendersearch-api-team-api-openapi.yml
  format: yaml
  label: Offendersearch API Team API
  slug: offendersearch-api-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-team-api-openapi.yml
- filename: offendersearch-api-usage-api-openapi.yml
  format: yaml
  label: Offendersearch API Usage API
  slug: offendersearch-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-usage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Offendersearch Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Offendersearch API secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Offendersearch API
provider_slug: offendersearch-api
scheme_count: 4
schemes:
- description: Customer API key. Primary auth for search/records/compat/proof.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/offendersearch-api-openapi.yml
  type: apiKey
- description: Signed session token (HMAC-SHA256). Auth for account/dashboard endpoints; also accepted by POST /v1/search and the compat endpoint.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/offendersearch-api-openapi.yml
  type: http
- description: API key passed as `?key=` — offenders.io demo mode (compat endpoint only).
  in: query
  name: QueryKeyAuth
  parameter: key
  sources:
  - openapi/offendersearch-api-openapi.yml
  type: apiKey
- description: Internal admin credential — separate from customer API keys.
  in: header
  name: AdminAuth
  parameter: X-Admin-Key
  sources:
  - openapi/offendersearch-api-openapi.yml
  type: apiKey
slug: offendersearch-api-authentication
source_filename: offendersearch-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: derived\nsource: openapi/offendersearch-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Customer API key. Primary auth for search/records/compat/proof.\n  sources:\n  - openapi/offendersearch-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Signed session token (HMAC-SHA256). Auth for account/dashboard endpoints; also\n    accepted by POST /v1/search and the compat endpoint.\n  sources:\n  - openapi/offendersearch-api-openapi.yml\n- name: QueryKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key passed as `?key=` — offenders.io demo mode (compat endpoint only).\n  sources:\n  - openapi/offendersearch-api-openapi.yml\n- name: AdminAuth\n  type: apiKey\n  in: header\n  parameter: X-Admin-Key\n  description: Internal admin credential — separate\
  \ from customer API keys.\n  sources:\n  - openapi/offendersearch-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/authentication/offendersearch-api-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Background Checks
- Identity Verification
- Public Records
- Criminal Records
- Compliance
- Trust and Safety
- HR Tech
- Recruiting
- PropTech
- Tenant Screening
- healthcare-screening
- Data API
- MCP Server
- agent-native
---
