---
api_key_in:
- header
api_specs:
- filename: simpleanalytics-events-api-openapi.yml
  format: yaml
  label: Simple Analytics Events API
  slug: simpleanalytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-events-api-openapi.yml
- filename: simpleanalytics-export-api-openapi.yml
  format: yaml
  label: Simple Analytics Export API
  slug: simpleanalytics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-export-api-openapi.yml
- filename: simpleanalytics-stats-api-openapi.yml
  format: yaml
  label: Simple Analytics Stats API
  slug: simpleanalytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-stats-api-openapi.yml
- filename: simpleanalytics-websites-api-openapi.yml
  format: yaml
  label: Simple Analytics Websites API
  slug: simpleanalytics-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-websites-api-openapi.yml
auth_types:
- apiKey
description: 'Simple Analytics authenticates with a pair of custom headers, not a bearer token. There is no OAuth, no OIDC, no token exchange and no refresh — an Api-Key identifies the account and a User-Id identifies the principal, and Admin API calls need both. Two surfaces need no credential at all: public websites on the read APIs, and the server-side event collection endpoint.'
kind: authentication
layout: security
method: searched
name: Simpleanalytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simple Analytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Simple Analytics
provider_slug: simpleanalytics
scheme_count: 2
schemes:
- description: Account API key created in account settings. Required for the Admin API and for the Stats and Export APIs when the website is private.
  example_shape: sa_api_key_ followed by an opaque token
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  prefix: sa_api_key_
  sources:
  - https://docs.simpleanalytics.com/api/authenticate
  - openapi/simpleanalytics-events-api-openapi.yml
  - openapi/simpleanalytics-export-api-openapi.yml
  - openapi/simpleanalytics-stats-api-openapi.yml
  - openapi/simpleanalytics-websites-api-openapi.yml
  type: apiKey
- description: User identifier shown in account settings. Required alongside Api-Key on Admin API calls; a non-UUIDv4 value returns HTTP 400 "Invalid user id format, it should be a UUIDv4".
  format: sa_user_id_ + UUIDv4
  in: header
  name: UserId
  parameter: User-Id
  prefix: sa_user_id_
  sources:
  - https://docs.simpleanalytics.com/api/authenticate
  - https://docs.simpleanalytics.com/api/admin
  - openapi/simpleanalytics-events-api-openapi.yml
  - openapi/simpleanalytics-export-api-openapi.yml
  - openapi/simpleanalytics-stats-api-openapi.yml
  - openapi/simpleanalytics-websites-api-openapi.yml
  type: apiKey
slug: simpleanalytics-authentication
source_filename: simpleanalytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://docs.simpleanalytics.com/api/authenticate\nsource: >-\n  https://docs.simpleanalytics.com/api/authenticate,\n  https://docs.simpleanalytics.com/api/stats,\n  https://docs.simpleanalytics.com/api/admin,\n  https://docs.simpleanalytics.com/events/server-side, derived baseline from\n  openapi/simpleanalytics-events-api-openapi.yml,\n  openapi/simpleanalytics-export-api-openapi.yml,\n  openapi/simpleanalytics-stats-api-openapi.yml,\n  openapi/simpleanalytics-websites-api-openapi.yml, plus live probes of\n  https://simpleanalytics.com 2026-08-13\ndescription: >-\n  Simple Analytics authenticates with a pair of custom headers, not a bearer\n  token. There is no OAuth, no OIDC, no token exchange and no refresh — an\n  Api-Key identifies the account and a User-Id identifies the principal, and\n  Admin API calls need both. Two surfaces need no credential at all: public\n  websites on the read APIs, and the server-side event collection\
  \ endpoint.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  bearer: false\n  rotation_documented: false\n  scopes: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  prefix: sa_api_key_\n  description: >-\n    Account API key created in account settings. Required for the Admin API and\n    for the Stats and Export APIs when the website is private.\n  example_shape: sa_api_key_ followed by an opaque token\n  sources:\n  - https://docs.simpleanalytics.com/api/authenticate\n  - openapi/simpleanalytics-events-api-openapi.yml\n  - openapi/simpleanalytics-export-api-openapi.yml\n  - openapi/simpleanalytics-stats-api-openapi.yml\n  - openapi/simpleanalytics-websites-api-openapi.yml\n- name: UserId\n  type: apiKey\n  in: header\n  parameter: User-Id\n  prefix: sa_user_id_\n  format: sa_user_id_ + UUIDv4\n  description: >-\n    User identifier shown in account settings. Required\
  \ alongside Api-Key on\n    Admin API calls; a non-UUIDv4 value returns HTTP 400 \"Invalid user id\n    format, it should be a UUIDv4\".\n  sources:\n  - https://docs.simpleanalytics.com/api/authenticate\n  - https://docs.simpleanalytics.com/api/admin\n  - openapi/simpleanalytics-events-api-openapi.yml\n  - openapi/simpleanalytics-export-api-openapi.yml\n  - openapi/simpleanalytics-stats-api-openapi.yml\n  - openapi/simpleanalytics-websites-api-openapi.yml\nrequirements_by_operation:\n- operation: getStats\n  required:\n  - Api-Key\n  conditional: true\n  note: Public websites answer with no credentials; private websites require Api-Key.\n- operation: exportDataPoints\n  required:\n  - Api-Key\n  conditional: true\n  note: >-\n    Verified answering anonymously for a public hostname on 2026-08-13. Private\n    hostnames require Api-Key and a Business or Enterprise plan.\n- operation: listWebsites\n  required:\n  - Api-Key\n  - User-Id\n  conditional: false\n- operation: addWebsite\n  required:\n\
  \  - Api-Key\n  - User-Id\n  conditional: false\n  note: Also requires a Business or Enterprise plan; calling it auto-upgrades the account.\n- operation: collectEvent\n  required: []\n  conditional: false\n  note: >-\n    queue.simpleanalyticscdn.com/events accepts unauthenticated POSTs — the\n    hostname in the payload is the routing key. There is no write credential.\nexample_request: |\n  curl \"https://simpleanalytics.com/api/websites\" \\\n    -H 'Content-Type: application/json' \\\n    -H 'Api-Key: sa_api_key_REDACTED_EXAMPLE' \\\n    -H 'User-Id: sa_user_id_00000000-0000-0000-0000-000000000000'\nfailure_modes:\n  note: >-\n    Authentication failures return HTTP 400, not 401 — an agent's standard\n    \"401 means re-auth\" heuristic will not fire here. Probed 2026-08-13.\n  observed:\n  - status: 400\n    body: '{\"success\": false, \"error\": \"No Api-Key found, specify via header\"}'\n  - status: 400\n    body: '{\"success\": false, \"error\": \"No User-Id defined\"}'\n  - status:\
  \ 400\n    body: '{\"success\": false, \"error\": \"Invalid user id format, it should be a UUIDv4\"}'\n  artifact: errors/simpleanalytics-problem-types.yml\nkey_management:\n  create: Account settings in the dashboard\n  rotate: Not documented\n  revoke: Not documented\n  expiry: No documented TTL\n  scopes: None — a key is all-or-nothing for the account\n  note: >-\n    No scoping, rotation or expiry story is published, so a leaked Api-Key plus\n    User-Id grants full account read and the ability to add billable websites\n    until it is manually replaced.\ndashboard_sso:\n  note: >-\n    Okta and Microsoft Entra SAML SSO are available for dashboard sign-in\n    (docs.simpleanalytics.com/okta-saml-sso, /microsoft-entra-saml-sso). This\n    governs human login only; it issues no API credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/authentication/simpleanalytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
- Events
- Data Export
- Europe
---
