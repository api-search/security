---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ansible Playbooks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ansible Playbooks secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ansible Playbooks
provider_slug: ansible-playbooks
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Personal or application OAuth2 access token.
  name: OAuth2Token
  scheme: bearer
  sources:
  - openapi/ansible-playbooks-openapi.yml
  type: http
- description: HTTP Basic authentication using local controller credentials.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/ansible-playbooks-openapi.yml
  type: http
slug: ansible-playbooks-authentication
source_filename: ansible-playbooks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ansible-playbooks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth2Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Personal or application OAuth2 access token.\n  sources:\n  - openapi/ansible-playbooks-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using local controller credentials.\n  sources:\n  - openapi/ansible-playbooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/authentication/ansible-playbooks-authentication.yml
summary_line: http · 2 schemes
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure As Code
- Orchestration
- Playbooks
---
