---
api_key_in:
- header
api_specs:
- filename: springer-nature-meta-openapi.yml
  format: yaml
  label: Springer Nature Meta API
  slug: springer-nature-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/springer-nature/refs/heads/main/openapi/springer-nature-meta-openapi.yml
- filename: springer-nature-openaccess-openapi.yml
  format: yaml
  label: Springer Nature Open Access API
  slug: springer-nature-openaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/springer-nature/refs/heads/main/openapi/springer-nature-openaccess-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Springer Nature Authentication
name_suffix: Authentication
oauth_flows: []
overview: Springer Nature secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Springer Nature
provider_slug: springer-nature
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-ApiKey
  sources:
  - openapi/springer-nature-meta-openapi.yml
  - openapi/springer-nature-openaccess-openapi.yml
  type: apiKey
slug: springer-nature-authentication
source_filename: springer-nature-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/springer-nature-meta-openapi.yml, openapi/springer-nature-openaccess-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-ApiKey\n  sources:\n  - openapi/springer-nature-meta-openapi.yml\n  - openapi/springer-nature-openaccess-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/springer-nature/refs/heads/main/authentication/springer-nature-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Academic Publishing
- Open Access
- Research
- Scholarly Content
- Scientific Publishing
---
