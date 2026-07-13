---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Cisco Directory Connector Sync API
  slug: cisco-directory-connector-sync-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Control Hub API
  slug: webex-control-hub-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Directory Connector Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Directory Connector secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Directory Connector
provider_slug: cisco-directory-connector
scheme_count: 1
schemes:
- bearerFormat: OAuth2-Access-Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-directory-connector-openapi.yml
  type: http
slug: cisco-directory-connector-authentication
source_filename: cisco-directory-connector-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-directory-connector-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2-Access-Token\n  sources:\n  - openapi/cisco-directory-connector-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-directory-connector/refs/heads/main/authentication/cisco-directory-connector-authentication.yml
summary_line: http · 1 scheme
tags:
- Active Directory
- Directory
- Enterprise
- Identity Management
- LDAP
- Provisioning
- SCIM
- Synchronization
---
