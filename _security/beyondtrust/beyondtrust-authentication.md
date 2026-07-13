---
api_key_in:
- header
api_specs:
- filename: beyondtrust-password-safe-api.yaml
  format: yaml
  label: BeyondTrust Password Safe API
  slug: beyondtrust-password-safe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/openapi/beyondtrust-password-safe-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Beyondtrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: BeyondTrust secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BeyondTrust
provider_slug: beyondtrust
scheme_count: 1
schemes:
- description: PS-Auth key={APIKey}; runas={AppID}. Authenticate by first calling /auth/signappin to get a session cookie, then use PS-Auth header for subsequent requests.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/beyondtrust-password-safe-api.yaml
  type: apiKey
slug: beyondtrust-authentication
source_filename: beyondtrust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beyondtrust-password-safe-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: PS-Auth key={APIKey}; runas={AppID}. Authenticate by first calling /auth/signappin\n    to get a session cookie, then use PS-Auth header for subsequent requests.\n  sources:\n  - openapi/beyondtrust-password-safe-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/authentication/beyondtrust-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
---
