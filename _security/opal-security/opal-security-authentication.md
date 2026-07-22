---
api_key_in: []
api_specs:
- filename: opal-security-openapi.yaml
  format: yaml
  label: Opal API
  slug: opal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal-security/refs/heads/main/openapi/opal-security-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opal Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opal Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opal Security
provider_slug: opal-security
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/opal-security-openapi.yaml
  type: http
slug: opal-security-authentication
source_filename: opal-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opal-security-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/opal-security-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opal-security/refs/heads/main/authentication/opal-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Access Management
- Identity and Access Management
- Least Privilege
- Access Reviews
- Security
---
