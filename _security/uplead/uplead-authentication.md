---
api_key_in:
- header
api_specs:
- filename: uplead-account-api-openapi.yml
  format: yaml
  label: UpLead Account API
  slug: uplead-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-account-api-openapi.yml
- filename: uplead-combined-api-openapi.yml
  format: yaml
  label: UpLead Combined API
  slug: uplead-combined-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-combined-api-openapi.yml
- filename: uplead-company-api-openapi.yml
  format: yaml
  label: UpLead Company API
  slug: uplead-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-company-api-openapi.yml
- filename: uplead-lists-api-openapi.yml
  format: yaml
  label: UpLead Lists API
  slug: uplead-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-lists-api-openapi.yml
- filename: uplead-person-api-openapi.yml
  format: yaml
  label: UpLead Person API
  slug: uplead-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-person-api-openapi.yml
- filename: uplead-prospector-api-openapi.yml
  format: yaml
  label: UpLead Prospector API
  slug: uplead-prospector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-prospector-api-openapi.yml
- filename: uplead-reference-api-openapi.yml
  format: yaml
  label: UpLead Reference API
  slug: uplead-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-reference-api-openapi.yml
- filename: uplead-search-api-openapi.yml
  format: yaml
  label: UpLead Search API
  slug: uplead-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-search-api-openapi.yml
auth_types:
- apiKey
description: 'UpLead uses a single static API key on every call. The key is placed in the Authorization header and sent bare — "Authorization: myapikey" — with no Bearer or other scheme prefix, which is the detail most integrations get wrong. There is no OAuth, no OpenID Connect, no mutual TLS, no signing, no key rotation endpoint, and no scope system: one key carries the account''s full plan entitlement.'
kind: authentication
layout: security
method: searched
name: Uplead Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpLead secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpLead
provider_slug: uplead
scheme_count: 1
schemes:
- description: 'Your UpLead API key passed as the raw value of the Authorization header. The documentation''s example is literally `Authorization: myapikey` — replace `myapikey` with your key and add no prefix.'
  docs: https://docs.uplead.com/#authentication
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  required_on: every operation, including getCredits
  scheme_prefix: null
  sources:
  - openapi/uplead-account-api-openapi.yml
  - openapi/uplead-combined-api-openapi.yml
  - openapi/uplead-company-api-openapi.yml
  - openapi/uplead-lists-api-openapi.yml
  - openapi/uplead-person-api-openapi.yml
  - openapi/uplead-prospector-api-openapi.yml
  - openapi/uplead-reference-api-openapi.yml
  - openapi/uplead-search-api-openapi.yml
  type: apiKey
slug: uplead-authentication
source_filename: uplead-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://docs.uplead.com/#authentication\nsource: >-\n  https://docs.uplead.com/#authentication, cross-checked against the\n  securitySchemes declared in openapi/uplead-account-api-openapi.yml,\n  openapi/uplead-combined-api-openapi.yml, openapi/uplead-company-api-openapi.yml,\n  openapi/uplead-lists-api-openapi.yml, openapi/uplead-person-api-openapi.yml,\n  openapi/uplead-prospector-api-openapi.yml,\n  openapi/uplead-reference-api-openapi.yml and\n  openapi/uplead-search-api-openapi.yml\nname: UpLead authentication\ndescription: >-\n  UpLead uses a single static API key on every call. The key is placed in the\n  Authorization header and sent bare — \"Authorization: myapikey\" — with no Bearer\n  or other scheme prefix, which is the detail most integrations get wrong. There\n  is no OAuth, no OpenID Connect, no mutual TLS, no signing, no key rotation\n  endpoint, and no scope system: one key carries the account's full plan\n \
  \ entitlement.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_prefix: null\n  description: >-\n    Your UpLead API key passed as the raw value of the Authorization header. The\n    documentation's example is literally `Authorization: myapikey` — replace\n    `myapikey` with your key and add no prefix.\n  required_on: every operation, including getCredits\n  docs: https://docs.uplead.com/#authentication\n  sources:\n  - openapi/uplead-account-api-openapi.yml\n  - openapi/uplead-combined-api-openapi.yml\n  - openapi/uplead-company-api-openapi.yml\n  - openapi/uplead-lists-api-openapi.yml\n  - openapi/uplead-person-api-openapi.yml\n  - openapi/uplead-prospector-api-openapi.yml\n  - openapi/uplead-reference-api-openapi.yml\n  - openapi/uplead-search-api-openapi.yml\n\nkey_management:\n  where: UpLead account settings\n  request_form: https://www.uplead.com/data-api/\n\
  \  request_note: >-\n    The API product page routes an API-key request through a Google Form rather\n    than issuing a key self-serve, so obtaining a key is a human-mediated step\n    even though the documentation is fully public.\n  rotation_endpoint: null\n  expiry: null\n  multiple_keys: not documented\n  revocation: not documented\n  guidance: >-\n    \"Your API key is what identifies your account, so be sure to keep it secret!\n    Please don't share it with anyone outside of your organization.\"\n\nunauthenticated_surface:\n  - operation: getCompanyLogo\n    host: https://logo.uplead.com\n    note: >-\n      The Company Logo API is free and requires no key. Attribution back to\n      uplead.com is required wherever the logo is displayed.\n\nfailure_modes:\n  - status: 401\n    meaning: The key is wrong or missing.\n    note: >-\n      The most common cause is sending \"Authorization: Bearer <key>\" instead of\n      the bare key.\n  - status: 403\n    meaning: The key is valid\
  \ but the account is paused, unsubscribed, or on a plan that does not include this endpoint.\n    note: >-\n      Authorization here is plan-based rather than scope-based. Prospector Pro,\n      Quick Search, Industries and Lists are Professional/Elite/Enterprise only;\n      prospector-preview is reseller-only.\n\ntransport:\n  https_required: true\n  tls: see security/uplead-domain-security.yml\n\nnot_supported:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  - http basic\n  - http bearer\n  - request signing\n  - scopes or granular permissions\n  - service accounts\n  - JWT\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/authentication/uplead-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Lead Generation
- Contact Data
- Company Data
- Email Verification
- Data Enrichment
- Sales Intelligence
---
