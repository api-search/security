---
api_key_in:
- header
api_specs:
- filename: plasmic-openapi.yml
  format: yaml
  label: Plasmic CMS API
  slug: cms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plasmic/refs/heads/main/openapi/plasmic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Plasmic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plasmic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plasmic
provider_slug: plasmic
scheme_count: 1
schemes:
- description: 'Plasmic CMS authentication header in the form `CMS_ID:TOKEN`. Use the

    public token for read operations and the secret token for write

    operations.'
  in: header
  name: cmsTokens
  parameter: x-plasmic-api-cms-tokens
  sources:
  - openapi/plasmic-openapi.yml
  type: apiKey
slug: plasmic-authentication
source_filename: plasmic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plasmic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: cmsTokens\n  type: apiKey\n  in: header\n  parameter: x-plasmic-api-cms-tokens\n  description: |-\n    Plasmic CMS authentication header in the form `CMS_ID:TOKEN`. Use the\n    public token for read operations and the secret token for write\n    operations.\n  sources:\n  - openapi/plasmic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plasmic/refs/heads/main/authentication/plasmic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Visual Builder
- Headless CMS
- React
- Next.js
- Gatsby
- Low-Code
- Frontend
---
