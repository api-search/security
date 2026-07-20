---
api_key_in: []
api_specs:
- filename: cirrus-identity-log-api-openapi.json
  format: json
  label: Cirrus Identity Log API
  slug: cirrus-identity-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cirrus-identity/refs/heads/main/openapi/cirrus-identity-log-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cirrus Identity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cirrus Identity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cirrus Identity
provider_slug: cirrus-identity
scheme_count: 1
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/cirrus-identity-log-api-openapi.json
  type: http
slug: cirrus-identity-authentication
source_filename: cirrus-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cirrus-identity-log-api-openapi.json\ndocs: https://blog.cirrusidentity.com/documentation/log-api-credentials\nnotes: >\n  Log API endpoints require HTTP Basic authentication using Log API credentials\n  provisioned in the Cirrus Console.\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cirrus-identity-log-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cirrus-identity/refs/heads/main/authentication/cirrus-identity-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Identity
- Authentication
- Single Sign-On
- SAML
- OIDC
- Higher Education
- Identity Management
- Federation
- Logs
---
