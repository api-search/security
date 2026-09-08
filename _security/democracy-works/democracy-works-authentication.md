---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: democracy-works-authorities-api-openapi.yml
  format: yaml
  label: Democracy Works Authorities API
  slug: democracy-works-authorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-authorities-api-openapi.yml
- filename: democracy-works-elections-api-openapi.yml
  format: yaml
  label: Democracy Works Elections API
  slug: democracy-works-elections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-elections-api-openapi.yml
- filename: democracy-works-exports-api-openapi.yml
  format: yaml
  label: Democracy Works Exports API
  slug: democracy-works-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-exports-api-openapi.yml
- filename: democracy-works-ballot-measures-api-openapi.yml
  format: yaml
  label: Democracy Works Ballot Measures API
  slug: democracy-works-ballot-measures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-ballot-measures-api-openapi.yml
- filename: democracy-works-candidates-api-openapi.yml
  format: yaml
  label: Democracy Works Candidates API
  slug: democracy-works-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-candidates-api-openapi.yml
- filename: democracy-works-contests-api-openapi.yml
  format: yaml
  label: Democracy Works Contests API
  slug: democracy-works-contests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-contests-api-openapi.yml
- filename: democracy-works-endorsements-api-openapi.yml
  format: yaml
  label: Democracy Works Endorsements API
  slug: democracy-works-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-endorsements-api-openapi.yml
- filename: democracy-works-voting-locations-api-openapi.yml
  format: yaml
  label: Democracy Works Voting Locations API
  slug: democracy-works-voting-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-voting-locations-api-openapi.yml
- filename: democracy-works-elections-v1-api-openapi.yml
  format: yaml
  label: Democracy Works Elections API v1 (legacy)
  slug: democracy-works-elections-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-elections-v1-api-openapi.yml
auth_types:
- apiKey
description: A single API-key header, no OAuth, no scopes, and no self-service issuance. Note that the two live generations of this API use DIFFERENT auth headers — the v1 surface, still served, uses an Authorization header with an "apikey" prefix.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Democracy Works Authentication
name_suffix: Authentication
oauth_flows: []
overview: Democracy Works secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Democracy Works
provider_slug: democracy-works
scheme_count: 2
schemes:
- applies_to: API v2 (https://api.democracy.works/v2) — all 11 operations
  example: 'curl "https://api.democracy.works/v2/elections" --header "X-API-KEY: <YOUR API KEY>"'
  in: header
  name: ApiKeyAuth
  note: The contract's prose writes the header as "X-API-Key" and its curl example as "X-API-KEY"; HTTP header names are case-insensitive so either is accepted. The catalog's refined specs were normalized to the published curl form.
  parameter: X-API-KEY
  sources:
  - openapi/democracy-works-authorities-api-openapi.yml
  - openapi/democracy-works-ballot-measures-api-openapi.yml
  - openapi/democracy-works-candidates-api-openapi.yml
  - openapi/democracy-works-contests-api-openapi.yml
  - openapi/democracy-works-elections-api-openapi.yml
  - openapi/democracy-works-endorsements-api-openapi.yml
  - openapi/democracy-works-exports-api-openapi.yml
  - openapi/democracy-works-voting-locations-api-openapi.yml
  type: apiKey
- applies_to: API v1 (https://api.democracy.works, unversioned paths) — legacy, still live
  example: 'curl -H "Accept: application/json" -H "Authorization: apikey $YOUR_API_KEY" "https://api.democracy.works/elections/upcoming"'
  in: header
  name: AuthorizationApiKey
  note: Documented at https://developers.democracy.works/api/v1, which is also what the portal root serves. The v1 contract declares no securityScheme object — the header is described only in prose and as a request parameter on the upcoming-elections operation.
  parameter: Authorization
  sources:
  - openapi/democracy-works-elections-v1-api-openapi.yml
  type: apiKey
  value_format: apikey <YOUR_API_KEY>
slug: democracy-works-authentication
source_filename: democracy-works-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Democracy Works\nproviderId: democracy-works\ngenerated: '2026-09-07'\nmethod: searched\ndocs: https://developers.democracy.works/api/v2#section/Introduction/Authentication\nsource: >-\n  Derived from the securitySchemes of the eight refined OpenAPI documents in openapi/, then\n  upgraded from the provider's own authentication section at\n  https://developers.democracy.works/api/v2 and a live probe of\n  https://api.democracy.works/v2/elections on 2026-09-07\ndescription: >-\n  A single API-key header, no OAuth, no scopes, and no self-service issuance. Note that the\n  two live generations of this API use DIFFERENT auth headers — the v1 surface, still\n  served, uses an Authorization header with an \"apikey\" prefix.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  scopes: false\n  mtls: false\n  openid_connect: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: X-API-KEY\n  applies_to: 'API v2 (https://api.democracy.works/v2) — all 11 operations'\n  example: 'curl \"https://api.democracy.works/v2/elections\" --header \"X-API-KEY: <YOUR API KEY>\"'\n  sources:\n  - openapi/democracy-works-authorities-api-openapi.yml\n  - openapi/democracy-works-ballot-measures-api-openapi.yml\n  - openapi/democracy-works-candidates-api-openapi.yml\n  - openapi/democracy-works-contests-api-openapi.yml\n  - openapi/democracy-works-elections-api-openapi.yml\n  - openapi/democracy-works-endorsements-api-openapi.yml\n  - openapi/democracy-works-exports-api-openapi.yml\n  - openapi/democracy-works-voting-locations-api-openapi.yml\n  note: >-\n    The contract's prose writes the header as \"X-API-Key\" and its curl example as\n    \"X-API-KEY\"; HTTP header names are case-insensitive so either is accepted. The\n    catalog's refined specs were normalized to the published curl form.\n- name: AuthorizationApiKey\n  type: apiKey\n  in: header\n\
  \  parameter: Authorization\n  value_format: 'apikey <YOUR_API_KEY>'\n  applies_to: 'API v1 (https://api.democracy.works, unversioned paths) — legacy, still live'\n  example: 'curl -H \"Accept: application/json\" -H \"Authorization: apikey $YOUR_API_KEY\" \"https://api.democracy.works/elections/upcoming\"'\n  sources:\n  - openapi/democracy-works-elections-v1-api-openapi.yml\n  note: >-\n    Documented at https://developers.democracy.works/api/v1, which is also what the portal\n    root serves. The v1 contract declares no securityScheme object — the header is described\n    only in prose and as a request parameter on the upcoming-elections operation.\nissuance:\n  self_service: false\n  signup_url: null\n  process: >-\n    Keys are issued by Democracy Works after a partnership conversation. The contract points\n    at https://data.democracy.works/api-signup, which now soft-404s to the marketing\n    homepage; the working routes are partnerships@democracy.works and\n    https://www.democracy.works/contact.\n\
  \  test_key: >-\n    A test key is available on the same request path. There is no separate sandbox host and\n    no key prefix distinguishing test from live. See sandbox/democracy-works-sandbox.yml.\nobserved_behavior:\n- url: https://api.democracy.works/v2/elections\n  request: no credential\n  status: 403\n  body: '{\"message\":\"Forbidden\"}'\n  headers_of_note: 'x-amzn-errortype: ForbiddenException'\n  probed: '2026-09-07'\n- url: https://api.democracy.works/v2/elections\n  request: 'X-API-KEY: not-a-real-key'\n  status: 403\n  body: '{\"message\":\"Forbidden\"}'\n  probed: '2026-09-07'\n  note: >-\n    An invalid key and an absent key are indistinguishable — same status, same body. A\n    client cannot tell \"I forgot the header\" from \"my key was revoked\" without out-of-band\n    information.\n- url: https://api.democracy.works/elections/upcoming\n  request: no credential\n  status: 403\n  body: '{:message \"Missing Authorization apikey header\"}'\n  content_type: application/edn\n\
  \  probed: '2026-09-07'\n  note: >-\n    The v1 surface DOES name the missing header, and answers in EDN rather than JSON.\ntransport:\n  https_only: true\n  tls: TLSv1.3\n  hsts: false\n  note: >-\n    api.democracy.works serves TLS 1.3 but sends no Strict-Transport-Security header on the\n    v2 surface; the v1 surface does (max-age=31536000; includeSubdomains). See\n    security/democracy-works-domain-security.yml.\ngaps:\n- No key rotation, expiry or scoping documented.\n- No per-key permission model — one key grants the whole surface.\n- No OAuth or delegated-authorization path, so an agent cannot act on a voter's behalf with\n  a scoped, revocable grant; it holds a full-surface key.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/authentication/democracy-works-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Civic Tech
- Elections
- Government
- Non-Profit
- Voter Information
- Voting
---
