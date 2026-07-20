---
api_key_in: []
api_specs:
- filename: kita-capture-openapi.yml
  format: yaml
  label: Kita Capture API
  slug: capture
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-capture-openapi.yml
- filename: kita-underwriter-openapi.yml
  format: yaml
  label: Kita AI Underwriter API
  slug: underwriter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-underwriter-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kita Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kita secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kita
provider_slug: kita
scheme_count: 2
schemes:
- api: Kita Capture API
  description: Organization API key for the Kita Capture document-intelligence API, issued from the Kita dashboard.
  env_var: KITA_API_KEY
  header: 'Authorization: Bearer [example key]'
  issued_from: https://portal.usekita.com
  key_prefix: kita_prod_
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kita-capture-openapi.yml
  type: http
- accepted_headers:
  - 'Authorization: ApiKey kita_uw_...'
  - 'Authorization: Bearer [example key]'
  api: Kita AI Underwriter API
  description: Organization API key for the Kita AI Underwriter API. Displayed once at creation; Kita stores only a SHA-256 hash, so a lost key cannot be recovered and must be revoked and re-minted.
  env_var: KITA_UNDERWRITER_API_KEY
  issued_from: Settings → API keys (organization admin)
  key_prefix: kita_uw_
  key_scopes:
  - grants: GET endpoints — list and read applications, credit picture, memo, documents, conversation, transcripts and exports.
    scope: read
  - grants: Mutations — intake, create/update/delete applications, upload documents, generate memo.
    scope: write
  name: ApiKeyAuth
  scheme: bearer
  scope_enforcement: A valid key without the required scope receives HTTP 403.
  sources:
  - openapi/kita-underwriter-openapi.yml
  type: http
slug: kita-authentication
source_filename: kita-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kita-capture-openapi.yml, openapi/kita-underwriter-openapi.yml\ndocs: https://www.kita.ai/documentation\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  model: organization-scoped API keys\n  oauth2: false\n  openid_connect: false\n  notes: 'Kita uses long-lived organization API keys, not OAuth. Each product issues its own\n    key with its own prefix. The Underwriter key carries coarse read/write scopes enforced\n    per endpoint; those are key scopes, not OAuth scopes, so there is no authorization\n    server, no token endpoint and no scopes/ artifact for this provider. Enterprise plans\n    additionally offer SSO/SAML for dashboard sign-in (not for API calls).'\nschemes:\n- name: BearerAuth\n  api: Kita Capture API\n  type: http\n  scheme: bearer\n  key_prefix: kita_prod_\n  header: 'Authorization: Bearer [example key]'\n  issued_from: https://portal.usekita.com\n  env_var: KITA_API_KEY\n  description:\
  \ Organization API key for the Kita Capture document-intelligence API, issued\n    from the Kita dashboard.\n  sources:\n  - openapi/kita-capture-openapi.yml\n- name: ApiKeyAuth\n  api: Kita AI Underwriter API\n  type: http\n  scheme: bearer\n  key_prefix: kita_uw_\n  accepted_headers:\n  - 'Authorization: ApiKey kita_uw_...'\n  - 'Authorization: Bearer [example key]'\n  issued_from: Settings → API keys (organization admin)\n  env_var: KITA_UNDERWRITER_API_KEY\n  description: Organization API key for the Kita AI Underwriter API. Displayed once at\n    creation; Kita stores only a SHA-256 hash, so a lost key cannot be recovered and must be\n    revoked and re-minted.\n  key_scopes:\n  - scope: read\n    grants: GET endpoints — list and read applications, credit picture, memo, documents,\n      conversation, transcripts and exports.\n  - scope: write\n    grants: Mutations — intake, create/update/delete applications, upload documents,\n      generate memo.\n  scope_enforcement: A valid key\
  \ without the required scope receives HTTP 403.\n  sources:\n  - openapi/kita-underwriter-openapi.yml\nrotation:\n  revocable: true\n  hashed_at_rest: true\n  hash: SHA-256\n  recovery: none — a compromised key must be revoked and regenerated\nhandling:\n  server_side_only: true\n  notes: Kita documents that keys must stay out of browsers and public repositories; the\n    official MCP server takes the key via server-side environment variables.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/authentication/kita-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Fintech
- Lending
- Underwriting
- Credit Scoring
- Document Intelligence
- Document Extraction
- Fraud Detection
- Artificial Intelligence
- Computer Vision
- Emerging Markets
- Loan Origination
---
