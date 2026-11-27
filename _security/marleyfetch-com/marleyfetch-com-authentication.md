---
anonymous_access: false
api_key_in: []
api_specs:
- filename: marleyfetch-com-email-api-openapi.yml
  format: yaml
  label: MarleyFetch Email API
  slug: marleyfetch-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marleyfetch-com/openapi/marleyfetch-com-email-api-openapi.yml
auth_types: []
description: Authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MarleyFetch Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarleyFetch declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MarleyFetch
provider_slug: marleyfetch-com
scheme_count: 1
schemes:
- evidence: 'Every API request carries an API key in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Create a key in the API Keys page of the MarleyFetch dashboard; the full key is shown once and starts with `mf_live_`.
  location: header
  name: API Key
  type: apiKey
slug: marleyfetch-com-authentication
source_filename: marleyfetch-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.marleyfetch.com/guides/api-keys.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.marleyfetch.com/guides/api-keys.md\nsources:\n- https://docs.marleyfetch.com/guides/api-keys.md\n- https://docs.marleyfetch.com/guides/api-keys\n- https://docs.marleyfetch.com/getting-started.md\n- https://docs.marleyfetch.com/getting-started\ndescription: Authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Every API request carries an API key in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the API Keys page of the MarleyFetch dashboard; the full key is shown once and starts with `mf_live_`.\ndocs: https://docs.marleyfetch.com/guides/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/marleyfetch-com/authentication/marleyfetch-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Artificial Intelligence
- Software-as-a-Service
- Automation
---
