---
api_key_in:
- query
api_specs:
- filename: madaket-provider-api.yml
  format: yaml
  label: Madaket Provider API
  slug: provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madaket/refs/heads/main/openapi/madaket-provider-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Madaket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Madaket secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Madaket
provider_slug: madaket
scheme_count: 2
schemes:
- description: Madaket-issued API key (UUID form). Issued on request; contact Madaket.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/madaket-provider-api.yml
  - https://registry.npmjs.org/@madaket/provider-api-client-js
  type: apiKey
- description: Time-windowed derived token. URL-safe Base64 of SHA-256(api_key + api_secret + timestamp), where timestamp is the current GMT time formatted yyyy-mm-dd-HH-MM with the final character removed, creating a rolling ten-minute window. Valid at least 10 and at most 20 minutes.
  in: query
  name: auth_token
  parameter: auth_token
  sources:
  - openapi/madaket-provider-api.yml
  - https://registry.npmjs.org/@madaket/api-token-generator
  type: apiKey
slug: madaket-authentication
source_filename: madaket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://registry.npmjs.org/@madaket/provider-api-client-js (first-party README,\n  @madaket/provider-api-client-js@0.0.3) + openapi/madaket-provider-api.yml\ndocs: https://www.npmjs.com/package/@madaket/provider-api-client-js#documentation-for-authentication\nnote: >-\n  Madaket documents the Provider API authentication scheme verbatim in the README of its own\n  npm clients (@madaket/provider-api-client-js, @madaket/provider-api-client-ts) and ships a\n  standalone token generator (@madaket/api-token-generator). Both credentials travel as QUERY\n  STRING parameters, not headers. There is no OAuth 2.0 / OIDC surface, so scopes/ is not\n  applicable. Credentials are issued by Madaket on request — there is no self-service key\n  issuance.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  self_service_signup: false\n  credential_issuance: contact Madaket; no public\
  \ developer signup\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Madaket-issued API key (UUID form). Issued on request; contact Madaket.\n  sources:\n  - openapi/madaket-provider-api.yml\n  - https://registry.npmjs.org/@madaket/provider-api-client-js\n- name: auth_token\n  type: apiKey\n  in: query\n  parameter: auth_token\n  description: >-\n    Time-windowed derived token. URL-safe Base64 of SHA-256(api_key + api_secret + timestamp),\n    where timestamp is the current GMT time formatted yyyy-mm-dd-HH-MM with the final character\n    removed, creating a rolling ten-minute window. Valid at least 10 and at most 20 minutes.\n  sources:\n  - openapi/madaket-provider-api.yml\n  - https://registry.npmjs.org/@madaket/api-token-generator\ntoken_derivation:\n  algorithm: SHA-256\n  cleartext: <api_key><api_secret><timestamp>\n  timestamp_format: 'GMT yyyy-mm-dd-HH-MM with the trailing character truncated (10-minute window)'\n  encoding: Base64,\
  \ then URL-safe substitution (+ -> -, / -> _, trailing = stripped)\n  validity: at least 10 minutes, at most 20 minutes\n  reference_implementation: https://www.npmjs.com/package/@madaket/api-token-generator\nobservations:\n- id: secret-never-transmitted\n  note: The API secret is never sent on the wire; only a time-bounded hash of it is. That is a\n    deliberate and defensible design for a 2018-era key scheme.\n- id: credentials-in-query-string\n  note: >-\n    Both api_key and auth_token are QUERY parameters, so they are written to access logs,\n    proxy logs and browser history in a way an Authorization header would not be. For an API\n    carrying provider PII (SSN, DOB, DEA numbers) this is the most significant weakness in the\n    scheme.\n- id: no-scopes\n  note: No OAuth 2.0, no scopes and no per-operation permission model are published. Every\n    credential appears to carry the full surface it is entitled to.\n- id: authorized-query-models\n  note: >-\n    The spec distinguishes\
  \ plain (Board, Specialty, University) from *Authorized* query models\n    (AdverseActionAuthorizedSearchQuery, DeaLicenseAuthorizedFilterQuery, ...) on the\n    provider-sensitive resources, which implies an authorization tier is enforced server-side\n    on the resources carrying regulated data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madaket/refs/heads/main/authentication/madaket-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Healthcare
- Provider Data Management
- Payer Enrollment
- Credentialing
- Provider Directory
- EDI
- Health Insurance
- Licensing
- Healthcare Administration
---
