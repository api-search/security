---
api_key_in: []
api_specs:
- filename: sybase-backups-api-openapi.yml
  format: yaml
  label: Sybase Backups API
  slug: sybase-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-backups-api-openapi.yml
- filename: sybase-configuration-api-openapi.yml
  format: yaml
  label: Sybase Configuration API
  slug: sybase-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-configuration-api-openapi.yml
- filename: sybase-databases-api-openapi.yml
  format: yaml
  label: Sybase Databases API
  slug: sybase-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-databases-api-openapi.yml
- filename: sybase-devices-api-openapi.yml
  format: yaml
  label: Sybase Devices API
  slug: sybase-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-devices-api-openapi.yml
- filename: sybase-performance-api-openapi.yml
  format: yaml
  label: Sybase Performance API
  slug: sybase-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-performance-api-openapi.yml
- filename: sybase-servers-api-openapi.yml
  format: yaml
  label: Sybase Servers API
  slug: sybase-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-servers-api-openapi.yml
- filename: sybase-users-api-openapi.yml
  format: yaml
  label: Sybase Users API
  slug: sybase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-users-api-openapi.yml
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
