---
api_key_in: []
api_specs:
- filename: lucidya-ltd-social-listening-api-openapi.yml
  format: yaml
  label: Lucidya Social Listening API
  slug: lucidya-social-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-social-listening-api-openapi.yml
- filename: lucidya-ltd-ai-api-openapi.yml
  format: yaml
  label: Lucidya AI API
  slug: lucidya-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-ai-api-openapi.yml
- filename: lucidya-ltd-cdp-api-openapi.yml
  format: yaml
  label: Lucidya CDP API
  slug: lucidya-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-cdp-api-openapi.yml
- filename: lucidya-ltd-omnichannel-api-openapi.yml
  format: yaml
  label: Lucidya OmniChannel API
  slug: lucidya-omnichannel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-omnichannel-api-openapi.yml
- filename: lucidya-ltd-omniserve-analytics-api-openapi.yml
  format: yaml
  label: Lucidya OmniServe Analytics API
  slug: lucidya-omniserve-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-omniserve-analytics-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Lucidya Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucidya Ltd declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lucidya Ltd
provider_slug: lucidya-ltd
scheme_count: 1
schemes:
- declared_in_spec:
  - openapi/lucidya-ltd-omniserve-analytics-api-openapi.yml
  description: '"The API authorization token for the request" — declared verbatim as an apiKey/header securityScheme in the OmniServe Analytics OpenAPI, and used identically (undeclared in the spec but documented in prose and in every cURL sample) by the Social Listening, AI, CDP and OmniChannel APIs.'
  documented_only:
  - openapi/lucidya-ltd-social-listening-api-openapi.yml
  - openapi/lucidya-ltd-ai-api-openapi.yml
  - openapi/lucidya-ltd-cdp-api-openapi.yml
  - openapi/lucidya-ltd-omnichannel-api-openapi.yml
  example_header: 'luc-authorization: <YOUR_API_TOKEN>'
  in: header
  name: luc-authorization
  scheme_name: OmniserveToken
  type: apiKey
slug: lucidya-ltd-authentication
source_filename: lucidya-ltd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.lucidya.com/docs/Social-Listening-api/uh64vtmx7x4kl-authorization\nname: Lucidya API Authentication\ntype: Authentication\nsummary: >-\n  Every Lucidya public API product uses one API-token scheme: a bearer-style\n  opaque token sent in the custom HTTP header `luc-authorization`. Tokens are\n  self-service generated from the Lucidya CXM console (Settings -> Lucidya API)\n  once a Customer Success Manager has approved an access request, and each token\n  is bound to an API product type and to one or more subnet IP allow-list\n  entries.\ncorrections:\n  - date: '2026-08-13'\n    was: 'oauth2 (per-product OAuth client applications)'\n    now: 'apiKey in header `luc-authorization`'\n    why: >-\n      The 2026-07-20 pass could not reach the Stoplight-hosted Authorization\n      articles and inferred OAuth. The provider's own Authorization pages and the\n      OmniServe OpenAPI securityScheme both state an API-token\
  \ header scheme.\n      Lucidya publishes no OAuth authorization or token endpoint.\nschemes:\n  - type: apiKey\n    name: luc-authorization\n    in: header\n    scheme_name: OmniserveToken\n    description: >-\n      \"The API authorization token for the request\" — declared verbatim as an\n      apiKey/header securityScheme in the OmniServe Analytics OpenAPI, and used\n      identically (undeclared in the spec but documented in prose and in every\n      cURL sample) by the Social Listening, AI, CDP and OmniChannel APIs.\n    example_header: 'luc-authorization: <YOUR_API_TOKEN>'\n    declared_in_spec:\n      - openapi/lucidya-ltd-omniserve-analytics-api-openapi.yml\n    documented_only:\n      - openapi/lucidya-ltd-social-listening-api-openapi.yml\n      - openapi/lucidya-ltd-ai-api-openapi.yml\n      - openapi/lucidya-ltd-cdp-api-openapi.yml\n      - openapi/lucidya-ltd-omnichannel-api-openapi.yml\noauth2: false\noauth2_note: >-\n  No OAuth 2.0 authorization server, token endpoint, scopes\
  \ or grant types are\n  published on any Lucidya host. /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration return 404 on lucidya.com, api.lucidya.com\n  and docs.lucidya.com. Consequently no scopes/ artifact is emitted.\ntoken_issuance:\n  self_serve: partial\n  steps:\n    - Hold an active Lucidya account (AI API additionally requires the CXM Core product).\n    - Log in at https://cxm.lucidya.com/login and open Settings -> Lucidya API.\n    - Click \"Request Access\"; a Customer Success Manager approves the request by email.\n    - After approval, click \"Generate API Key\", pick the API type, name the key and add subnet IP(s).\n    - The token is displayed exactly once and cannot be viewed again.\n  gate: >-\n    Key issuance is CSM-approved, so the credential is not fully self-serve even\n    though the documentation and specs are fully public.\nconstraints:\n  keys_per_api_type: 3\n  api_type_bound: true\n  ip_allowlist:\n    supported: true\n    field:\
  \ Subnet IP(s)\n    multiple: true\n    note: A single key may carry multiple subnet IPs.\n  token_deactivation_days: 30\n  token_deactivation_rule: >-\n    A key not used within a 30-day period is deactivated; an email notice is sent.\n  token_expiration_days: 60\n  token_expiration_rule: >-\n    A key used continuously for a 60-day period reaches expiration; an email\n    alert is sent. A new token must then be generated.\ntransport:\n  https_required: true\n  http_allowed: false\n  note: >-\n    \"API requests must use HTTPS, HTTP requests will not be allowed.\" TLS is\n    documented as the transport standard for all Lucidya REST APIs.\nfailure_modes:\n  - status: 401\n    slug: unauthorized\n    meaning: Authorization error (invalid API key).\n  - status: 403\n    slug: forbidden\n    meaning: >-\n      Request understood but refused — either access is not allowed, or the\n      caller was blocked after too many errors in a short window.\nhosts:\n  - https://api.lucidya.com\n  - https://api.lucidya.com/public_api/omniserve\n\
  docs:\n  - product: Social Listening\n    url: https://docs.lucidya.com/docs/Social-Listening-api/uh64vtmx7x4kl-authorization\n  - product: AI\n    url: https://docs.lucidya.com/docs/ai-api/sjq8uo8o8lt93-authorization\n  - product: CDP\n    url: https://docs.lucidya.com/docs/cdp-api/6tqmgs82r4jxa-authorization\n  - product: OmniChannel\n    url: https://docs.lucidya.com/docs/omnichannel-api/cfqqlsohea8mv-authorization\n  - product: OmniServe Analytics\n    url: https://docs.lucidya.com/docs/omniserve/8s65uy0al6adj-authorization\n  - product: Security Considerations (token expiry, TLS)\n    url: https://docs.lucidya.com/docs/Social-Listening-api/sztlqqzqzmdb0-security-considerations\nnotes: >-\n  Lucidya's own Authorization pages misspell the header as `luc-autharization`\n  in the prose sentence while every code sample, the OmniServe securityScheme and\n  the \"Try Out\" console all use `luc-authorization`. The correct header is\n  `luc-authorization`; the prose spelling is a documentation\
  \ typo and is recorded\n  here so an agent does not copy it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/authentication/lucidya-ltd-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Customer Experience
- Social Listening
- Customer Data Platform
- Analytics
- Artificial Intelligence
- Omnichannel
- Arabic NLP
- MENA
---
