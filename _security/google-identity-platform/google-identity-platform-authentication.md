---
api_key_in:
- query
api_specs:
- filename: identity-toolkit-openapi.yml
  format: yaml
  label: Identity Toolkit API
  slug: identity-toolkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-identity-platform/refs/heads/main/openapi/identity-toolkit-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Google Identity Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Identity Platform secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google Identity Platform
provider_slug: google-identity-platform
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/identity-toolkit-openapi.yml
  type: apiKey
slug: google-identity-platform-authentication
source_filename: google-identity-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/identity-toolkit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/identity-toolkit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-identity-platform/refs/heads/main/authentication/google-identity-platform-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication
- Google Cloud
- Identity
- Multi-Tenancy
- OAuth
- OpenID Connect
- SAML
---
