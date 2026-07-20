---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kudobuzz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kudobuzz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kudobuzz
provider_slug: kudobuzz
scheme_count: 2
schemes:
- context: server
  description: The Kudobuzz account token. Used for server-side calls. Passed to the official client wrapper as `accessToken`. Must never be exposed in browser code.
  id: kudobuzz_token
  name: accessToken
  secret: true
  source: https://docs.kudobuzz.com/auth.md
  type: apiKey
- context: browser
  description: The Kudobuzz client id. Used for client-side / browser calls where a secret token cannot be safely held. Passed to the official client wrapper as `clientId`.
  id: kudobuzz_client_id
  name: clientId
  secret: false
  source: https://docs.kudobuzz.com/auth.md
  type: apiKey
slug: kudobuzz-authentication
source_filename: kudobuzz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kudobuzz.com/auth.md\ndocs: https://docs.kudobuzz.com/#/auth\nnotes: >-\n  Kudobuzz does not publish an OpenAPI definition, so this profile is taken\n  verbatim from the published authentication page of the Kudobuzz API docs\n  rather than derived from securitySchemes. Kudobuzz uses a two-credential\n  model split by execution context: a secret account token for server-side\n  calls and a public client id for browser-side calls. There is no OAuth 2.0\n  authorization-code flow and therefore no scope surface (scopes/ is\n  intentionally absent for this provider).\naccess_model:\n  gated: true\n  how_to_get_access: >-\n    API access is granted per account. Merchants on the Buffet plan have full\n    API access; app developers building integrations get API access for free.\n    Access is requested by emailing the Kudobuzz team, which then issues\n    credentials.\n  request_url: https://kudobuzz.com/developer-api\n\
  \  eligibility:\n    - Kudobuzz merchants on the Buffet plan\n    - Third-party app developers building Kudobuzz integrations (free)\ncredentials_location: https://dashboard.kudobuzz.com/settings\nschemes:\n  - id: kudobuzz_token\n    type: apiKey\n    name: accessToken\n    context: server\n    secret: true\n    description: >-\n      The Kudobuzz account token. Used for server-side calls. Passed to the\n      official client wrapper as `accessToken`. Must never be exposed in\n      browser code.\n    source: https://docs.kudobuzz.com/auth.md\n  - id: kudobuzz_client_id\n    type: apiKey\n    name: clientId\n    context: browser\n    secret: false\n    description: >-\n      The Kudobuzz client id. Used for client-side / browser calls where a\n      secret token cannot be safely held. Passed to the official client\n      wrapper as `clientId`.\n    source: https://docs.kudobuzz.com/auth.md\nusage_example:\n  language: javascript\n  package: \"@kudobuzz/kbclient\"\n  code: |\n    import\
  \ makeClient from '@kudobuzz/kbclient'\n    const client = makeClient({\n        accessToken: 'Your access token here',\n        clientId: 'Your client ID here'\n    })\ntransport:\n  https_required: true\n  evidence: >-\n    The Kudobuzz API standards require HTTPS/TLS for all API access\n    (https://github.com/kudobuzz/api-standards).\ninternal_standard:\n  note: >-\n    Kudobuzz's own published API design standard recommends OAuth 2.0 bearer\n    tokens for its services. The public Developer API as documented today ships\n    the token + client id model above, not an OAuth authorization server.\n  source: https://github.com/kudobuzz/api-standards#security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kudobuzz/refs/heads/main/authentication/kudobuzz-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Reviews
- User Generated Content
- Ecommerce
- Social Proof
- Conversion Rate Optimization
- Marketing
- Shopify
- Customer Feedback
- SaaS
---
