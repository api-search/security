---
api_key_in:
- header
api_specs:
- filename: chef-software-applications-applications-openapi.json
  format: json
  label: Chef Automate API
  slug: chef-automate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef-software/refs/heads/main/openapi/chef-software-applications-applications-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chef Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chef Software secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chef Software
provider_slug: chef-software
scheme_count: 1
schemes:
- description: Chef Automate API token supplied in the `api-token` HTTP header. Created via the Automate UI, the IAM v2 Tokens API (Tokens_CreateToken), or the `chef-automate iam token create` CLI. Access is authorized by IAM v2 policies that reference the token as a member.
  in: header
  name: ApiToken
  parameter_name: api-token
  sources:
  - https://docs.chef.io/automate/api_tokens/
  - openapi/chef-software-iam-v2-tokens-openapi.json
  type: apiKey
slug: chef-software-authentication
source_filename: chef-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chef.io/automate/api_tokens/\ndocs: https://docs.chef.io/automate/api_tokens/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_header: api-token\n  oauth2_flows: []\n  note: >-\n    Chef Automate API tokens are the only supported way to authenticate against\n    the Chef Automate API. A token is presented in the `api-token` request\n    header on every call. Tokens are issued and governed through Chef Automate\n    IAM v2 (see the tokens, policies and rules services); an admin token grants\n    full access and additional tokens can be scoped through IAM policies.\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter_name: api-token\n  description: >-\n    Chef Automate API token supplied in the `api-token` HTTP header. Created via\n    the Automate UI, the IAM v2 Tokens API (Tokens_CreateToken), or the\n    `chef-automate iam token create` CLI. Access is authorized by IAM v2\n  \
  \  policies that reference the token as a member.\n  sources:\n  - https://docs.chef.io/automate/api_tokens/\n  - openapi/chef-software-iam-v2-tokens-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chef-software/refs/heads/main/authentication/chef-software-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- DevOps
- Infrastructure Automation
- Configuration Management
- Compliance
- Security
- Infrastructure as Code
- Cloud
- Continuous Compliance
- Node Management
---
