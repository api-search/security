---
api_key_in: []
api_specs:
- filename: apiida-api-control-plane-openapi.yml
  format: yaml
  label: APIIDA API Control Plane
  slug: api-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/openapi/apiida-api-control-plane-openapi.yml
- filename: apiida-api-gateway-manager-openapi.yml
  format: yaml
  label: APIIDA API Gateway Manager
  slug: api-gateway-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/openapi/apiida-api-gateway-manager-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apiida Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIIDA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIIDA
provider_slug: apiida
scheme_count: 1
schemes:
- description: Bearer token authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apiida-api-control-plane-openapi.yml
  - openapi/apiida-api-gateway-manager-openapi.yml
  type: http
slug: apiida-authentication
source_filename: apiida-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apiida-api-control-plane-openapi.yml, openapi/apiida-api-gateway-manager-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication\n  sources:\n  - openapi/apiida-api-control-plane-openapi.yml\n  - openapi/apiida-api-gateway-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/authentication/apiida-authentication.yml
summary_line: http · 1 scheme
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
---
