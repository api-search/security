---
api_key_in:
- header
api_specs:
- filename: prisma-cloud-openapi.yml
  format: yaml
  label: Prisma Cloud
  slug: prisma-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma-cloud/refs/heads/main/openapi/prisma-cloud-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prisma Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prisma Cloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prisma Cloud
provider_slug: prisma-cloud
scheme_count: 1
schemes:
- description: 'JWT obtained from POST /login. Tokens are valid for 10 minutes and can be

    refreshed via GET /auth_token/extend.'
  in: header
  name: redlockAuth
  parameter: x-redlock-auth
  sources:
  - openapi/prisma-cloud-openapi.yml
  type: apiKey
slug: prisma-cloud-authentication
source_filename: prisma-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prisma-cloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: redlockAuth\n  type: apiKey\n  in: header\n  parameter: x-redlock-auth\n  description: |-\n    JWT obtained from POST /login. Tokens are valid for 10 minutes and can be\n    refreshed via GET /auth_token/extend.\n  sources:\n  - openapi/prisma-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prisma-cloud/refs/heads/main/authentication/prisma-cloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Native
- Cloud Security
- Compliance
- Containers
- CSPM
- Security
---
