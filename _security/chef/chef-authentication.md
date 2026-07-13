---
api_key_in:
- header
api_specs:
- filename: chef-infra-server-api-openapi.yml
  format: yaml
  label: Chef Infra Server API
  slug: chef-infra-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-infra-server-api-openapi.yml
- filename: chef-automate-api-openapi.yml
  format: yaml
  label: Chef Automate API
  slug: chef-automate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-automate-api-openapi.yml
- filename: chef-habitat-builder-api-openapi.yml
  format: yaml
  label: Chef Habitat Builder API
  slug: chef-habitat-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-habitat-builder-api-openapi.yml
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
