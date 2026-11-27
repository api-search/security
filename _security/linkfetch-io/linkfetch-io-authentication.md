---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: linkfetch-io-accounts-api-openapi.yml
  format: yaml
  label: LinkFetch Accounts API
  slug: linkfetch-io-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-accounts-api-openapi.yml
- filename: linkfetch-io-ai-functions-api-openapi.yml
  format: yaml
  label: LinkFetch AI functions API
  slug: linkfetch-io-ai-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-ai-functions-api-openapi.yml
- filename: linkfetch-io-companies-api-openapi.yml
  format: yaml
  label: LinkFetch Companies API
  slug: linkfetch-io-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-companies-api-openapi.yml
- filename: linkfetch-io-jobs-and-companies-api-openapi.yml
  format: yaml
  label: LinkFetch Jobs and companies API
  slug: linkfetch-io-jobs-and-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-jobs-and-companies-api-openapi.yml
- filename: linkfetch-io-jobs-api-openapi.yml
  format: yaml
  label: LinkFetch Jobs API
  slug: linkfetch-io-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-jobs-api-openapi.yml
- filename: linkfetch-io-messages-api-openapi.yml
  format: yaml
  label: LinkFetch Messages API
  slug: linkfetch-io-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-messages-api-openapi.yml
- filename: linkfetch-io-network-api-openapi.yml
  format: yaml
  label: LinkFetch Network API
  slug: linkfetch-io-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-network-api-openapi.yml
- filename: linkfetch-io-people-api-openapi.yml
  format: yaml
  label: LinkFetch People API
  slug: linkfetch-io-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-people-api-openapi.yml
- filename: linkfetch-io-posts-api-openapi.yml
  format: yaml
  label: LinkFetch Posts API
  slug: linkfetch-io-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-posts-api-openapi.yml
- filename: linkfetch-io-your-leads-api-openapi.yml
  format: yaml
  label: LinkFetch Your leads API
  slug: linkfetch-io-your-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkfetch-io/openapi/linkfetch-io-your-leads-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: LinkFetch Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkFetch secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LinkFetch
provider_slug: linkfetch-io
scheme_count: 2
schemes:
- description: Your API key (lf_…) from the dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/linkfetch-io-openapi.json
  type: http
- description: The same API key, as a header.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/linkfetch-io-openapi.json
  type: apiKey
slug: linkfetch-io-authentication
source_filename: linkfetch-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/linkfetch-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Your API key (lf_…) from the dashboard.\n  sources:\n  - openapi/linkfetch-io-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The same API key, as a header.\n  sources:\n  - openapi/linkfetch-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linkfetch-io/authentication/linkfetch-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- LinkedIn
- Automation
- Productivity
- Data
---
