---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NHANES (CDC) Authentication
name_suffix: Authentication
oauth_flows: []
overview: NHANES (CDC) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NHANES (CDC)
provider_slug: nhanes
scheme_count: 1
schemes:
- description: Optional Socrata application token.
  in: header
  name: appToken
  parameter: X-App-Token
  required: false
  type: apiKey
slug: nhanes-authentication
source_filename: nhanes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://dev.socrata.com/docs/app-tokens.html\ndocs: https://dev.socrata.com/docs/app-tokens.html\nsummary: NHANES datasets on data.cdc.gov are readable anonymously (GET returned 200 with no credentials on 2026-10-30). The platform documents an optional application token that moves a client from a shared IP pool to its own request pool.\nschemes:\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  required: false\n  description: Optional Socrata application token.\n"
source_yaml_url: https://artifacts.apis.io/nhanes/authentication/nhanes-authentication.yml
summary_line: 1 scheme
tags:
- Public Health
- Health Statistics
- Nutrition
- Open Data
- Survey Data
- Government
- CDC
---
