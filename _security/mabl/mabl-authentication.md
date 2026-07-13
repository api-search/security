---
api_key_in: []
api_specs:
- filename: mabl-openapi.yml
  format: yaml
  label: Mabl API
  slug: mabl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mabl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mabl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mabl
provider_slug: mabl
scheme_count: 1
schemes:
- description: HTTP Basic with username "key" and a mabl API key as the password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/mabl-openapi.yml
  type: http
slug: mabl-authentication
source_filename: mabl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mabl-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with username \"key\" and a mabl API key as the password.\n  sources:\n  - openapi/mabl-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/authentication/mabl-authentication.yml
summary_line: http · 1 scheme
tags:
- Test Automation
- QA
- DevOps
- AI Testing
- Platform
---
