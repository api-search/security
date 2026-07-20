---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Commaai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comma.ai secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Comma.ai
provider_slug: commaai
scheme_count: 2
schemes:
- bearer_format: JWT
  in: header
  name: connectJWT
  parameter: Authorization
  scheme: bearer
  sources:
  - https://api.comma.ai
  token_url: https://jwt.comma.ai
  type: http
  value_format: JWT {token}
- bearer_format: JWT
  description: Device authentication for openpilot units via POST /v2/pilotauth/.
  name: pilotDeviceAuth
  scheme: bearer
  sources:
  - https://api.comma.ai
  type: http
slug: commaai-authentication
source_filename: commaai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.comma.ai\ndocs: https://api.comma.ai\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\n  token_issuer: https://jwt.comma.ai\nnotes: >-\n  The comma connect API authenticates with a JSON Web Token passed in the\n  Authorization header as `Authorization: JWT {token}` (a `JWT` auth-scheme\n  keyword rather than `Bearer`). Tokens are minted at jwt.comma.ai. Devices\n  running openpilot authenticate separately via POST /v2/pilotauth/ to obtain\n  a device (dongle) token. There is no documented OAuth 2.0 authorization-code\n  flow or scopes reference; access to a device is granted per-user via\n  add_user / del_user on the device.\nschemes:\n- name: connectJWT\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter: Authorization\n  value_format: 'JWT {token}'\n  token_url: https://jwt.comma.ai\n  sources:\n  - https://api.comma.ai\n- name: pilotDeviceAuth\n  type:\
  \ http\n  scheme: bearer\n  bearer_format: JWT\n  description: Device authentication for openpilot units via POST /v2/pilotauth/.\n  sources:\n  - https://api.comma.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commaai/refs/heads/main/authentication/commaai-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Automotive
- Self-Driving
- Robotics
- Artificial Intelligence
- Machine Learning
- Open Source
- Connected Vehicles
- Telematics
- Developer API
---
