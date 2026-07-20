---
api_key_in: []
api_specs:
- filename: kota-openapi-original.json
  format: json
  label: Kota API
  slug: kota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kota/refs/heads/main/openapi/kota-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kota Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kota secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kota
provider_slug: kota
scheme_count: 1
schemes:
- applied: globally (root-level security requirement in the published spec)
  description: Authorization header using the Bearer scheme
  env_var_convention: KOTA_API_KEY
  header: 'Authorization: Bearer <YOUR_API_SECRET_KEY>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kota-api-reference-openapi.json
  - openapi/kota-openapi-original.json
  type: http
slug: kota-authentication
source_filename: kota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kota-openapi-original.json, openapi/kota-api-reference-openapi.json\ndocs: https://docs.kota.io/core-components/authentication\nreference: https://docs.kota.io/api-reference#authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  model: >-\n    Single-credential bearer API key. No OAuth 2.0, no OpenID Connect, no scope surface — access is\n    bounded by the platform the key belongs to and that platform's type, not by scopes.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authorization header using the Bearer scheme\n  header: 'Authorization: Bearer <YOUR_API_SECRET_KEY>'\n  env_var_convention: KOTA_API_KEY\n  applied: globally (root-level security requirement in the published spec)\n  sources:\n  - openapi/kota-api-reference-openapi.json\n  - openapi/kota-openapi-original.json\nkey_model:\n  prefixes:\n  - prefix: pk_test_\n \
  \   mode: test\n    base_url: https://test.api.kota.io\n  - prefix: pk_live_\n    mode: live\n    base_url: https://api.kota.io\n  scoping: >-\n    API keys are tied to an individual platform and restricted to that platform's type, such as\n    employer_of_record or payroll_provider. Endpoints restricted to specific platform types are\n    noted in the API reference and return 403 forbidden to keys of the wrong type.\n  handling: >-\n    Secret keys must not be shared in publicly accessible areas such as GitHub or client-side code.\n    Browser-side flows use short-lived Embed session tokens from POST /embed/sessions instead.\ntransport:\n  https_required: true\n  note: >-\n    All API requests must be made over HTTPS; calls made over plain HTTP will fail. Requests\n    without authentication also fail.\nbrowser_credentials:\n  mechanism: Embed session access token\n  issued_by: POST /embed/sessions (server-side, with the secret key)\n  scope: bound to a single employer or employee UI\
  \ context\n  docs: https://docs.kota.io/embed/server-side\nauth_errors:\n- status: 401\n  error_code: unauthorized\n  meaning: Authorization header missing or invalid\n- status: 403\n  error_code: forbidden\n  meaning: Token lacks permission for the operation (often a platform-type restriction)\noauth_scopes: none - Kota publishes no OAuth 2.0 or scope surface\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kota/refs/heads/main/authentication/kota-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Insurance
- Employee Benefits
- Health Insurance
- Pensions
- Insurtech
- Embedded Finance
- Human Resources
- Payroll
---
