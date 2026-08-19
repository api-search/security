---
api_key_in:
- header
api_specs:
- filename: malt-exposed-apis-openapi.yml
  format: yaml
  label: Malt Exposed APIs
  slug: malt-exposed-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/malt/refs/heads/main/openapi/malt-exposed-apis-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Malt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Malt secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Malt
provider_slug: malt
scheme_count: 2
schemes:
- applied_note: Declared in components.securitySchemes but referenced by no operation and not present in the document's global `security`. Effectively dead in the contract.
  applied_to_operations: 0
  bearerFormat: JWT
  description: API token obtained from your Malt representative
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/malt-exposed-apis-openapi.yml
  type: http
- applied_note: The six SCIM operations under /scim/v2/Users.
  applied_to_operations: 6
  description: To obtain an access token, please follow the instructions at https://api.malt.com
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/malt-exposed-apis-openapi.yml
  type: apiKey
slug: malt-authentication
source_filename: malt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/malt-exposed-apis-openapi.yml\ndocs: https://api.malt.com/\nnote: >-\n  Baseline derived mechanically from the OpenAPI securitySchemes, then upgraded from Malt's own\n  published authentication guidance (the long info.description on the unified spec, which is the\n  entirety of Malt's API documentation). Two findings a client must know before writing code.\n  (1) The documented header form is a BARE token — `Authorization: your-api-token-here` — with no\n  `Bearer ` prefix, even though the spec also declares an http/bearer scheme with bearerFormat JWT.\n  The prose and the spec disagree; the prose plus the worked cURL and JavaScript examples all show\n  the bare form, so that is what to send. (2) The declared BearerAuth scheme is applied to NO\n  operation, the document's global `security` is an EMPTY ARRAY, and the seven /freelancer/*\n  operations declare no security requirement at all — yet a live unauthenticated\
  \ call to\n  /freelancer/invoices returns 401. The contract understates its own auth requirement; only the six\n  SCIM operations reference ApiKeyAuth.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mutual_tls: false\n  header: Authorization\n  prefix: none (bare token, per Malt's documented examples)\n  token_lifetime: long-lived (no expiry documented, no refresh mechanism)\n  rotation: manual (the docs advise rotating tokens regularly; no API for it)\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: API token obtained from your Malt representative\n  applied_to_operations: 0\n  applied_note: >-\n    Declared in components.securitySchemes but referenced by no operation and not present in the\n    document's global `security`. Effectively dead in the contract.\n  sources:\n  - openapi/malt-exposed-apis-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n\
  \  parameter: Authorization\n  description: >-\n    To obtain an access token, please follow the instructions at https://api.malt.com\n  applied_to_operations: 6\n  applied_note: The six SCIM operations under /scim/v2/Users.\n  sources:\n  - openapi/malt-exposed-apis-openapi.yml\ntoken_types:\n- name: Freelancer account token\n  audience: individual freelancer\n  self_serve: true\n  obtain: >-\n    Create an identity at https://www.malt.com/signup, then generate the token at\n    https://www.malt.com/account/tokens (My Account > API Keys), selecting the permission scopes.\n  scopes: >-\n    The token-creation UI offers \"related permission scopes\" per Malt's own instructions, but the\n    scope names are not published anywhere public and no oauth2 scope map exists in the spec — so\n    the scope vocabulary is only visible to a signed-in account holder. No scopes/ artifact is\n    emitted for that reason.\n  covers:\n  - /freelancer/invoices\n  - /freelancer/invoices/{id}\n  - /freelancer/invoices/{id}/pdf\n\
  \  - /freelancer/payments\n  - /freelancer/fee-invoices\n  - /freelancer/fee-invoices/{id}\n  - /freelancer/fee-invoices/{id}/pdf\n- name: Client team token\n  audience: a buying team inside a client company\n  self_serve: false\n  obtain: Contact your Malt representative.\n- name: Organization token\n  audience: an enterprise organization\n  self_serve: false\n  obtain: Contact your Malt representative.\n  covers:\n  - /scim/v2/Users\n  - /scim/v2/Users/{userId}\nauthorization_model:\n  kind: identity-based\n  detail: >-\n    Malt's own wording: \"APIs are accessible with a given identity based scope at malt.\" The token's\n    identity — freelancer, client team, or organization — determines what is visible, rather than a\n    scope string presented per request. A practical consequence: a 403 from this API most often\n    means the WRONG TOKEN TYPE was used, not a missing scope.\ntoken_handling:\n  displayed_once: true\n  displayed_once_note: >-\n    Malt's instructions state the token\
  \ \"will only be accessible at the moment you see it\" — capture\n    it at creation.\n  published_guidance:\n  - Never expose your token in client-side code\n  - Store tokens securely\n  - Rotate tokens regularly\n  - Monitor token usage in your API dashboard\n  guidance_gap: >-\n    The guidance refers to monitoring \"token usage in your API dashboard\", but no such dashboard is\n    documented or linked anywhere in the public surface.\ndiscovery:\n  oauth_authorization_server: 404 at https://api.malt.com/.well-known/oauth-authorization-server\n  oauth_protected_resource: 404 at https://api.malt.com/.well-known/oauth-protected-resource\n  openid_configuration: 404 at https://api.malt.com/.well-known/openid-configuration\n  finding: >-\n    No machine-readable auth discovery of any kind. An agent cannot negotiate credentials; a human\n    must obtain a token out of band.\nlive_behaviour:\n- url: https://api.malt.com/freelancer/invoices?since=2026-01-01\n  no_credentials: true\n  http_status:\
  \ 401\n  content_length: 0\n  fetched: '2026-08-17'\n  note: >-\n    Confirms the freelancer surface is auth-gated at runtime despite declaring no security in the\n    spec. The 401 carries no body, so not even the documented error envelope appears.\n- url: https://api.malt.com/scim/v2/Users\n  no_credentials: true\n  http_status: 401\n  content_length: 0\n  fetched: '2026-08-17'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/malt/refs/heads/main/authentication/malt-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Marketplace
- Freelance Marketplace
- Freelance Management System
- Talent Marketplace
- Workforce Management
- Contingent Workforce
- Invoicing
- Payments
- SCIM
- Identity Provisioning
- Procurement
- Future of Work
- France
- Europe
---
