---
api_key_in: []
api_specs:
- filename: nutanix-prism-central-v3-openapi.yml
  format: yaml
  label: Nutanix Prism Central API V3
  slug: prism-central-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-prism-central-v3-openapi.yml
- filename: nutanix-prism-element-v2-openapi.yml
  format: yaml
  label: Nutanix Prism Element API V2
  slug: prism-element-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-prism-element-v2-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nutanix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nutanix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nutanix
provider_slug: nutanix
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Prism Central username and password credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/nutanix-prism-central-v3-openapi.yml
  - openapi/nutanix-prism-element-v2-openapi.yml
  type: http
slug: nutanix-authentication
source_filename: nutanix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nutanix-prism-central-v3-openapi.yml, openapi/nutanix-prism-element-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Prism Central username and password credentials.\n  sources:\n  - openapi/nutanix-prism-central-v3-openapi.yml\n  - openapi/nutanix-prism-element-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/authentication/nutanix-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Management
- Hyperconverged
- Infrastructure
- Virtualization
- Kubernetes
- Database
---
