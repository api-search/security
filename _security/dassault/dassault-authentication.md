---
api_key_in:
- header
api_specs:
- filename: ws3dx-dotnet
  format: yaml
  label: 3DEXPERIENCE Engineering Web Services
  slug: 3dexperience-engineering-web-services
  spec_type: OpenAPI
  url: https://github.com/3ds-cpe-emed/ws3dx-dotnet
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dassault Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dassault Systèmes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dassault Systèmes
provider_slug: dassault
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/dassault-api4partners-openapi.yaml
  type: apiKey
slug: dassault-authentication
source_filename: dassault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dassault-api4partners-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/dassault-api4partners-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/authentication/dassault-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- 3DEXPERIENCE
- PLM
- Product Lifecycle Management
- CAD
- Manufacturing
- SolidWorks
- CATIA
- ENOVIA
- Engineering
- 3D Collaboration
---
