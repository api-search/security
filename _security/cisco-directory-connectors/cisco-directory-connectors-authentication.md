---
api_key_in: []
api_specs:
- filename: cisco-directory-connectors-openapi.yml
  format: yaml
  label: Cisco Directory Connector API
  slug: cisco-directory-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-directory-connectors/refs/heads/main/openapi/cisco-directory-connectors-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Directory Connectors Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Directory Connectors secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Directory Connectors
provider_slug: cisco-directory-connectors
scheme_count: 1
schemes:
- bearerFormat: OAuth2-Access-Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-directory-connectors-openapi.yml
  type: http
slug: cisco-directory-connectors-authentication
source_filename: cisco-directory-connectors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-directory-connectors-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2-Access-Token\n  sources:\n  - openapi/cisco-directory-connectors-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-directory-connectors/refs/heads/main/authentication/cisco-directory-connectors-authentication.yml
summary_line: http · 1 scheme
tags:
- Active Directory
- Directory Services
- Identity Management
- LDAP
- User Synchronization
---
