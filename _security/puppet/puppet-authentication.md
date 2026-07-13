---
api_key_in:
- header
api_specs:
- filename: puppet-openapi.yml
  format: yaml
  label: Puppet Enterprise Orchestrator API
  slug: orchestrator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puppet/refs/heads/main/openapi/puppet-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Puppet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Puppet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Puppet
provider_slug: puppet
scheme_count: 1
schemes:
- description: 'Puppet Enterprise RBAC user authentication token. May be retrieved via

    `puppet-access show`. Required on every request.'
  in: header
  name: rbacToken
  parameter: X-Authentication
  sources:
  - openapi/puppet-openapi.yml
  type: apiKey
slug: puppet-authentication
source_filename: puppet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/puppet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rbacToken\n  type: apiKey\n  in: header\n  parameter: X-Authentication\n  description: |-\n    Puppet Enterprise RBAC user authentication token. May be retrieved via\n    `puppet-access show`. Required on every request.\n  sources:\n  - openapi/puppet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puppet/refs/heads/main/authentication/puppet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Configuration Management
- DevOps
- Enterprise
- Infrastructure as Code
- Orchestration
- RBAC
---
