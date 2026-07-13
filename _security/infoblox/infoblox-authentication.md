---
api_key_in:
- cookie
api_specs:
- filename: infoblox-wapi-openapi.yml
  format: yaml
  label: Infoblox WAPI (Web API)
  slug: infoblox-wapi-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoblox/refs/heads/main/openapi/infoblox-wapi-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Infoblox BloxOne API
  slug: infoblox-bloxone-api
  spec_type: OpenAPI
  url: https://csp.infoblox.com/apidoc/
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Infoblox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infoblox secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Infoblox
provider_slug: infoblox
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using NIOS admin credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/infoblox-wapi-openapi.yml
  type: http
- description: Session cookie returned after successful authentication. Pass the ibapauth cookie with subsequent requests to maintain an authenticated session.
  in: cookie
  name: cookieAuth
  parameter: ibapauth
  sources:
  - openapi/infoblox-wapi-openapi.yml
  type: apiKey
slug: infoblox-authentication
source_filename: infoblox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/infoblox-wapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using NIOS admin credentials.\n  sources:\n  - openapi/infoblox-wapi-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: ibapauth\n  description: Session cookie returned after successful authentication. Pass the ibapauth cookie\n    with subsequent requests to maintain an authenticated session.\n  sources:\n  - openapi/infoblox-wapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infoblox/refs/heads/main/authentication/infoblox-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cloud
- DDI
- DHCP
- DNS
- IPAM
- Network Management
- Security
- Threat Intelligence
---
