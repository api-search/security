---
api_key_in: []
api_specs:
- filename: microsoft-fabric-openapi.yml
  format: yaml
  label: Microsoft Fabric REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-fabric/refs/heads/main/openapi/microsoft-fabric-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Fabric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Fabric secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Fabric
provider_slug: microsoft-fabric
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-fabric-openapi.yml
  type: http
slug: microsoft-fabric-authentication
source_filename: microsoft-fabric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-fabric-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-fabric-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-fabric/refs/heads/main/authentication/microsoft-fabric-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Analytics
- Data Engineering
- Data Platform
- Lakehouse
- Microsoft
---
