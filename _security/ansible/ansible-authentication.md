---
api_key_in: []
api_specs:
- filename: ansible-auth-api-openapi.yml
  format: yaml
  label: Ansible Auth API
  slug: ansible-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-auth-api-openapi.yml
- filename: ansible-credentials-api-openapi.yml
  format: yaml
  label: Ansible Credentials API
  slug: ansible-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-credentials-api-openapi.yml
- filename: ansible-hosts-api-openapi.yml
  format: yaml
  label: Ansible Hosts API
  slug: ansible-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-hosts-api-openapi.yml
- filename: ansible-inventories-api-openapi.yml
  format: yaml
  label: Ansible Inventories API
  slug: ansible-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-inventories-api-openapi.yml
- filename: ansible-job-templates-api-openapi.yml
  format: yaml
  label: Ansible Job Templates API
  slug: ansible-job-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-job-templates-api-openapi.yml
- filename: ansible-jobs-api-openapi.yml
  format: yaml
  label: Ansible Jobs API
  slug: ansible-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-jobs-api-openapi.yml
- filename: ansible-organizations-api-openapi.yml
  format: yaml
  label: Ansible Organizations API
  slug: ansible-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-organizations-api-openapi.yml
- filename: ansible-projects-api-openapi.yml
  format: yaml
  label: Ansible Projects API
  slug: ansible-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-projects-api-openapi.yml
- filename: ansible-schedules-api-openapi.yml
  format: yaml
  label: Ansible Schedules API
  slug: ansible-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-schedules-api-openapi.yml
- filename: ansible-users-api-openapi.yml
  format: yaml
  label: Ansible Users API
  slug: ansible-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-users-api-openapi.yml
- filename: ansible-workflow-job-templates-api-openapi.yml
  format: yaml
  label: Ansible Workflow Job Templates API
  slug: ansible-workflow-job-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-workflow-job-templates-api-openapi.yml
- filename: ansible-workflow-jobs-api-openapi.yml
  format: yaml
  label: Ansible Workflow Jobs API
  slug: ansible-workflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-workflow-jobs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ansible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ansible secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ansible
provider_slug: ansible
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Personal or application OAuth2 access token.
  name: OAuth2Token
  scheme: bearer
  sources:
  - openapi/ansible-openapi.yml
  type: http
- description: HTTP Basic authentication using local controller credentials.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/ansible-openapi.yml
  type: http
slug: ansible-authentication
source_filename: ansible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ansible-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth2Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Personal or application OAuth2 access token.\n  sources:\n  - openapi/ansible-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using local controller credentials.\n  sources:\n  - openapi/ansible-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/authentication/ansible-authentication.yml
summary_line: http · 2 schemes
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure as Code
- Open-Source
- Orchestration
- Red Hat
---
