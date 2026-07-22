---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Range Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Range secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Range
provider_slug: range
scheme_count: 2
schemes:
- description: API keys are created in Range developer settings and passed via HTTP Basic authentication — the API key is supplied as the username and the password is left blank. All requests must be made over HTTPS with TLS 1.2 or higher.
  name: apiKeyBasic
  scheme: basic
  sources:
  - https://www.range.co/docs/api
  type: http
- description: OAuth 2.0 bearer tokens are supported through a currently closed program; access must be requested from the Range support team.
  name: oauthBearer
  scheme: bearer
  sources:
  - https://www.range.co/docs/api
  status: closed-program
  type: oauth2
slug: range-authentication
source_filename: range-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.range.co/docs/api\ndocs: https://www.range.co/docs/api\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header   # HTTP Basic Authorization header (API key as username, blank password)\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKeyBasic\n  type: http\n  scheme: basic\n  description: API keys are created in Range developer settings and passed via HTTP\n    Basic authentication — the API key is supplied as the username and the password\n    is left blank. All requests must be made over HTTPS with TLS 1.2 or higher.\n  sources:\n  - https://www.range.co/docs/api\n- name: oauthBearer\n  type: oauth2\n  scheme: bearer\n  description: OAuth 2.0 bearer tokens are supported through a currently closed program;\n    access must be requested from the Range support team.\n  status: closed-program\n  sources:\n  - https://www.range.co/docs/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/range/refs/heads/main/authentication/range-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Team Collaboration
- Async Communication
- Standups
- Check-ins
- Meetings
- Goals
- OKRs
- Productivity
- Workplace
---
