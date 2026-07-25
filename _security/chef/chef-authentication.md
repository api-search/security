---
api_key_in:
- header
api_specs:
- filename: chef-channels-api-openapi.yml
  format: yaml
  label: Chef Channels API
  slug: chef-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-channels-api-openapi.yml
- filename: chef-clients-api-openapi.yml
  format: yaml
  label: Chef Clients API
  slug: chef-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-clients-api-openapi.yml
- filename: chef-cookbooks-api-openapi.yml
  format: yaml
  label: Chef Cookbooks API
  slug: chef-cookbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-cookbooks-api-openapi.yml
- filename: chef-data-bags-api-openapi.yml
  format: yaml
  label: Chef Data Bags API
  slug: chef-data-bags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-data-bags-api-openapi.yml
- filename: chef-environments-api-openapi.yml
  format: yaml
  label: Chef Environments API
  slug: chef-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-environments-api-openapi.yml
- filename: chef-iam-api-openapi.yml
  format: yaml
  label: Chef IAM API
  slug: chef-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-iam-api-openapi.yml
- filename: chef-nodes-api-openapi.yml
  format: yaml
  label: Chef Nodes API
  slug: chef-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-nodes-api-openapi.yml
- filename: chef-packages-api-openapi.yml
  format: yaml
  label: Chef Packages API
  slug: chef-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-packages-api-openapi.yml
- filename: chef-profiles-api-openapi.yml
  format: yaml
  label: Chef Profiles API
  slug: chef-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-profiles-api-openapi.yml
- filename: chef-reports-api-openapi.yml
  format: yaml
  label: Chef Reports API
  slug: chef-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-reports-api-openapi.yml
- filename: chef-roles-api-openapi.yml
  format: yaml
  label: Chef Roles API
  slug: chef-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-roles-api-openapi.yml
- filename: chef-scans-api-openapi.yml
  format: yaml
  label: Chef Scans API
  slug: chef-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-scans-api-openapi.yml
- filename: chef-users-api-openapi.yml
  format: yaml
  label: Chef Users API
  slug: chef-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chef Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chef secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chef
provider_slug: chef
scheme_count: 3
schemes:
- description: API token issued through the Chef Automate UI or admin API.
  in: header
  name: apiToken
  parameter: api-token
  sources:
  - openapi/chef-automate-api-openapi.yml
  type: apiKey
- bearerFormat: HabitatBuilderToken
  name: habitatToken
  scheme: bearer
  sources:
  - openapi/chef-habitat-builder-api-openapi.yml
  type: http
- description: Chef signed-header authentication using an RSA key associated with a client.
  in: header
  name: chefSignedAuth
  parameter: X-Ops-Authorization
  sources:
  - openapi/chef-infra-server-api-openapi.yml
  type: apiKey
slug: chef-authentication
source_filename: chef-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chef-automate-api-openapi.yml, openapi/chef-habitat-builder-api-openapi.yml,\n  openapi/chef-infra-server-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: api-token\n  description: API token issued through the Chef Automate UI or admin API.\n  sources:\n  - openapi/chef-automate-api-openapi.yml\n- name: habitatToken\n  type: http\n  scheme: bearer\n  bearerFormat: HabitatBuilderToken\n  sources:\n  - openapi/chef-habitat-builder-api-openapi.yml\n- name: chefSignedAuth\n  type: apiKey\n  in: header\n  parameter: X-Ops-Authorization\n  description: Chef signed-header authentication using an RSA key associated with a client.\n  sources:\n  - openapi/chef-infra-server-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/authentication/chef-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Application Delivery
- Automation
- Compliance
- Configuration Management
- DevOps
- DevSecOps
- Habitat
- Infrastructure as Code
- InSpec
---
