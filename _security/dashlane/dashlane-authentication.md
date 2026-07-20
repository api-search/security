---
api_key_in: []
api_specs:
- filename: dashlane-public-api-openapi-original.json
  format: json
  label: Dashlane Public API
  slug: dashlane-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dashlane/refs/heads/main/openapi/dashlane-public-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dashlane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dashlane secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dashlane
provider_slug: dashlane
scheme_count: 2
schemes:
- description: Does not require anything to access the endpoint
  name: NONE
  scheme: x-dashlane-auth-none
  sources:
  - openapi/dashlane-public-api-openapi-original.json
  type: http
- description: Bearer authentication with DLP token
  name: PublicAPIToken
  scheme: bearer
  sources:
  - openapi/dashlane-public-api-openapi-original.json
  type: http
slug: dashlane-authentication
source_filename: dashlane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dashlane-public-api-openapi-original.json\ndocs: https://dashlane.github.io/public-api-documentation/\ntoken_format: Bearer [example key]\nprovisioning: Dashlane Admin Console or `dcli team public-api create-key`\nsummary:\n  types:\n  - http\nschemes:\n- name: NONE\n  type: http\n  scheme: x-dashlane-auth-none\n  description: Does not require anything to access the endpoint\n  sources:\n  - openapi/dashlane-public-api-openapi-original.json\n- name: PublicAPIToken\n  type: http\n  scheme: bearer\n  description: Bearer authentication with DLP token\n  sources:\n  - openapi/dashlane-public-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dashlane/refs/heads/main/authentication/dashlane-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Cybersecurity
- Password Management
- Identity
- Security
- Credential Monitoring
- Secrets Management
---
