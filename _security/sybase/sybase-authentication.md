---
api_key_in: []
api_specs:
- filename: sybase-ase-rest-api-openapi.yml
  format: yaml
  label: Sybase ASE REST API
  slug: sybase-ase-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-ase-rest-api-openapi.yml
- filename: openapi.json
  format: json
  label: Sybase IQ REST API
  slug: sybase-iq-rest-api
  spec_type: OpenAPI
  url: https://api.sybase.example.com/iq/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sybase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sybase secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sybase
provider_slug: sybase
scheme_count: 2
schemes:
- description: HTTP Basic authentication using SAP ASE server login credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sybase-ase-rest-api-openapi.yml
  type: http
- description: Bearer token authentication for API access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sybase-ase-rest-api-openapi.yml
  type: http
slug: sybase-authentication
source_filename: sybase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sybase-ase-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using SAP ASE server login credentials.\n  sources:\n  - openapi/sybase-ase-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for API access.\n  sources:\n  - openapi/sybase-ase-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/authentication/sybase-authentication.yml
summary_line: http · 2 schemes
tags:
- Database
- Enterprise
- SAP
- SQL
---
