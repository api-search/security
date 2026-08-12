---
api_key_in:
- header
api_specs:
- filename: tadeus-api-integration-openapi.json
  format: json
  label: Tadeus Integration API
  slug: tadeus-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-integration-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tadeus Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tadeus API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tadeus API
provider_slug: tadeus-api
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: X-API-KEY-ID
  required: true
  sources:
  - openapi/tadeus-api-integration-openapi.json
  - https://tadeus.net/api-examples
  type: apiKey
- in: header
  name: api_secret
  parameter: X-API-SECRET
  required: true
  sources:
  - openapi/tadeus-api-integration-openapi.json
  - https://tadeus.net/api-examples
  type: apiKey
slug: tadeus-api-authentication
source_filename: tadeus-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: openapi/tadeus-api-integration-openapi.json\ndocs: https://tadeus.net/api-examples\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  model: static-key-pair\n  oauth2: false\n  oidc: false\n  mtls: false\n  scopes: false\n  rotation_documented: false\n  expiry_documented: false\nquote: >-\n  \"The Integration API is keyed, not session-based. Send your key id and secret as headers\n  on every call. Load them from the environment so they never end up in source control.\"\nissuance:\n  where: Tadeus dashboard, under \"API access\"\n  self_service: true\n  source: https://tadeus.net/api-examples\nschemes:\n  - name: api_key\n    type: apiKey\n    in: header\n    parameter: X-API-KEY-ID\n    required: true\n    sources:\n      - openapi/tadeus-api-integration-openapi.json\n      - https://tadeus.net/api-examples\n  - name: api_secret\n    type: apiKey\n    in: header\n    parameter: X-API-SECRET\n    required: true\n\
  \    sources:\n      - openapi/tadeus-api-integration-openapi.json\n      - https://tadeus.net/api-examples\nspec_vs_docs_discrepancy: >-\n  The Swagger document declares the two headers as SEPARATE apiKey schemes and combines them\n  in a top-level `security: [{api_key: []}, {api_secret: []}]` array, which is OR semantics —\n  a code generator reading the contract alone will produce a client that sends only one\n  header. The documentation is unambiguous that both are required on every call. Correct\n  behaviour is AND; the contract says OR.\nagent_surface:\n  mcp:\n    url: https://app.tadeus.net/mcp\n    scheme: same key pair\n    parameter_names: [api_key_id, api_secret]\n    accepted_in: [query parameters, headers]\n    challenge_status: 401\n    challenge_body: >-\n      {\"detail\":\"Authentication required. Pass 'api_key_id' and 'api_secret' in query\n      parameters or headers.\"}\n    oauth: false\n    note: >-\n      The MCP server accepts the credentials in QUERY PARAMETERS\
  \ as well as headers, which\n      puts long-lived secrets into URLs, proxy logs and browser history. It also does not\n      implement the MCP OAuth flow, and publishes no\n      /.well-known/oauth-protected-resource (403), so an MCP client cannot discover the auth\n      requirement programmatically.\nobserved_behaviour:\n  - url: https://app.tadeus.net/api/integration/v1/organisation/\n    sent: no credentials\n    status: 403\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    www_authenticate: absent\n    note: >-\n      Returns 403 rather than the 401 RFC 9110 specifies for a missing credential, and sends\n      no WWW-Authenticate challenge.\nenterprise:\n  sso: true\n  saml: true\n  note: >-\n    \"SSO, SAML & EU data residency\" is an Enterprise-tier entitlement\n    (https://tadeus.net/#pricing). This is dashboard sign-in, not API authentication — the\n    API surface is key-pair only at every tier.\nprovider_gaps:\n  - >-\n    Express the two headers\
  \ as a single AND requirement in the contract\n    (`security: [{api_key: [], api_secret: []}]`), or the generated clients will be wrong.\n  - Publish key rotation and expiry guidance; neither is documented.\n  - Return 401 with WWW-Authenticate instead of 403 for a missing credential.\n  - Stop accepting the secret in MCP query parameters.\n  - No scopes or least-privilege model exists — one key pair is full account access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/authentication/tadeus-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Voice AI
- Research
- Interviews
- Workforce
- HR Tech
- Conversational AI
- Employee Experience
- AI Agents
- MCP
- EU AI Act
- Compliance
- Employee Engagement
---
