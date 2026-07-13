---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Orange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orange secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orange
provider_slug: orange
scheme_count: 1
schemes:
- name: openId
  openIdConnectUrl: https://api.orange.com/.well-known/openid-configuration
  sources:
  - openapi/orange-openapi.yml
  type: openIdConnect
slug: orange-authentication
source_filename: orange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orange-openapi.yml\nsummary:\n  types:\n  - openIdConnect\nschemes:\n- name: openId\n  type: openIdConnect\n  openIdConnectUrl: https://api.orange.com/.well-known/openid-configuration\n  sources:\n  - openapi/orange-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange/refs/heads/main/authentication/orange-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Network
- Telecom
- Identity
- Messaging
- Location
- Payment
- IoT
---
