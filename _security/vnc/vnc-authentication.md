---
api_key_in: []
api_specs:
- filename: vnc-cloud-openapi.yml
  format: yaml
  label: VNC Cloud API
  slug: vnc-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vnc/refs/heads/main/openapi/vnc-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vnc Authentication
name_suffix: Authentication
oauth_flows: []
overview: VNC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VNC
provider_slug: vnc
scheme_count: 1
schemes:
- description: Basic authentication using VNC Cloud API key (username) and secret (password) provided by RealVNC.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/vnc-cloud-openapi.yml
  type: http
slug: vnc-authentication
source_filename: vnc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vnc-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using VNC Cloud API key (username) and secret (password)\n    provided by RealVNC.\n  sources:\n  - openapi/vnc-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vnc/refs/heads/main/authentication/vnc-authentication.yml
summary_line: http · 1 scheme
tags:
- Remote Desktop
- Remote Access
- VNC
- Networking
- Screen Sharing
---
