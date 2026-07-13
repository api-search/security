---
api_key_in: []
api_specs:
- filename: konsentus-verify-api-openapi.yml
  format: yaml
  label: Konsentus Verify API
  slug: konsentus-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konsentus/refs/heads/main/openapi/konsentus-verify-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Konsentus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Konsentus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Konsentus
provider_slug: konsentus
scheme_count: 1
schemes:
- description: HTTP Basic authentication using the API consumer's client ID and client secret.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/konsentus-verify-api-openapi.yml
  type: http
slug: konsentus-authentication
source_filename: konsentus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/konsentus-verify-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the API consumer's client ID and client secret.\n  sources:\n  - openapi/konsentus-verify-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konsentus/refs/heads/main/authentication/konsentus-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- Open Finance
- PSD2
- PSD3
- FiDA
- TPP Verification
- Identity
- eIDAS
- Trust Services
- Regulatory Checking
- Financial Services
---
