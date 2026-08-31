---
api_key_in: []
api_specs:
- filename: ansible-playbooks-auth-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Auth API
  slug: ansible-playbooks-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-auth-api-openapi.yml
- filename: ansible-playbooks-credentials-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Credentials API
  slug: ansible-playbooks-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-credentials-api-openapi.yml
- filename: ansible-playbooks-hosts-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Hosts API
  slug: ansible-playbooks-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-hosts-api-openapi.yml
- filename: ansible-playbooks-inventories-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Inventories API
  slug: ansible-playbooks-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-inventories-api-openapi.yml
- filename: ansible-playbooks-job-templates-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Job Templates API
  slug: ansible-playbooks-job-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-job-templates-api-openapi.yml
- filename: ansible-playbooks-jobs-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Jobs API
  slug: ansible-playbooks-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-jobs-api-openapi.yml
- filename: ansible-playbooks-organizations-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Organizations API
  slug: ansible-playbooks-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-organizations-api-openapi.yml
- filename: ansible-playbooks-projects-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Projects API
  slug: ansible-playbooks-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-projects-api-openapi.yml
- filename: ansible-playbooks-schedules-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Schedules API
  slug: ansible-playbooks-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-schedules-api-openapi.yml
- filename: ansible-playbooks-users-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Users API
  slug: ansible-playbooks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-users-api-openapi.yml
- filename: ansible-playbooks-workflow-job-templates-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Workflow Job Templates API
  slug: ansible-playbooks-workflow-job-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-workflow-job-templates-api-openapi.yml
- filename: ansible-playbooks-workflow-jobs-api-openapi.yml
  format: yaml
  label: Ansible Playbooks Workflow Jobs API
  slug: ansible-playbooks-workflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/openapi/ansible-playbooks-workflow-jobs-api-openapi.yml
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
