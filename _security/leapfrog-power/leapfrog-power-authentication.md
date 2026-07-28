---
api_key_in:
- header
api_specs:
- filename: leapfrog-power-create-meters-openapi.yml
  format: yaml
  label: Leap Create Meters API
  slug: leapfrog-power-create-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-create-meters-openapi.yml
- filename: leapfrog-power-meter-enrollment-openapi.yml
  format: yaml
  label: Leap Meter Enrollment API
  slug: leapfrog-power-meter-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-enrollment-openapi.yml
- filename: leapfrog-power-meter-details-openapi.yml
  format: yaml
  label: Leap Meter Details API
  slug: leapfrog-power-meter-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-details-openapi.yml
- filename: leapfrog-power-nominations-openapi.yml
  format: yaml
  label: Leap Meter Nomination API
  slug: leapfrog-power-nominations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-nominations-openapi.yml
- filename: leapfrog-power-dispatch-openapi.yml
  format: yaml
  label: Leap Dispatch API
  slug: leapfrog-power-dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-dispatch-openapi.yml
- filename: leapfrog-power-webhooks-openapi.yml
  format: yaml
  label: Leap Webhook Subscription API
  slug: leapfrog-power-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-webhooks-openapi.yml
- filename: leapfrog-power-revenue-analytics-openapi.yml
  format: yaml
  label: Leap Revenue and Analytics API
  slug: leapfrog-power-revenue-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-revenue-analytics-openapi.yml
- filename: leapfrog-power-interval-data-upload-openapi.json
  format: json
  label: Leap Interval Data Upload API
  slug: leapfrog-power-interval-data-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-interval-data-upload-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Leapfrog Power Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leap secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Leap
provider_slug: leapfrog-power
scheme_count: 2
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/leapfrog-power-create-meters-openapi.yml
  - openapi/leapfrog-power-meter-details-openapi.yml
  - openapi/leapfrog-power-meter-enrollment-openapi.yml
  - openapi/leapfrog-power-nominations-openapi.yml
  - openapi/leapfrog-power-revenue-analytics-openapi.yml
  type: http
- bearerFormat: JWT
  name: http
  note: The same credential declared under a second scheme name. Four definitions declare bearerFormat JWT (dispatch, webhooks, interval data, revenue) and four declare no format — a naming inconsistency across teams, not two credentials.
  scheme: bearer
  sources:
  - openapi/leapfrog-power-dispatch-openapi.yml
  - openapi/leapfrog-power-webhooks-openapi.yml
  - openapi/leapfrog-power-interval-data-upload-openapi.json
  type: http
slug: leapfrog-power-authentication
source_filename: leapfrog-power-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\ndocs: https://developer.leap.energy/docs/api-key-authentication\nsource: https://developer.leap.energy/docs/api-key-authentication, https://developer.leap.energy/docs/getting-started,\n  openapi/leapfrog-power-create-meters-openapi.yml, openapi/leapfrog-power-dispatch-openapi.yml,\n  openapi/leapfrog-power-interval-data-upload-openapi.json, openapi/leapfrog-power-meter-details-openapi.yml,\n  openapi/leapfrog-power-meter-enrollment-openapi.yml, openapi/leapfrog-power-nominations-openapi.yml,\n  openapi/leapfrog-power-revenue-analytics-openapi.yml, openapi/leapfrog-power-webhooks-openapi.yml\nsummary:\n  types:\n  - http\n  schemes:\n  - bearer\n  api_key_in:\n  - header\n  oauth2: false\n  oidc: false\n  mtls: false\nmodel: >-\n  A single authentication model across all eight services: an opaque, long-lived API key presented\n  as an HTTP bearer token. Keys are created by a partner admin inside the Leap Partner Portal with\n  per-key\
  \ permissions selected at creation time; they cannot be self-issued, because the partner\n  account itself is provisioned by Leap. Keys are scoped to exactly one environment — a staging key\n  used against production (or the reverse) returns 403.\nheader: 'Authorization: Bearer <API_KEY>'\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/leapfrog-power-create-meters-openapi.yml\n  - openapi/leapfrog-power-meter-details-openapi.yml\n  - openapi/leapfrog-power-meter-enrollment-openapi.yml\n  - openapi/leapfrog-power-nominations-openapi.yml\n  - openapi/leapfrog-power-revenue-analytics-openapi.yml\n- name: http\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/leapfrog-power-dispatch-openapi.yml\n  - openapi/leapfrog-power-webhooks-openapi.yml\n  - openapi/leapfrog-power-interval-data-upload-openapi.json\n  note: >-\n    The same credential declared under a second scheme name. Four definitions declare bearerFormat\n    JWT (dispatch,\
  \ webhooks, interval data, revenue) and four declare no format — a naming\n    inconsistency across teams, not two credentials.\nkey_issuance:\n  self_serve: false\n  provisioning: >-\n    Leap creates the partner account; initial admin users are then invited to create their\n    credentials. Prospective partners are directed to their Leap account manager or partners@leap.ac.\n  portal_urls:\n  - environment: production\n    url: https://partner.leap.energy/account?settings=apiKeys\n  - environment: staging\n    url: https://partner.staging.leap.energy/account?settings=apiKeys\n  roles:\n  - name: Manager\n    capability: full admin access, including inviting/deleting users and creating/revoking API keys\n  - name: User\n    capability: cannot manage account settings\n  user_note: A user invited in the production Partner Account page automatically gains staging access.\npermissions:\n  model: per-key permission selection at creation time\n  evidence: >-\n    The Getting Started guide shows\
  \ a decoded example JWT payload carrying user_id, account_id, an\n    expiration_date and a permissions array. The example permissions are RegisterMeter, GetMeter,\n    DeleteMeter, PlaceBid and GetBid.\n  documented_values: [RegisterMeter, GetMeter, DeleteMeter, PlaceBid, GetBid]\n  caveat: >-\n    Those five come from a single illustrative example payload, not from a published permissions\n    reference. Leap publishes no scope or permission catalog on its anonymous surface, and no\n    OpenAPI operation declares a required permission, so a complete permission list cannot be\n    recorded. No scopes/ artifact is emitted — this is key-based auth, not OAuth.\nenvironments:\n- name: production\n  base_url: https://api.leap.energy\n- name: staging\n  base_url: https://api.staging.leap.energy\nenvironment_mismatch: 403\nbrowser_auth:\n  sso: >-\n    The developer portal has SSO integration with the Partner Portal. Logging in auto-populates a\n    temporary bearer token in the CREDENTIALS\
  \ box of the API reference pages so calls can be made\n    from the browser against staging or production. This is a documentation convenience, not a\n    documented OAuth surface.\ngaps:\n- No OAuth 2.0, OpenID Connect or mTLS option; no /.well-known/openid-configuration and no\n  /.well-known/oauth-authorization-server (404 on all four Leap hosts).\n- No documented key rotation policy, key expiry policy or WWW-Authenticate challenge.\n- The Interval Data Upload definition declares the bearer securityScheme but sets no top-level\n  security requirement, so the spec never states that its operations are protected — a governance\n  gap in the specification, not in the service.\n- Webhook deliveries are authenticated only by a partner-supplied static header; Leap publishes no\n  signature scheme (see conventions/leapfrog-power-conventions.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/authentication/leapfrog-power-authentication.yml
summary_line: http · 2 schemes
tags:
- Energy
- United States
- Electricity
- Grid
- Demand Response
- DER
- Virtual Power Plant
- Energy Markets
- Storage Flexibility
- EV Charging
- Smart Metering
---
