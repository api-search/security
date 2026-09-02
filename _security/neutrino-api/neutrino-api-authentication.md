---
api_key_in:
- header
- query
- body
api_specs:
- filename: neutrino-api-data-tools-api-openapi.yml
  format: yaml
  label: Neutrino API Data Tools API
  slug: neutrino-api-data-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-data-tools-api-openapi.yml
- filename: neutrino-api-e-commerce-api-openapi.yml
  format: yaml
  label: Neutrino API E Commerce API
  slug: neutrino-api-e-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-e-commerce-api-openapi.yml
- filename: neutrino-api-geolocation-api-openapi.yml
  format: yaml
  label: Neutrino API Geolocation API
  slug: neutrino-api-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-geolocation-api-openapi.yml
- filename: neutrino-api-imaging-api-openapi.yml
  format: yaml
  label: Neutrino API Imaging API
  slug: neutrino-api-imaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-imaging-api-openapi.yml
- filename: neutrino-api-security-and-networking-api-openapi.yml
  format: yaml
  label: Neutrino API Security and Networking API
  slug: neutrino-api-security-and-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-security-and-networking-api-openapi.yml
- filename: neutrino-api-telephony-api-openapi.yml
  format: yaml
  label: Neutrino API Telephony API
  slug: neutrino-api-telephony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-telephony-api-openapi.yml
- filename: neutrino-api-www-api-openapi.yml
  format: yaml
  label: Neutrino API WWW API
  slug: neutrino-api-www-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-www-api-openapi.yml
auth_types:
- apiKey
description: 'Two static API-key credentials sent together on every request: `user-id` identifies the account and `api-key` is one of several rotatable keys issued from the account dashboard. Both are declared in the OpenAPI as header apiKey schemes and the document''s top-level `security` requires BOTH simultaneously. The documentation additionally allows sending them as GET query parameters or POST body fields, and allows collapsing them into a single combined header — neither of which the specification expresses.'
kind: authentication
layout: security
method: searched
name: Neutrino Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neutrino API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neutrino API
provider_slug: neutrino-api
scheme_count: 2
schemes:
- description: Your user ID — the static ID for the account; cannot be changed.
  in: header
  name: user-id
  parameter: user-id
  sources:
  - openapi/neutrino-api-openapi-3.1.json
  - openapi/neutrino-api-swagger-2.0.json
  type: apiKey
- description: One of your API keys, generated from the account dashboard.
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/neutrino-api-openapi-3.1.json
  - openapi/neutrino-api-swagger-2.0.json
  type: apiKey
slug: neutrino-api-authentication
source_filename: neutrino-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: >-\n  https://www.neutrinoapi.com/api/api-basics/ and\n  https://www.neutrinoapi.com/api/best-practice/, reconciled with the\n  securitySchemes in openapi/neutrino-api-openapi-3.1.json and\n  openapi/neutrino-api-swagger-2.0.json, and confirmed with a live\n  unauthenticated request to https://neutrinoapi.net/ip-info on 2026-08-09\n  (HTTP 403, api-error 43).\ndocs: https://www.neutrinoapi.com/api/api-basics/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  - body\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  mfa_on_account: true\ndescription: >-\n  Two static API-key credentials sent together on every request: `user-id`\n  identifies the account and `api-key` is one of several rotatable keys issued\n  from the account dashboard. Both are declared in the OpenAPI as header apiKey\n  schemes and the document's top-level `security` requires BOTH simultaneously.\n  The documentation additionally\
  \ allows sending them as GET query parameters or\n  POST body fields, and allows collapsing them into a single combined header —\n  neither of which the specification expresses.\nschemes:\n- name: user-id\n  type: apiKey\n  in: header\n  parameter: user-id\n  description: Your user ID — the static ID for the account; cannot be changed.\n  sources:\n  - openapi/neutrino-api-openapi-3.1.json\n  - openapi/neutrino-api-swagger-2.0.json\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: One of your API keys, generated from the account dashboard.\n  sources:\n  - openapi/neutrino-api-openapi-3.1.json\n  - openapi/neutrino-api-swagger-2.0.json\ncombined_header:\n  header: API-Key\n  format: '<user-id>:<api-key>'\n  note: >-\n    Documented alternative that carries both credentials in one header. Not\n    expressed in either specification, so generated clients do not use it.\nalternative_locations:\n  - {in: query, note: 'Both values may be sent as GET query parameters\
  \ (user-id, api-key).'}\n  - {in: body, note: 'Both values may be sent as POST form/JSON fields. The batch /multi endpoint takes them in the JSON body.'}\nkey_management:\n  console: https://www.neutrinoapi.com/account/login/\n  multiple_keys: true\n  rotation: Keys are generated and revoked from the account dashboard.\n  endpoint_restriction:\n    supported: true\n    note: >-\n      Keys can be restricted to specific endpoints — the provider's own\n      best-practice guide recommends least-privilege per-key scoping, and\n      separate keys per environment and per application. There is no\n      machine-readable scope vocabulary, so no scopes/ artifact is emitted.\n    docs: https://www.neutrinoapi.com/api/best-practice/\n  self_imposed_quotas:\n    supported: true\n    note: An account holder can set per-key/per-endpoint daily caps; exceeding one returns api-error 31.\n  account_mfa:\n    supported: true\n    mechanism: TOTP, compatible with major authenticator apps and hardware keys.\n\
  \    since: '2022-01-19'\n    note: Protects the dashboard/account, not API calls.\nfailure_mode:\n  http_status: 403\n  api_error: 43\n  message: ACCESS DENIED. USER ID OR API KEY INVALID\n  observed: '2026-08-09'\ngaps:\n  - No OAuth 2.0 or OpenID Connect — there is no delegated/third-party authorization story.\n  - No published key prefix convention, so a leaked key is not identifiable by shape.\n  - Credentials may travel in query strings, which is convenient and lands them in access logs and browser history.\n  - No mutual TLS option for the API hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/authentication/neutrino-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data Validation
- Data Tools
- Telephony
- Communications
- SMS
- Voice
- Geolocation
- IP Intelligence
- Security
- Networking
- Anti-Fraud
- E-Commerce
- Payments
- Imaging
- Rendering
- Currency
- FX
---
