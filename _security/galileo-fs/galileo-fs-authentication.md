---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Galileo Fs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Galileo Financial Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Galileo Financial Technologies
provider_slug: galileo-fs
scheme_count: 1
schemes:
- description: 'HTTPS request authenticated with provider ID, username, password, and

    product ID as documented in the Galileo Pro tenant onboarding guide.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/galileo-fs-openapi.yml
  type: http
slug: galileo-fs-authentication
source_filename: galileo-fs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/galileo-fs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTPS request authenticated with provider ID, username, password, and\n    product ID as documented in the Galileo Pro tenant onboarding guide.\n  sources:\n  - openapi/galileo-fs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/authentication/galileo-fs-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- BaaS
- Card Issuing
- Banking
- Payments
- ACH
---
