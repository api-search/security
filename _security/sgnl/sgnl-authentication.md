---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sgnl Authentication
name_suffix: Authentication
oauth_flows: []
overview: SGNL secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SGNL
provider_slug: sgnl
scheme_count: 1
schemes:
- description: 'The SGNL Public API v2 (Access Service) authenticates with a Bearer token passed in the Authorization header ("Authorization: Bearer {access-token}"). The token is generated during integration/protected-system configuration in the SGNL console. All requests must use HTTPS.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.sgnl.ai/
  type: http
slug: sgnl-authentication
source_filename: sgnl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.sgnl.ai/\ndocs: https://developer.sgnl.ai/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    The SGNL Public API v2 (Access Service) authenticates with a Bearer token passed\n    in the Authorization header (\"Authorization: Bearer {access-token}\"). The token\n    is generated during integration/protected-system configuration in the SGNL\n    console. All requests must use HTTPS.\n  sources:\n  - https://developer.sgnl.ai/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sgnl/refs/heads/main/authentication/sgnl-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Identity
- Authorization
- Access Management
- CAEP
- Shared Signals
- Zero Standing Privilege
- IAM
---
