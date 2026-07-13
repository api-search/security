---
api_key_in:
- header
api_specs:
- filename: pfsense-openapi.yml
  format: yaml
  label: pfSense REST API (pfSense-pkg-RESTAPI)
  slug: rest-api-package
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pfsense/refs/heads/main/openapi/pfsense-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pfsense Authentication
name_suffix: Authentication
oauth_flows: []
overview: pfSense secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: pfSense
provider_slug: pfsense
scheme_count: 3
schemes:
- description: HTTP Basic auth with a pfSense local database username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pfsense-openapi.yml
  type: http
- description: 'API key generated through the webConfigurator or API endpoints. Keys

    inherit the permissions of the user that issued them.'
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/pfsense-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'JWT bearer token obtained from POST /api/v2/auth/jwt. Tokens default

    to one hour of validity.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pfsense-openapi.yml
  type: http
slug: pfsense-authentication
source_filename: pfsense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pfsense-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with a pfSense local database username and password.\n  sources:\n  - openapi/pfsense-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    API key generated through the webConfigurator or API endpoints. Keys\n    inherit the permissions of the user that issued them.\n  sources:\n  - openapi/pfsense-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT bearer token obtained from POST /api/v2/auth/jwt. Tokens default\n    to one hour of validity.\n  sources:\n  - openapi/pfsense-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pfsense/refs/heads/main/authentication/pfsense-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Firewall
- Network Security
- Router
- VPN
- Open Source
- FreeBSD
- Netgate
---
