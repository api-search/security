---
api_key_in: []
api_specs:
- filename: ansible-controller-api.yaml
  format: yaml
  label: Ansible Automation Controller API
  slug: controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-automation-platform/refs/heads/main/openapi/ansible-controller-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ansible Automation Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ansible Automation Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ansible Automation Platform
provider_slug: ansible-automation-platform
scheme_count: 1
schemes:
- description: OAuth2 token or personal access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ansible-controller-api.yaml
  type: http
slug: ansible-automation-platform-authentication
source_filename: ansible-automation-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ansible-controller-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 token or personal access token.\n  sources:\n  - openapi/ansible-controller-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible-automation-platform/refs/heads/main/authentication/ansible-automation-platform-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Configuration Management
- DevOps
- Infrastructure as Code
- Orchestration
---
