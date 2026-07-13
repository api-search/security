---
api_key_in: []
api_specs:
- filename: karrio-openapi.yml
  format: yaml
  label: Karrio Shipping API
  slug: shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Karrio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Karrio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Karrio
provider_slug: karrio
scheme_count: 1
schemes:
- description: Karrio API token sent as a Bearer credential in the Authorization header.
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/karrio-openapi.yml
  type: http
slug: karrio-authentication
source_filename: karrio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/karrio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  description: Karrio API token sent as a Bearer credential in the Authorization header.\n  sources:\n  - openapi/karrio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/authentication/karrio-authentication.yml
summary_line: http · 1 scheme
tags:
- Label Generation
- Logistics
- Package Tracking
- Shipping
---
