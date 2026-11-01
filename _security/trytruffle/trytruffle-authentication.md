---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trytruffle-agents-api-openapi.yml
  format: yaml
  label: Truffle AI Agents API
  slug: trytruffle-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trytruffle/openapi/trytruffle-agents-api-openapi.yml
auth_types: []
description: Truffle AI API uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Trytruffle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truffle AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Truffle AI
provider_slug: trytruffle
scheme_count: 1
schemes:
- evidence: 'Authentication is performed via the `x-api-key` header:'
  header: x-api-key
  how_to_obtain: Sign up for a Truffle AI account, navigate to the API section in your dashboard, and generate a new API key.
  location: header
  name: API Key
  type: apiKey
slug: trytruffle-authentication
source_filename: trytruffle-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.trytruffle.ai/api-reference/authentication.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.trytruffle.ai/api-reference/authentication.md\nsources:\n- https://docs.trytruffle.ai/api-reference/authentication.md\n- https://docs.trytruffle.ai/quickstart.md\n- https://docs.trytruffle.ai/sdk/quickstart.md\ndescription: Truffle AI API uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Authentication is performed via the `x-api-key` header:'\n  location: header\n  header: x-api-key\n  how_to_obtain: Sign up for a Truffle AI account, navigate to the API section in your dashboard, and generate a new API key.\ndocs: https://docs.trytruffle.ai/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/trytruffle/authentication/trytruffle-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
