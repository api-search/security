---
api_key_in:
- header
- query
api_specs:
- filename: happyornot-openapi-original.yml
  format: yaml
  label: HappyOrNot Customer API v2
  slug: happyornot-customer-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyornot/refs/heads/main/openapi/happyornot-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Happyornot Authentication
name_suffix: Authentication
oauth_flows: []
overview: HappyOrNot secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HappyOrNot
provider_slug: happyornot
scheme_count: 2
schemes:
- description: API Tokens are managed in Organization Settings page in Analytics
  in: header
  name: ApiTokenAuth
  parameter: X-HON-API-Token
  sources:
  - openapi/happyornot-openapi-original.yml
  type: apiKey
- description: E.g. /some/path?auth=<tokenhere>
  in: query
  name: ApiTokenViaQueryStringAuth
  parameter: auth
  sources:
  - openapi/happyornot-openapi-original.yml
  type: apiKey
slug: happyornot-authentication
source_filename: happyornot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/happyornot-openapi-original.yml\ndocs: https://happyornot.github.io/docs/api-v1/authentication/\nnotes: >-\n  API v2 tokens are generated on the Organization Settings page in HappyOrNot\n  Analytics (Admin privileges required). Tokens are scoped to the groups and\n  experience points the issuing user is authorised for. v1 and v2 tokens are not\n  interchangeable. Provide the token via the X-HON-API-Token header (recommended)\n  or the auth query-string parameter.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-HON-API-Token\n  description: API Tokens are managed in Organization Settings page in Analytics\n  sources:\n  - openapi/happyornot-openapi-original.yml\n- name: ApiTokenViaQueryStringAuth\n  type: apiKey\n  in: query\n  parameter: auth\n  description: E.g. /some/path?auth=<tokenhere>\n  sources:\n  - openapi/happyornot-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyornot/refs/heads/main/authentication/happyornot-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise
- Customer Experience
- Customer Feedback
- Surveys
- Analytics
- Voice of Customer
- Retail
- Feedback
---
