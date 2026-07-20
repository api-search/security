---
api_key_in: []
api_specs:
- filename: boltz-compute.yml
  format: yaml
  label: Boltz Compute API
  slug: boltz-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltz/refs/heads/main/openapi/boltz-compute.yml
auth_types: []
description: 'Authentication profile for the Boltz Compute API. Bearer-token auth: either a Boltz API key or an OAuth bearer token in the Authorization header. OAuth callers scope requests to an organization with the X-Boltz-Organization-Id header. API keys carry a mode (test vs live).'
kind: authentication
layout: security
method: searched
name: Boltz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boltz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Boltz
provider_slug: boltz
scheme_count: 1
schemes:
- credential_types:
  - api_key
  - oauth_bearer
  env_var: BOLTZ_API_KEY
  format: 'Authorization: Bearer <token>'
  header: Authorization
  id: bearerAuth
  location: header
  notes: SDKs default the key from the BOLTZ_API_KEY environment variable. API keys are managed under the Admin API (create/list/revoke).
  scheme: bearer
  type: http
slug: boltz-authentication
source_filename: boltz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://github.com/boltz-bio/boltz-api-go (auth.go, client.go, README) and\n  https://boltz.bio/api. Confirmed against the official SDKs.\ndescription: >-\n  Authentication profile for the Boltz Compute API. Bearer-token auth: either a\n  Boltz API key or an OAuth bearer token in the Authorization header. OAuth\n  callers scope requests to an organization with the X-Boltz-Organization-Id\n  header. API keys carry a mode (test vs live).\nbase_url: https://api.boltz.bio\nschemes:\n  - id: bearerAuth\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: 'Authorization: Bearer <token>'\n    credential_types:\n      - api_key   # created via POST /compute/v1/admin/api-keys; has a mode (test|live)\n      - oauth_bearer  # user/OAuth session tokens\n    env_var: BOLTZ_API_KEY\n    notes: >-\n      SDKs default the key from the BOLTZ_API_KEY environment variable. API keys\n      are\
  \ managed under the Admin API (create/list/revoke).\nsupplemental_headers:\n  - name: X-Boltz-Organization-Id\n    purpose: OAuth callers select which organization membership the request runs under.\nidentity_endpoint: /compute/v1/auth/me\nkey_management:\n  create: POST /compute/v1/admin/api-keys\n  list: GET /compute/v1/admin/api-keys\n  revoke: POST /compute/v1/admin/api-keys/{api_key_id}/revoke\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltz/refs/heads/main/authentication/boltz-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Digital Biology
- Drug Discovery
- Artificial Intelligence
- Machine Learning
- Protein Design
- Structure Prediction
- Life Sciences
- Compute
---
