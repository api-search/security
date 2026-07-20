---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gloat Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Gloat secures its APIs with oauth2, apiKey, and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Gloat
provider_slug: gloat
scheme_count: 2
schemes:
- access_token_ttl_seconds: 86400
  applies_to:
  - Skills Foundation
  - Company API
  - Authorization API
  - Candidacy API
  credential_provisioning: Client ID + Client Secret generated in the Gloat Admin Console under Integration > API access (requires IT Admin role). Secret shown once; rotate on suspected compromise.
  flow: clientCredentials
  name: clientCredentialsJWT
  source: https://developer.gloat.com/docs/authentication
  token_request: HTTP Basic header = base64("CLIENT_ID:CLIENT_SECRET")
  token_type: Bearer
  token_url: https://{company_slug}.gloat.com/api/auth/token
  type: oauth2
- applies_to:
  - Talent Marketplace API
  companion_header: X-Tenant-ID
  credential_provisioning: Contact your Gloat representative to obtain an API key.
  features:
  - optional expiration dates
  - CIDR / IP allowlist restrictions
  - HTTPS enforced only
  in: header
  name: gloatApiKey
  parameter_name: X-Gloat-API-Key
  source: https://developer.gloat.com/docs/talent-marketplace-authentication
  type: apiKey
slug: gloat-authentication
source_filename: gloat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.gloat.com/docs/authentication\ndocs:\n- https://developer.gloat.com/docs/authentication\n- https://developer.gloat.com/docs/talent-marketplace-authentication\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    Gloat has two distinct auth schemes. The Customer APIs (Skills Foundation,\n    Company, Authorization, Candidacy) use client-credentials: base64(CLIENT_ID:CLIENT_SECRET)\n    is POSTed as HTTP Basic to a per-tenant token endpoint, returning a 24h JWT used\n    as a Bearer token. The Talent Marketplace APIs use a static API key sent in the\n    X-Gloat-API-Key header (plus X-Tenant-ID), supporting optional expiry and CIDR\n    restrictions. All hosts are per-tenant: https://{company_slug}.gloat.com/api.\nschemes:\n- name: clientCredentialsJWT\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://{company_slug}.gloat.com/api/auth/token\n\
  \  token_request: HTTP Basic header = base64(\"CLIENT_ID:CLIENT_SECRET\")\n  token_type: Bearer\n  access_token_ttl_seconds: 86400\n  applies_to: [Skills Foundation, Company API, Authorization API, Candidacy API]\n  credential_provisioning: >-\n    Client ID + Client Secret generated in the Gloat Admin Console under\n    Integration > API access (requires IT Admin role). Secret shown once; rotate on\n    suspected compromise.\n  source: https://developer.gloat.com/docs/authentication\n- name: gloatApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Gloat-API-Key\n  companion_header: X-Tenant-ID\n  applies_to: [Talent Marketplace API]\n  features:\n  - optional expiration dates\n  - CIDR / IP allowlist restrictions\n  - HTTPS enforced only\n  credential_provisioning: Contact your Gloat representative to obtain an API key.\n  source: https://developer.gloat.com/docs/talent-marketplace-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloat/refs/heads/main/authentication/gloat-authentication.yml
summary_line: oauth2/apiKey/http · 2 schemes
tags:
- Company
- Ai
- Human Resources
- Talent Marketplace
- Skills
- Workforce
- Internal Mobility
- HR Tech
---
