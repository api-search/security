---
api_key_in: []
api_specs:
- filename: citrix-sharefile-openapi.yml
  format: yaml
  label: ShareFile REST API v3
  slug: rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Citrix Sharefile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citrix ShareFile secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Citrix ShareFile
provider_slug: citrix-sharefile
scheme_count: 1
schemes:
- bearerFormat: OAuth2-Access-Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/citrix-sharefile-openapi.yml
  type: http
slug: citrix-sharefile-authentication
source_filename: citrix-sharefile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/citrix-sharefile-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2-Access-Token\n  sources:\n  - openapi/citrix-sharefile-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/authentication/citrix-sharefile-authentication.yml
summary_line: http · 1 scheme
tags:
- File Sharing
- Document Workflow
- Secure File Transfer
- E-Signature
- Client Portal
- Content Collaboration
---
