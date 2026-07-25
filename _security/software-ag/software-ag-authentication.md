---
api_key_in: []
api_specs:
- filename: software-ag-apis-api-openapi.yml
  format: yaml
  label: Software AG APIs API
  slug: software-ag-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/openapi/software-ag-apis-api-openapi.yml
- filename: software-ag-applications-api-openapi.yml
  format: yaml
  label: Software AG Applications API
  slug: software-ag-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/openapi/software-ag-applications-api-openapi.yml
- filename: software-ag-policies-api-openapi.yml
  format: yaml
  label: Software AG Policies API
  slug: software-ag-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/openapi/software-ag-policies-api-openapi.yml
- filename: software-ag-publishing-api-openapi.yml
  format: yaml
  label: Software AG Publishing API
  slug: software-ag-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/openapi/software-ag-publishing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Software Ag Authentication
name_suffix: Authentication
oauth_flows: []
overview: Software AG secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Software AG
provider_slug: software-ag
scheme_count: 1
schemes:
- description: Basic authentication with API Gateway administrator credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/webmethods-api-gateway-openapi.yml
  type: http
slug: software-ag-authentication
source_filename: software-ag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/webmethods-api-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with API Gateway administrator credentials\n  sources:\n  - openapi/webmethods-api-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/authentication/software-ag-authentication.yml
summary_line: http · 1 scheme
tags:
- API Management
- Enterprise Integration
- iPaaS
- webMethods
- Integration Platform
- API Gateway
---
