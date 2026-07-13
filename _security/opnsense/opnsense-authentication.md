---
api_key_in: []
api_specs:
- filename: opnsense-openapi.yml
  format: yaml
  label: OPNsense Core REST API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opnsense/refs/heads/main/openapi/opnsense-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opnsense Authentication
name_suffix: Authentication
oauth_flows: []
overview: OPNsense secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OPNsense
provider_slug: opnsense
scheme_count: 1
schemes:
- description: 'HTTP Basic Authentication with the API key as username and the

    API secret as password.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/opnsense-openapi.yml
  type: http
slug: opnsense-authentication
source_filename: opnsense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opnsense-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Authentication with the API key as username and the\n    API secret as password.\n  sources:\n  - openapi/opnsense-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opnsense/refs/heads/main/authentication/opnsense-authentication.yml
summary_line: http · 1 scheme
tags:
- Firewall
- Networking
- Security
- VPN
- Routing
- Open Source
---
