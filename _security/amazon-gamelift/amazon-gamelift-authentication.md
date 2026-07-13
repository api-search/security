---
api_key_in:
- header
api_specs:
- filename: amazon-gamelift-openapi.yaml
  format: yaml
  label: Amazon GameLift API
  slug: amazon-gamelift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/openapi/amazon-gamelift-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Gamelift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon GameLift secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-gamelift-openapi.yaml
  type: apiKey
slug: amazon-gamelift-authentication
source_filename: amazon-gamelift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-gamelift-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-gamelift-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/authentication/amazon-gamelift-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
---
