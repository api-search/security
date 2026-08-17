---
api_key_in: []
auth_types: []
description: 'Clearbit authenticates with a single long-lived Secret API key scoped to the account, presented either as HTTP Basic (key as the username, empty password) or as an RFC 6750 Bearer token. There is no OAuth 2.0 authorization server, no OIDC discovery document, no scopes and no per-endpoint permission model — every key carries the full entitlement of its account''s plan. Key issuance is now closed: Clearbit''s own help centre states API keys are available only for accounts created in 2023 and earlier, so the authentication surface is live but unobtainable for new integrators.'
kind: authentication
layout: security
method: searched
name: Clearbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clearbit (HubSpot Breeze Intelligence) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clearbit (HubSpot Breeze Intelligence)
provider_slug: clearbit
scheme_count: 2
schemes:
- description: 'API key supplied as the HTTP Basic username with an empty password (Authorization: Basic base64("<api_key>:")).'
  evidence:
    body: '{"error":{"type":"invalid_api_key","message":"Invalid API key provided"}}'
    http_status: 401
    note: A deliberately invalid key produced invalid_api_key rather than auth_required, which proves the Basic credential was parsed and evaluated.
    request: curl -u "<key>:" https://person.clearbit.com/v2/people/find?email=...
  header: Authorization
  in: header
  name: SecretApiKeyBasic
  scheme: basic
  type: http
  verified: probed
- description: 'API key supplied as a bearer token (Authorization: Bearer <api_key>).'
  evidence:
    body: '{"error":{"type":"invalid_api_key","message":"Invalid API key provided"}}'
    http_status: 401
    request: 'curl -H "Authorization: Bearer <key>" https://company.clearbit.com/v2/companies/find?domain=...'
  header: Authorization
  in: header
  name: SecretApiKeyBearer
  scheme: bearer
  type: http
  verified: probed
slug: clearbit-authentication
source_filename: clearbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://help.clearbit.com/hc/en-us/articles/6045527495191-How-Do-I-Access-My-Clearbit-API-Key\n  plus live 401 probes of person/company/reveal/prospector/risk/discovery.clearbit.com on 2026-08-13\ndocs: https://help.clearbit.com/hc/en-us/articles/6045527495191-How-Do-I-Access-My-Clearbit-API-Key\nprovider: Clearbit (HubSpot Breeze Intelligence)\nproviderId: clearbit\ndescription: >-\n  Clearbit authenticates with a single long-lived Secret API key scoped to the account, presented\n  either as HTTP Basic (key as the username, empty password) or as an RFC 6750 Bearer token. There\n  is no OAuth 2.0 authorization server, no OIDC discovery document, no scopes and no per-endpoint\n  permission model — every key carries the full entitlement of its account's plan. Key issuance is\n  now closed: Clearbit's own help centre states API keys are available only for accounts created\n  in 2023 and earlier, so the authentication surface\
  \ is live but unobtainable for new integrators.\nschemes:\n- name: SecretApiKeyBasic\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  description: >-\n    API key supplied as the HTTP Basic username with an empty password\n    (Authorization: Basic base64(\"<api_key>:\")).\n  verified: probed\n  evidence:\n    request: 'curl -u \"<key>:\" https://person.clearbit.com/v2/people/find?email=...'\n    http_status: 401\n    body: '{\"error\":{\"type\":\"invalid_api_key\",\"message\":\"Invalid API key provided\"}}'\n    note: >-\n      A deliberately invalid key produced invalid_api_key rather than auth_required, which proves\n      the Basic credential was parsed and evaluated.\n- name: SecretApiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: 'API key supplied as a bearer token (Authorization: Bearer <api_key>).'\n  verified: probed\n  evidence:\n    request: 'curl -H \"Authorization: Bearer <key>\" https://company.clearbit.com/v2/companies/find?domain=...'\n\
  \    http_status: 401\n    body: '{\"error\":{\"type\":\"invalid_api_key\",\"message\":\"Invalid API key provided\"}}'\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  model: none\n  note: >-\n    No OAuth scopes and no permission scoping of any kind. One account-level secret key grants\n    every endpoint the plan entitles. scopes/ is intentionally not emitted for this provider.\nkey_management:\n  location: Clearbit dashboard - Settings > Keys & Settings\n  visibility: Account Admins only\n  rotation_documented: false\n  issuance_status: closed\n  issuance_note: >-\n    \"API keys are available for Clearbit accounts created in 2023 and earlier. If you signed up in\n    2024, free or paid plans with API keys are not available.\" — help centre, last updated\n    2025-02-16. Free Clearbit accounts were sunset 2025-04-30 and new accounts are not being\n    created.\nunauthenticated_endpoints:\n- name: Autocomplete API\n  base_url: https://autocomplete.clearbit.com\n \
  \ path: /v1/companies/suggest\n  auth: none\n  verified: probed\n  http_status: 200\n  note: >-\n    The only Clearbit endpoint that answers without a credential. Confirmed live 2026-08-13\n    returning a JSON array of {name, domain, logo}; the logo field now returns null (see\n    lifecycle/clearbit-lifecycle.yml).\nfailure_modes:\n- http_status: 401\n  type: auth_required\n  message: Authentication is required for this action. Sign up at https://clearbit.com\n  meaning: No Authorization header presented.\n- http_status: 401\n  type: invalid_api_key\n  message: Invalid API key provided\n  meaning: Authorization header presented but the credential did not resolve to an account.\ntransport:\n  https_required: true\n  hsts: true\n  hsts_max_age: 63072000\n  note: Every API host answered HTTP/2 with strict-transport-security preload on 2026-08-13.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearbit/refs/heads/main/authentication/clearbit-authentication.yml
summary_line: 2 schemes
tags:
- Sales Intelligence
- B2B
- Enrichment
- Reveal
- HubSpot
- Marketing
- Data
- Firmographics
- Lead Enrichment
- Company Data
---
