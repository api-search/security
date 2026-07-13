---
api_key_in: []
api_specs:
- filename: cisco-systems-cisco-api-openapi.yml
  format: yaml
  label: Cisco DevNet API Catalog
  slug: devnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-systems/refs/heads/main/openapi/cisco-systems-cisco-api-openapi.yml
- filename: openapiSpec
  format: yaml
  label: Cisco Meraki Dashboard
  slug: meraki
  spec_type: OpenAPI
  url: https://api.meraki.com/api/v1/openapiSpec
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Systems secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Systems
provider_slug: cisco-systems
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-systems-cisco-api-openapi.yml
  type: http
slug: cisco-systems-authentication
source_filename: cisco-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-systems-cisco-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cisco-systems-cisco-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-systems/refs/heads/main/authentication/cisco-systems-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Infrastructure
- Networking
- Security
- Fortune 100
---
