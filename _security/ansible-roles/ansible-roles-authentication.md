---
api_key_in:
- header
api_specs:
- filename: ansible-roles-ansible-galaxy-roles-collections-api-api-openapi.yml
  format: yaml
  label: Ansible Roles Ansible Galaxy Roles & Collections API API
  slug: ansible-roles-ansible-galaxy-roles-collections-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-ansible-galaxy-roles-collections-api-api-openapi.yml
- filename: ansible-roles-collections-api-openapi.yml
  format: yaml
  label: Ansible Roles Collections API
  slug: ansible-roles-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-collections-api-openapi.yml
- filename: ansible-roles-imports-api-openapi.yml
  format: yaml
  label: Ansible Roles Imports API
  slug: ansible-roles-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-imports-api-openapi.yml
- filename: ansible-roles-namespaces-api-openapi.yml
  format: yaml
  label: Ansible Roles Namespaces API
  slug: ansible-roles-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-namespaces-api-openapi.yml
- filename: ansible-roles-roles-api-openapi.yml
  format: yaml
  label: Ansible Roles Roles API
  slug: ansible-roles-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-roles-api-openapi.yml
- filename: ansible-roles-sync-api-openapi.yml
  format: yaml
  label: Ansible Roles Sync API
  slug: ansible-roles-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-sync-api-openapi.yml
- filename: ansible-roles-users-api-openapi.yml
  format: yaml
  label: Ansible Roles Users API
  slug: ansible-roles-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/openapi/ansible-roles-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ansible Roles Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ansible Roles secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ansible Roles
provider_slug: ansible-roles
scheme_count: 1
schemes:
- description: 'Galaxy / Automation Hub token, sent as `Authorization: Token <value>`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/ansible-roles-openapi.yml
  type: apiKey
slug: ansible-roles-authentication
source_filename: ansible-roles-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ansible-roles-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Galaxy / Automation Hub token, sent as `Authorization: Token <value>`.'\n  sources:\n  - openapi/ansible-roles-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/authentication/ansible-roles-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ansible
- Automation
- Collections
- Configuration Management
- DevOps
- Infrastructure As Code
- Roles
---
