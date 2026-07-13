---
api_key_in: []
api_specs:
- filename: dsco-platform-openapi.yml
  format: yaml
  label: Dsco Platform API
  slug: dsco-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/dsco-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rithum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rithum secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rithum
provider_slug: rithum
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dsco-platform-openapi.yml
  type: http
slug: rithum-authentication
source_filename: rithum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dsco-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dsco-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/authentication/rithum-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Dropship
- Marketplace
- Ecommerce
- Supply Chain
- Retail
---
