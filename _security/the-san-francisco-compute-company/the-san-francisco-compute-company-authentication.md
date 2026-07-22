---
api_key_in: []
api_specs:
- filename: the-san-francisco-compute-company-openapi.json
  format: json
  label: SF Compute API (Public Preview)
  slug: sf-compute-api-public-preview
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-san-francisco-compute-company/refs/heads/main/openapi/the-san-francisco-compute-company-openapi.json
auth_types:
- http
description: 'SF Compute''s public preview API authenticates with a Bearer token. Create an API token with `sf tokens create --name <name>` (or in the dashboard at https://sfcompute.com/account/api-keys); the token is shown once and starts with `sk_live_`. Tokens begin with no permissions - grant access per resource with `sf grants create --token <name> --role <role> --workspace <workspace>` (see Roles and Grants). For scripts, set the SF_BEARER_TOKEN or SF_API_KEY environment variable. Send the token as `Authorization: Bearer sk_live_...`.'
kind: authentication
layout: security
method: searched
name: The San Francisco Compute Company Authentication
name_suffix: Authentication
oauth_flows: []
overview: The San Francisco Compute Company secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The San Francisco Compute Company
provider_slug: the-san-francisco-compute-company
scheme_count: 1
schemes:
- authorization_model: role + grant per workspace/resource (see https://docs.sfcompute.com/preview/roles and https://docs.sfcompute.com/preview/grants)
  bearerFormat: JWT
  create_via:
  - 'CLI: sf tokens create --name <name>'
  - 'Dashboard: https://sfcompute.com/account/api-keys'
  description: Bearer token sent as Authorization header. Create via `sf tokens create` or the dashboard API keys page.
  env_vars:
  - SF_BEARER_TOKEN
  - SF_API_KEY
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/the-san-francisco-compute-company-openapi.json
  token_prefix: sk_live_
  type: http
slug: the-san-francisco-compute-company-authentication
source_filename: the-san-francisco-compute-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/the-san-francisco-compute-company-openapi.json\ndocs: https://docs.sfcompute.com/preview/tokens\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\ndescription: >-\n  SF Compute's public preview API authenticates with a Bearer token. Create an\n  API token with `sf tokens create --name <name>` (or in the dashboard at\n  https://sfcompute.com/account/api-keys); the token is shown once and starts\n  with `sk_live_`. Tokens begin with no permissions - grant access per resource\n  with `sf grants create --token <name> --role <role> --workspace <workspace>`\n  (see Roles and Grants). For scripts, set the SF_BEARER_TOKEN or SF_API_KEY\n  environment variable. Send the token as `Authorization: Bearer sk_live_...`.\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  token_prefix: sk_live_\n  create_via:\n  - 'CLI: sf tokens create --name <name>'\n  - 'Dashboard: https://sfcompute.com/account/api-keys'\n\
  \  env_vars:\n  - SF_BEARER_TOKEN\n  - SF_API_KEY\n  authorization_model: role + grant per workspace/resource (see https://docs.sfcompute.com/preview/roles and https://docs.sfcompute.com/preview/grants)\n  description: Bearer token sent as Authorization header. Create via `sf tokens create` or the dashboard API keys page.\n  sources:\n  - openapi/the-san-francisco-compute-company-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-san-francisco-compute-company/refs/heads/main/authentication/the-san-francisco-compute-company-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- GPU
- Compute
- Cloud Infrastructure
- Artificial Intelligence
- Machine Learning
- Compute Marketplace
- Reselling
- Infrastructure
---
