---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-fabric-fabriccapacities-api-openapi.yml
  format: yaml
  label: Microsoft Fabric Fabric Capacities API
  slug: microsoft-fabric-fabriccapacities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-fabric/openapi/microsoft-fabric-fabriccapacities-api-openapi.yml
- filename: microsoft-fabric-operations-api-openapi.yml
  format: yaml
  label: Microsoft Fabric Operations API
  slug: microsoft-fabric-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-fabric/openapi/microsoft-fabric-operations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
  - openapi/_superseded/microsoft-fabric-capacities-api-openapi.yml
  - openapi/_superseded/microsoft-fabric-connections-api-openapi.yml
  - openapi/_superseded/microsoft-fabric-items-api-openapi.yml
  - openapi/_superseded/microsoft-fabric-workspaces-api-openapi.yml
  type: http
slug: microsoft-fabric-authentication
source_filename: microsoft-fabric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-fabric-capacities-api-openapi.yml, openapi/_superseded/microsoft-fabric-connections-api-openapi.yml,\n  openapi/_superseded/microsoft-fabric-items-api-openapi.yml, openapi/_superseded/microsoft-fabric-workspaces-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_superseded/microsoft-fabric-capacities-api-openapi.yml\n  - openapi/_superseded/microsoft-fabric-connections-api-openapi.yml\n  - openapi/_superseded/microsoft-fabric-items-api-openapi.yml\n  - openapi/_superseded/microsoft-fabric-workspaces-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-fabric/authentication/microsoft-fabric-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Analytics
- Data Engineering
- Data Platform
- Lakehouse
- Microsoft
---
