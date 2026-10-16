---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yepapi-openapi-generated.yml
  format: yaml
  label: YepAPI API
  slug: yepapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yepapi/refs/heads/main/openapi/_ae-authored/yepapi-openapi-generated.yml
auth_types: []
description: Authentication using an API key passed in the request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Yepapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: YepAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: YepAPI
provider_slug: yepapi
scheme_count: 1
schemes:
- evidence: All requests to YepAPI require an API key passed via the x-api-key header.
  header: x-api-key
  location: header
  name: API Key
  type: apiKey
slug: yepapi-authentication
source_filename: yepapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.yepapi.com/getting-started/authentication
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.yepapi.com/getting-started/authentication\nsources:\n- https://docs.yepapi.com/getting-started/authentication\n- https://docs.yepapi.com/getting-started/billing\n- https://docs.yepapi.com/getting-started/errors\ndescription: Authentication using an API key passed in the request header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All requests to YepAPI require an API key passed via the x-api-key header.\n  location: header\n  header: x-api-key\nnote: Sign up at app.yepapi.com; your API key is available on the dashboard.\ndocs: https://docs.yepapi.com/getting-started/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yepapi/refs/heads/main/authentication/yepapi-authentication.yml
summary_line: 1 scheme
tags:
- SEO
- SERP
- WebScraping
- AIModels
- Marketing
---
