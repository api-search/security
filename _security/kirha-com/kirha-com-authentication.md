---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kirha-com-openapi-generated.yml
  format: yaml
  label: Kirha API
  slug: kirha-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kirha-com/openapi/_ae-authored/kirha-com-openapi-generated.yml
auth_types: []
description: All KIRHA API requests require an API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kirha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kirha declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kirha
provider_slug: kirha-com
scheme_count: 1
schemes:
- evidence: 'Or send it in the `Authorization` header for HTTP requests, with or without the `Bearer` scheme:'
  header: Authorization
  how_to_obtain: Create an account, create a project, and generate an API key in the dashboard.
  location: header
  name: API Key
  type: http-bearer
slug: kirha-com-authentication
source_filename: kirha-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.kirha.com/authentication.mdx
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.kirha.com/authentication.mdx\nsources:\n- https://docs.kirha.com/authentication.mdx\n- https://docs.kirha.com/index.mdx\n- https://docs.kirha.com/billing/quickstart.mdx\n- https://docs.kirha.com/search-api/quickstart.mdx\ndescription: All KIRHA API requests require an API key for authentication.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Or send it in the `Authorization` header for HTTP requests, with or without the `Bearer` scheme:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account, create a project, and generate an API key in the dashboard.\ndocs: https://docs.kirha.com/authentication.mdx\n"
source_yaml_url: https://artifacts.apis.io/kirha-com/authentication/kirha-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Data Aggregation
- Contextual Search
- Developer Tools
- Platform
---
