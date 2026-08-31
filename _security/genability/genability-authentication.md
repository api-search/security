---
api_key_in: []
api_specs:
- filename: genability-get-api-openapi.yml
  format: yaml
  label: Genability GET API
  slug: genability-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-get-api-openapi.yml
- filename: genability-rest-api-openapi.yml
  format: yaml
  label: Genability Rest API
  slug: genability-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Genability Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genability secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Genability
provider_slug: genability
scheme_count: 1
schemes:
- applied: 'Globally — the document declares a root-level security requirement [{sec0: []}], so every one of the 33 operations requires it.'
  credentials:
    password: appKey
    username: appId
  docs: https://docs.arcadia.com/v2022-12-21-Signal/reference/authentication
  name: sec0
  quote: '"Authenticate Arcadia Signal API requests with HTTP Basic authentication using your appId and appKey." appId = username, appKey = password. "Most HTTP clients can send Basic Auth credentials directly. If your client requires a header, construct an Authorization: Basic header from the Base64-encoded appId:appKey pair."'
  scheme: basic
  sources:
  - openapi/genability-signal-openapi.json
  type: http
slug: genability-authentication
source_filename: genability-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/genability-signal-openapi.json\ndocs: https://docs.arcadia.com/v2022-12-21-Signal/reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mtls: false\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/genability-signal-openapi.json\n  applied: >-\n    Globally — the document declares a root-level security requirement\n    [{sec0: []}], so every one of the 33 operations requires it.\n  credentials:\n    username: appId\n    password: appKey\n  docs: https://docs.arcadia.com/v2022-12-21-Signal/reference/authentication\n  quote: >-\n    \"Authenticate Arcadia Signal API requests with HTTP Basic authentication\n    using your appId and appKey.\" appId = username, appKey = password. \"Most\n    HTTP clients can send Basic Auth credentials directly. If your client\n    requires a header, construct\
  \ an Authorization: Basic header from the\n    Base64-encoded appId:appKey pair.\"\ncredential_provisioning:\n  self_serve: true\n  steps:\n  - Create an Arcadia user account at https://dash.genability.com/signup\n  - Create or join an Organization at https://dash.genability.com/org (14-day free trial)\n  - Create an API Application at https://dash.genability.com/org/applications to mint appId and appKey\n  - Authenticate with HTTP Basic\n  credit_card_required: true\n  quote: >-\n    \"If you are on a free trial, you will need to enter a valid credit card to\n    create an Application and get an API Key.\"\n  docs: https://docs.arcadia.com/v2022-12-21-Signal/docs/quick-start\nvalidation:\n  endpoint: GET /rest/echo/authenticate\n  operationId: echo-api-authenticate\n  docs: https://docs.arcadia.com/v2022-12-21-Signal/reference/echo-api-authenticate\ntransport:\n  tls_required: true\n  quote: '\"All API methods should be called over SSL.\"'\n  observed_tls: TLSv1.2 on api.genability.com\
  \ (security/genability-domain-security.yml)\nanonymous_access:\n  available: false\n  note: >-\n    The /rest/public/ paths are \"public\" only in the sense of non-org-scoped\n    reference data. A live anonymous GET of\n    https://api.genability.com/rest/public/tariffs on 2026-07-27 returned HTTP\n    401 with {\"code\":\"Unauthorized\",\"message\":\"The credentials were not supplied\n    or are invalid\",\"propertyName\":\"appId\"}.\nnot_supported:\n  oauth2: No oauth2 securityScheme, no token endpoint, no scopes — scopes/ is intentionally absent.\n  openid_connect: >-\n    https://api.genability.com/.well-known/openid-configuration returns the\n    Signal 401 envelope, not an OIDC document.\n  mutual_tls: Not offered.\n  api_key_header: Not offered — credentials travel as Basic auth, not as a key header.\nrelated:\n  sso: >-\n    https://docs.arcadia.com/v2022-12-21-Signal/docs/single-sign-on covers SSO\n    for human sign-in to the Arcadia dashboard, not API authentication.\n  permissions:\
  \ >-\n    Creating private TOU definitions (POST /rest/timeofuses) \"requires special\n    API permissions. Contact platformsupport@arcadia.com to request access.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/authentication/genability-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- United States
- Utilities
- Electricity
- Tariffs
- Energy Rates
- Rate Calculation
- Energy Data Platform
- Solar
- Grid
---
