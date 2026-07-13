---
api_key_in: []
api_specs:
- filename: numlookupapi-openapi.yml
  format: yaml
  label: NumLookupAPI Phone Number Validation API
  slug: numlookupapi-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numlookupapi/refs/heads/main/openapi/numlookupapi-openapi.yml
- filename: numlookupapi-openapi.yml
  format: yaml
  label: NumLookupAPI Account Status API
  slug: numlookupapi-account-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numlookupapi/refs/heads/main/openapi/numlookupapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Numlookupapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: NumLookupAPI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NumLookupAPI
provider_slug: numlookupapi
scheme_count: 2
schemes:
- description: 'API key passed in the `apikey` HTTP request header. This is the recommended method. Example: `curl "https://api.numlookupapi.com/v1/status" -H "apikey: YOUR-API-KEY"`.'
  in: header
  name: apiKeyHeader
  parameterName: apikey
  recommended: true
  sources:
  - https://numlookupapi.com/docs/authentication
  type: apiKey
- description: 'API key passed as the `apikey` query-string parameter. Not recommended - the docs warn it can expose your API key in access logs and similar. Example: `curl "https://api.numlookupapi.com/v1/status?apikey=YOUR-API-KEY"`.'
  in: query
  name: apiKeyQuery
  parameterName: apikey
  recommended: false
  sources:
  - https://numlookupapi.com/docs/authentication
  type: apiKey
slug: numlookupapi-authentication
source_filename: numlookupapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://numlookupapi.com/docs/authentication\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameterName: apikey\n  description: >-\n    API key passed in the `apikey` HTTP request header. This is the recommended\n    method. Example: `curl \"https://api.numlookupapi.com/v1/status\" -H \"apikey:\n    YOUR-API-KEY\"`.\n  recommended: true\n  sources:\n  - https://numlookupapi.com/docs/authentication\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameterName: apikey\n  description: >-\n    API key passed as the `apikey` query-string parameter. Not recommended - the\n    docs warn it can expose your API key in access logs and similar. Example:\n    `curl \"https://api.numlookupapi.com/v1/status?apikey=YOUR-API-KEY\"`.\n  recommended: false\n  sources:\n  - https://numlookupapi.com/docs/authentication\nnotes: >-\n  Live-probed 2026-07-12: unauthenticated requests return\
  \ HTTP 401 with\n  {\"message\":\"No API key found in request\"} and a `WWW-Authenticate: Key\n  realm=\"kong\"` header, confirming an API-key model behind a Kong gateway. A key\n  is obtained from the NumLookupAPI account dashboard after signing up (free tier\n  available).\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numlookupapi/refs/heads/main/authentication/numlookupapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Number Verification
- Phone Validation
- Phone Number Lookup
- Carrier Lookup
- Line Type
- Verification
- Data Validation
- Caller Identity
---
