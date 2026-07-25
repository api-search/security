---
api_key_in: []
api_specs:
- filename: leap-create-meters-api-openapi.yml
  format: yaml
  label: Leap create meters API
  slug: leap-create-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-create-meters-api-openapi.yml
- filename: leap-group-dispatches-api-openapi.yml
  format: yaml
  label: Leap group-dispatches API
  slug: leap-group-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-group-dispatches-api-openapi.yml
- filename: leap-meter-details-api-openapi.yml
  format: yaml
  label: Leap Meter Details API
  slug: leap-meter-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meter-details-api-openapi.yml
- filename: leap-meter-dispatches-api-openapi.yml
  format: yaml
  label: Leap meter-dispatches API
  slug: leap-meter-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meter-dispatches-api-openapi.yml
- filename: leap-meter-enrollment-api-openapi.yml
  format: yaml
  label: Leap meter enrollment API
  slug: leap-meter-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meter-enrollment-api-openapi.yml
- filename: leap-nominations-api-openapi.yml
  format: yaml
  label: Leap nominations API
  slug: leap-nominations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-nominations-api-openapi.yml
- filename: leap-performance-api-openapi.yml
  format: yaml
  label: Leap performance API
  slug: leap-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-performance-api-openapi.yml
- filename: leap-provisional-assets-api-openapi.yml
  format: yaml
  label: Leap provisional assets API
  slug: leap-provisional-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-provisional-assets-api-openapi.yml
- filename: leap-revenue-api-openapi.yml
  format: yaml
  label: Leap revenue API
  slug: leap-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-revenue-api-openapi.yml
- filename: leap-webhooks-api-openapi.yml
  format: yaml
  label: Leap webhooks API
  slug: leap-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Leap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leap
provider_slug: leap
scheme_count: 1
schemes:
- bearer_format: opaque partner API key (the Dispatch, Revenue and Webhook specs declare bearerFormat JWT; the documented partner key is an opaque two-part string)
  header: 'Authorization: Bearer <API_KEY>'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/leap-create-meters-openapi-original.yml
  - openapi/leap-dispatching-openapi-original.yml
  - openapi/leap-enrollments-openapi-original.yml
  - openapi/leap-meters-openapi-original.yml
  - openapi/leap-nominations-openapi-original.yml
  - openapi/leap-settlement-openapi-original.yml
  - openapi/leap-webhooks-openapi-original.yml
  type: http
slug: leap-authentication
source_filename: leap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.leap.energy/docs/api-key-authentication\ndocs: https://developer.leap.energy/docs/api-key-authentication\nsummary:\n  model: bearer-api-key\n  types:\n  - http\n  notes: Every request to a Leap API endpoint must carry a valid bearer token in the HTTP Authorization\n    header. Tokens are long-lived partner API keys created in the Partner Portal, not OAuth access tokens\n    — there is no OAuth 2.0 authorization server, no scope grant flow and no token endpoint. API keys\n    are scoped to a single environment (production or staging) and carry a permission set selected at\n    creation time.\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <API_KEY>'\n  bearer_format: opaque partner API key (the Dispatch, Revenue and Webhook specs declare bearerFormat\n    JWT; the documented partner key is an opaque two-part string)\n  sources:\n  - openapi/leap-create-meters-openapi-original.yml\n\
  \  - openapi/leap-dispatching-openapi-original.yml\n  - openapi/leap-enrollments-openapi-original.yml\n  - openapi/leap-meters-openapi-original.yml\n  - openapi/leap-nominations-openapi-original.yml\n  - openapi/leap-settlement-openapi-original.yml\n  - openapi/leap-webhooks-openapi-original.yml\ncredentials:\n  issuance: Self-service in the Leap Partner Portal Partner Account page, API keys tab. Keys are created\n    with a selected permission set.\n  management_urls:\n    production: https://partner.leap.energy/account?settings=apiKeys\n    staging: https://partner.staging.leap.energy/account?settings=apiKeys\n  environment_scoped: true\n  environment_note: API keys are issued separately for production and staging. A key used against the\n    wrong environment returns 403. The same portal user credentials work in both environments.\n  permissions: Selected per key at creation time in the Partner Account page. Portal user roles are 'Manager'\n    (full admin, including inviting users\
  \ and creating/revoking API keys) and 'User' (no account settings\n    access).\n  rotation: Keys can be created and revoked at any time from the Partner Account page; no published expiry\n    or automatic rotation policy.\nbrowser_sso:\n  supported: true\n  note: The developer portal has SSO with the Partner Portal. Logging in populates a temporary bearer\n    token into the CREDENTIALS box on API Reference pages so calls can be made directly from the browser\n    against staging or production.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes_artifact: none — Leap publishes no OAuth scope surface; permissions are selected per API key in\n  the portal.\nfailure_modes:\n- status: 401\n  meaning: Missing or malformed Authorization header.\n- status: 403\n  meaning: Invalid key, key issued for the other environment, or key lacking the permission for the endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/authentication/leap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Electricity
- Virtual Power Plant
- Demand Response
- Distributed Energy Resources
- Grid Services
- Energy Markets
- Battery Storage
- EV Charging
- Smart Buildings
- Metering
- Webhooks
- Climate Tech
---
