---
api_key_in: []
api_specs:
- filename: veracode-applications-openapi.yml
  format: yaml
  label: Veracode Applications REST API
  slug: veracode-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-applications-openapi.yml
- filename: veracode-findings-openapi.yml
  format: yaml
  label: Veracode Findings REST API
  slug: veracode-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-findings-openapi.yml
- filename: veracode-identity-openapi.yml
  format: yaml
  label: Veracode Identity REST API
  slug: veracode-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-identity-openapi.yml
- filename: veracode-reporting-openapi.yml
  format: yaml
  label: Veracode Reporting REST API
  slug: veracode-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-reporting-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veracode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veracode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veracode
provider_slug: veracode
scheme_count: 1
schemes:
- description: HMAC authentication with Veracode API ID and key credentials
  name: HmacAuth
  scheme: veracode_hmac
  sources:
  - openapi/veracode-applications-openapi.yml
  - openapi/veracode-findings-openapi.yml
  - openapi/veracode-identity-openapi.yml
  - openapi/veracode-reporting-openapi.yml
  type: http
slug: veracode-authentication
source_filename: veracode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veracode-applications-openapi.yml, openapi/veracode-findings-openapi.yml, openapi/veracode-identity-openapi.yml,\n  openapi/veracode-reporting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HmacAuth\n  type: http\n  scheme: veracode_hmac\n  description: HMAC authentication with Veracode API ID and key credentials\n  sources:\n  - openapi/veracode-applications-openapi.yml\n  - openapi/veracode-findings-openapi.yml\n  - openapi/veracode-identity-openapi.yml\n  - openapi/veracode-reporting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/authentication/veracode-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Security
- SAST
- DAST
- SCA
- Security Testing
- DevSecOps
---
