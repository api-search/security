---
api_key_in: []
api_specs:
- filename: abstractapi-phone-openapi.yml
  format: yaml
  label: Abstract API Phone Validation API
  slug: abstractapi-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstractapi-phone/refs/heads/main/openapi/abstractapi-phone-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Abstractapi Phone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abstract API Phone Validation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abstract API Phone Validation
provider_slug: abstractapi-phone
scheme_count: 1
schemes:
- description: 'Abstract API authenticates by an API key passed as the `api_key` query parameter on the request, e.g. https://phonevalidation.abstractapi.com/v1/?api_key=YOUR_API_KEY&phone=+14152007986. Each Abstract API product (phone validation, email validation, IP geolocation, etc.) issues its own distinct key. Live-confirmed 2026-07-12: a missing or invalid key returns HTTP 401 with an "Invalid API key provided" error.'
  in: query
  keyName: api_key
  name: apiKeyQuery
  sources:
  - openapi/abstractapi-phone-openapi.yml
  - https://www.abstractapi.com/api/phone-validation-api
  type: apiKey
slug: abstractapi-phone-authentication
source_filename: abstractapi-phone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/abstractapi-phone-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  keyName: api_key\n  description: >-\n    Abstract API authenticates by an API key passed as the `api_key` query\n    parameter on the request, e.g.\n    https://phonevalidation.abstractapi.com/v1/?api_key=YOUR_API_KEY&phone=+14152007986.\n    Each Abstract API product (phone validation, email validation, IP\n    geolocation, etc.) issues its own distinct key. Live-confirmed 2026-07-12: a\n    missing or invalid key returns HTTP 401 with an \"Invalid API key provided\"\n    error.\n  sources:\n  - openapi/abstractapi-phone-openapi.yml\n  - https://www.abstractapi.com/api/phone-validation-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstractapi-phone/refs/heads/main/authentication/abstractapi-phone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Number Verification
- Phone Validation
- Phone Number
- Phone Number Lookup
- Verification
- Carrier Lookup
- Line Type
- Data Validation
---
