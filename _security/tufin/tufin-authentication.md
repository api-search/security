---
api_key_in: []
api_specs:
- filename: tufin-securetrack-openapi.yml
  format: yaml
  label: Tufin SecureTrack API
  slug: tufin-securetrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-securetrack-openapi.yml
- filename: tufin-securechange-openapi.yml
  format: yaml
  label: Tufin SecureChange API
  slug: tufin-securechange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-securechange-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tufin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tufin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tufin
provider_slug: tufin
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Tufin Orchestration Suite credentials. The authenticated user's TOS permissions apply to all API requests.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tufin-securechange-openapi.yml
  - openapi/tufin-securetrack-openapi.yml
  type: http
slug: tufin-authentication
source_filename: tufin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tufin-securechange-openapi.yml, openapi/tufin-securetrack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Tufin Orchestration Suite credentials. The authenticated\n    user's TOS permissions apply to all API requests.\n  sources:\n  - openapi/tufin-securechange-openapi.yml\n  - openapi/tufin-securetrack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/authentication/tufin-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Compliance
- Firewall Management
- Network Security
- Network Topology
- Policy Orchestration
- Risk Management
- Security Policy Management
- Zero Trust
---
