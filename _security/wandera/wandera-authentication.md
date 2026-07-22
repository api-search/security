---
api_key_in: []
api_specs:
- filename: wandera-risk-api-openapi.yml
  format: yaml
  label: Wandera RADAR Risk API
  slug: wandera-radar-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandera/refs/heads/main/openapi/wandera-risk-api-openapi.yml
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Wandera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wandera secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wandera
provider_slug: wandera
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/wandera-risk-api-openapi.yml
  type: http
  used_by:
  - login
- bearer_format: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wandera-risk-api-openapi.yml
  type: http
  used_by:
  - getDevices
  - overrideDeviceRisk
slug: wandera-authentication
source_filename: wandera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.jamf.com/jamf-security/docs/risk-api-2\ndocs: https://developer.jamf.com/jamf-security/docs/risk-api-2\nsummary:\n  types:\n    - http-basic\n    - http-bearer\n  token_format: JWT\n  token_ttl_seconds: 900\n  notes: >-\n    Two-step auth. Application ID + Application Secret are sent as HTTP Basic\n    credentials to POST /v1/login, which returns a JSON Web Token valid for 15\n    minutes. That JWT is then presented as a Bearer token on all Risk endpoints.\n    Application credentials are created in the Security Integrations section of\n    RADAR Settings.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    used_by:\n      - login\n    sources:\n      - openapi/wandera-risk-api-openapi.yml\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    used_by:\n      - getDevices\n      - overrideDeviceRisk\n    sources:\n      - openapi/wandera-risk-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wandera/refs/heads/main/authentication/wandera-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Cybersecurity
- Mobile Security
- Zero Trust
- Mobile Threat Defense
- Endpoint Security
- Device Risk
- Jamf
---
