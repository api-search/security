---
anonymous_access: false
api_key_in: []
api_specs:
- filename: federal-highway-administration-v2x-app-api-openapi.json
  format: json
  label: FHWA V2X App API
  slug: v2x-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-v2x-app-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Federal Highway Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Highway Administration secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Federal Highway Administration
provider_slug: federal-highway-administration
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Keycloak JWT Bearer Token. Required for all endpoints except decode endpoints. Obtain a token from the /auth/token endpoint using your credentials.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/federal-highway-administration-v2x-app-api-openapi.json
  type: http
slug: federal-highway-administration-authentication
source_filename: federal-highway-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: derived\nsource: openapi/federal-highway-administration-v2x-app-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Keycloak JWT Bearer Token. Required for all endpoints except decode endpoints.\n    Obtain a token from the /auth/token endpoint using your credentials.\n  sources:\n  - openapi/federal-highway-administration-v2x-app-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/authentication/federal-highway-administration-authentication.yml
summary_line: http · 1 scheme
tags:
- Federal-Government
- Transportation
- Highways
- Bridges
- Connected-Vehicles
- V2X
- Open-Source
- Open-Data
---
