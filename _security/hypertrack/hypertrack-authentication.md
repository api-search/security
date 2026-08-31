---
api_key_in: []
api_specs:
- filename: hypertrack-authentication-api-openapi.yml
  format: yaml
  label: HyperTrack Authentication API
  slug: hypertrack-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-authentication-api-openapi.yml
- filename: hypertrack-export-api-openapi.yml
  format: yaml
  label: HyperTrack Export API
  slug: hypertrack-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-export-api-openapi.yml
- filename: hypertrack-geotags-api-openapi.yml
  format: yaml
  label: HyperTrack Geotags API
  slug: hypertrack-geotags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-geotags-api-openapi.yml
- filename: hypertrack-nearby-api-openapi.yml
  format: yaml
  label: HyperTrack Nearby API
  slug: hypertrack-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-nearby-api-openapi.yml
- filename: hypertrack-orders-api-openapi.yml
  format: yaml
  label: HyperTrack Orders API
  slug: hypertrack-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-orders-api-openapi.yml
- filename: hypertrack-places-api-openapi.yml
  format: yaml
  label: HyperTrack Places API
  slug: hypertrack-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-places-api-openapi.yml
- filename: hypertrack-tracking-api-openapi.yml
  format: yaml
  label: HyperTrack Tracking API
  slug: hypertrack-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-tracking-api-openapi.yml
- filename: hypertrack-visits-api-openapi.yml
  format: yaml
  label: HyperTrack Visits API
  slug: hypertrack-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-visits-api-openapi.yml
- filename: hypertrack-workerexport-api-openapi.yml
  format: yaml
  label: HyperTrack Worker Export API
  slug: hypertrack-workerexport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-workerexport-api-openapi.yml
- filename: hypertrack-workers-api-openapi.yml
  format: yaml
  label: HyperTrack Workers API
  slug: hypertrack-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-workers-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hypertrack Authentication
name_suffix: Authentication
oauth_flows: []
overview: HyperTrack secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HyperTrack
provider_slug: hypertrack
scheme_count: 3
schemes:
- applies_to: 83 of 85 operations (everything except the two token endpoints)
  credential: base64(AccountID:SecretKey)
  declared_in_spec: true
  header: 'Authorization: Basic <base64(AccountID:SecretKey)>'
  name: BasicAuth
  note: This is the credential HyperTrack's own docs and agent skill use in every server-side example. The SecretKey grants full read AND write access to the whole account; HyperTrack's MCP page warns it should be treated like a password.
  scheme: basic
  sources:
  - openapi/hypertrack-openapi.yaml
  - https://github.com/hypertrack/hypertrack-skills
  type: http
- declared_in_spec: true
  header: 'Authorization: Bearer <access_token>'
  name: TokenAuth
  note: The bearer token issued by POST /oauth/token. Declared as a plain http/bearer scheme rather than as an oauth2 scheme with flows, which is why derive-oauth-scopes.py found no oauth2 flows to read.
  scheme: bearer
  sources:
  - openapi/hypertrack-openapi.yaml
  type: http
- declared_in_spec: true
  name: BearerAuth
  note: A third securityScheme, structurally identical to TokenAuth. The contract declares both and does not explain the difference; treat them as the same bearer credential.
  scheme: bearer
  sources:
  - openapi/hypertrack-openapi.yaml
  type: http
slug: hypertrack-authentication
source_filename: hypertrack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: >-\n  https://hypertrack.com/reference/get-orders, openapi/hypertrack-openapi.yaml,\n  https://github.com/hypertrack/hypertrack-skills (references/backend-api.md),\n  https://hypertrack.com/docs/sdk-config, https://hypertrack.com/docs/mcp-server\ndocs: https://hypertrack.com/docs/build-your-app\nsummary:\n  types: [http, oauth2]\n  primary: HTTP Basic\n  transport_security: TLS 1.3 (probed 2026-08-22)\n  credential_issuance: https://dashboard.hypertrack.com/setup\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  declared_in_spec: true\n  credential: 'base64(AccountID:SecretKey)'\n  header: 'Authorization: Basic <base64(AccountID:SecretKey)>'\n  applies_to: 83 of 85 operations (everything except the two token endpoints)\n  note: >-\n    This is the credential HyperTrack's own docs and agent skill use in every server-side example.\n    The SecretKey grants full read AND write access to the whole account; HyperTrack's\
  \ MCP page\n    warns it should be treated like a password.\n  sources:\n  - openapi/hypertrack-openapi.yaml\n  - https://github.com/hypertrack/hypertrack-skills\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  declared_in_spec: true\n  header: 'Authorization: Bearer <access_token>'\n  note: >-\n    The bearer token issued by POST /oauth/token. Declared as a plain http/bearer scheme rather\n    than as an oauth2 scheme with flows, which is why derive-oauth-scopes.py found no oauth2 flows\n    to read.\n  sources:\n  - openapi/hypertrack-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  declared_in_spec: true\n  note: >-\n    A third securityScheme, structurally identical to TokenAuth. The contract declares both and does\n    not explain the difference; treat them as the same bearer credential.\n  sources:\n  - openapi/hypertrack-openapi.yaml\noauth2:\n  supported: true\n  declared_as_securityscheme: false\n  grant: client_credentials\n  token_endpoint: https://v3.api.hypertrack.com/oauth/token\n\
  \  token_endpoint_operation_id: postOauthToken\n  request_media_type: application/x-www-form-urlencoded\n  request_params:\n    required: [grant_type, client_id, client_secret]\n    optional: [scope]\n  response_fields: [access_token, token_type, expires_in]\n  token_lifetime: short-lived; expires_in returned per token, value not documented as a constant\n  errors:\n    '401': Invalid client credentials.\n    '400': Invalid parameters (missing embed_url or invalid grant_type).\n  scopes:\n    published: false\n    note: >-\n      The token endpoint accepts an optional space-delimited `scope` parameter but HyperTrack\n      publishes no scope names and no securityScheme declares scopes. No scopes/ artifact is\n      written, because deriving one would mean inventing scope strings.\nembed_tokens:\n  operation: POST /oauth/embed-token\n  operation_id: postOauthEmbedToken\n  summary: Secure embed view\n  purpose: Mints a scoped token authorising an embedded HyperTrack Ops view for a given\
  \ embed_url.\n  see: components/hypertrack-components.yml\nmobile_sdk_credential:\n  name: Publishable Key\n  where: AndroidManifest / Info.plist, key HyperTrackPublishableKey\n  docs: https://hypertrack.com/docs/sdk-config\n  note: >-\n    A distinct credential from the server-side SecretKey, shipped inside the customer's mobile app.\n    Confusing the two is the most likely credential mistake in a HyperTrack integration, so it is\n    recorded here explicitly.\nmcp_credential:\n  env: [HYPERTRACK_ACCOUNT_ID, HYPERTRACK_SECRET_KEY]\n  note: >-\n    The MCP server reuses the same AccountID/SecretKey pair. There is no scoped or read-only\n    credential to hand an agent — the read-only guarantee comes from the server's tool set, not\n    from the key. See mcp/hypertrack-mcp.yml.\nunauthenticated_surface:\n- operation: GET /tracking/{tracking_id}\n  note: The public order-tracking view; the only data operation in the contract with no security requirement.\n- operation: POST /oauth/token\n\
  - operation: POST /oauth/embed-token\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/authentication/hypertrack-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Location
- Geolocation
- Tracking
- Logistics
- Last Mile Delivery
- Field Service
- Workforce
- Time and Attendance
- Mobile SDK
- Geofencing
- Routing
---
