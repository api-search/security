---
api_key_in: []
api_specs:
- filename: ribbon-health-cost-estimates-api-openapi.yml
  format: yaml
  label: Ribbon Health Cost Estimates API
  slug: ribbon-health-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-cost-estimates-api-openapi.yml
- filename: ribbon-health-filters-api-openapi.yml
  format: yaml
  label: Ribbon Health Filters API
  slug: ribbon-health-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-filters-api-openapi.yml
- filename: ribbon-health-focus-area-endpoints-api-openapi.yml
  format: yaml
  label: Ribbon Health Focus Area Endpoints API
  slug: ribbon-health-focus-area-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-focus-area-endpoints-api-openapi.yml
- filename: ribbon-health-locations-api-openapi.yml
  format: yaml
  label: Ribbon Health Locations API
  slug: ribbon-health-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-locations-api-openapi.yml
- filename: ribbon-health-networks-api-openapi.yml
  format: yaml
  label: Ribbon Health Networks API
  slug: ribbon-health-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-networks-api-openapi.yml
- filename: ribbon-health-organizations-api-openapi.yml
  format: yaml
  label: Ribbon Health Organizations API
  slug: ribbon-health-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-organizations-api-openapi.yml
- filename: ribbon-health-price-transparency-api-openapi.yml
  format: yaml
  label: Ribbon Health Price Transparency API
  slug: ribbon-health-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-price-transparency-api-openapi.yml
- filename: ribbon-health-providers-api-openapi.yml
  format: yaml
  label: Ribbon Health Providers API
  slug: ribbon-health-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-providers-api-openapi.yml
- filename: ribbon-health-reference-endpoints-api-openapi.yml
  format: yaml
  label: Ribbon Health Reference Endpoints API
  slug: ribbon-health-reference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-reference-endpoints-api-openapi.yml
- filename: ribbon-health-tins-api-openapi.yml
  format: yaml
  label: Ribbon Health TINs API
  slug: ribbon-health-tins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-tins-api-openapi.yml
- filename: ribbon-health-price-transparency-v2-api-openapi.yml
  format: yaml
  label: Ribbon Health Price Transparency v2 API
  slug: ribbon-health-price-transparency-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-price-transparency-v2-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ribbon Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ribbon Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ribbon Health
provider_slug: ribbon-health
scheme_count: 1
schemes:
- credential: single long-lived customer API key
  docs: https://ribbon.readme.io/docs/authentication
  header: 'Authorization: Bearer {customer_token}'
  issuance: Keys are issued through a sales/demo engagement at https://h1.co/request-demo/ — there is no self-serve key generation, no developer signup, and no key-management endpoint in the API.
  name: BearerAuth
  provider_guidance: '"Make sure to keep this API Key secure. Do not share your API Key in publicly accessible areas, such as Github, client-side code, or internal communication tools."'
  rotation_documented: false
  scheme: bearer
  sources:
  - openapi/ribbon-health-h1-api-openapi.yml
  test_credentials: false
  test_credentials_note: 'No sandbox, no test mode and no separate test key prefix are documented, which is why there is no sandbox/ artifact in this repo. The only mode-like distinction is entitlement: the spec''s own 403 example is "Trial accounts do not have access to custom specialties", so trial accounts exist but share the same production host and key format.'
  type: http
slug: ribbon-health-authentication
source_filename: ribbon-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/ribbon-health-h1-api-openapi.yml\ndocs: https://ribbon.readme.io/docs/authentication\nrevised: '2026-08-14'\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ribbon-health-h1-api-openapi.yml\n  docs: https://ribbon.readme.io/docs/authentication\n  header: 'Authorization: Bearer {customer_token}'\n  credential: single long-lived customer API key\n  issuance: >-\n    Keys are issued through a sales/demo engagement at https://h1.co/request-demo/ — there is no\n    self-serve key generation, no developer signup, and no key-management endpoint in the API.\n  rotation_documented: false\n  test_credentials: false\n  test_credentials_note: >-\n    No sandbox, no test mode and no separate test key prefix are documented, which is why there is\n    no sandbox/ artifact in this repo. The only mode-like distinction is entitlement:\
  \ the spec's\n    own 403 example is \"Trial accounts do not have access to custom specialties\", so trial\n    accounts exist but share the same production host and key format.\n  provider_guidance: >-\n    \"Make sure to keep this API Key secure. Do not share your API Key in publicly accessible\n    areas, such as Github, client-side code, or internal communication tools.\"\noauth2: false\noauth2_note: >-\n  No OAuth, no OIDC, no scopes. /.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all return 404 on\n  api.ribbonhealth.com (probed 2026-08-14). There is no scopes/ artifact for this provider because\n  there is no scope surface to capture — authorization is expressed as account-level product\n  entitlements (e.g. `doctors.can_price_transparency`) enforced with HTTP 403, not as token scopes.\nobserved:\n  method: probed\n  checked: '2026-08-14'\n  failures:\n  - status: 401\n    code: not_authenticated\n    trigger:\
  \ no Authorization header\n  - status: 401\n    code: authentication_failed\n    trigger: syntactically valid but invalid bearer token\n  note: >-\n    The API distinguishes \"no credential\" from \"bad credential\" with two different machine codes,\n    which is better than most. Branch on error.code — the same code returns two different message\n    strings depending on the path.\nagent_notes: >-\n  A single static bearer secret with no scoping, no expiry and no rotation endpoint means an agent\n  granted this key holds the customer's entire H1 surface, including the PHI-bearing eligibility\n  endpoint. There is no way to issue a read-only or module-limited credential from the API. Scope\n  the key at the account level with H1 before delegating it.\ncross_links:\n  conventions: conventions/ribbon-health-conventions.yml\n  errors: errors/ribbon-health-problem-types.yml\n  agentic_access: agentic-access/ribbon-health-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/authentication/ribbon-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Provider Directory
- Insurance
- Clinical Data
- Care Navigation
- Eligibility
- Price Transparency
- Provider Search
- Health Plans
- Digital Health
---
