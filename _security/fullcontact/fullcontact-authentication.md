---
api_key_in: []
api_specs:
- filename: fullcontact-openapi.yml
  format: yaml
  label: FullContact V3 API
  slug: v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fullcontact Authentication
name_suffix: Authentication
oauth_flows: []
overview: FullContact secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FullContact
provider_slug: fullcontact
scheme_count: 1
schemes:
- description: FullContact API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fullcontact-openapi.yml
  type: http
slug: fullcontact-authentication
source_filename: fullcontact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fullcontact-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: FullContact API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/fullcontact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/authentication/fullcontact-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity Resolution
- Customer Data
- Data Enrichment
- Person API
- Company API
- Privacy-Safe Identity
- Customer Recognition
---
