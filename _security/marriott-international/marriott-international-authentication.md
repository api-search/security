---
api_key_in:
- header
api_specs:
- filename: marriott-international-developer-api-openapi.yml
  format: yaml
  label: Marriott Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott-international/refs/heads/main/openapi/marriott-international-developer-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Marriott International Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Marriott International secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Marriott International
provider_slug: marriott-international
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://devportalprod.marriott.com/oauth/token
  name: oauth2
  sources:
  - openapi/marriott-international-developer-api-openapi.yml
  type: oauth2
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/marriott-international-developer-api-openapi.yml
  type: apiKey
slug: marriott-international-authentication
source_filename: marriott-international-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marriott-international-developer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://devportalprod.marriott.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/marriott-international-developer-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/marriott-international-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott-international/refs/heads/main/authentication/marriott-international-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Fortune 500
---
