---
api_key_in: []
api_specs:
- filename: rest-api
  format: yaml
  label: Soda Cloud REST API
  slug: soda-cloud-rest-api
  spec_type: OpenAPI
  url: https://docs.soda.io/reference/rest-api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soda Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soda
provider_slug: soda-co
scheme_count: 1
schemes:
- description: 'Base64-encoded API key ID and secret: base64(api_key_id:api_key_secret)'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/soda-cloud-rest-api.json
  type: http
slug: soda-co-authentication
source_filename: soda-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soda-cloud-rest-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Base64-encoded API key ID and secret: base64(api_key_id:api_key_secret)'\n  sources:\n  - openapi/soda-cloud-rest-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/authentication/soda-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Quality
- Data Observability
- Data Contracts
- Data Testing
- Data Monitoring
- Data Engineering
---
