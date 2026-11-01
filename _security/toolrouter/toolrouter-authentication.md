---
anonymous_access: false
api_key_in: []
api_specs:
- filename: toolrouter-api-reference-openapi.json
  format: json
  label: Toolrouter API Api-reference API
  slug: toolrouter-api-api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolrouter/openapi/_original/toolrouter-api-reference-openapi.json
auth_types: []
description: ToolRouter Account Management API uses API key authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Toolrouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: ToolRouter declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ToolRouter
provider_slug: toolrouter
scheme_count: 1
schemes:
- evidence: 'All Account Management API requests must include an API key in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Generate an API key from the ToolRouter dashboard (Log into your ToolRouter Dashboard → Navigate to your account settings → Generate a new API key).
  location: header
  name: API Key
  type: apiKey
slug: toolrouter-authentication
source_filename: toolrouter-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.toolrouter.ai/api-reference/endpoint/account/authentication.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.toolrouter.ai/api-reference/endpoint/account/authentication.md\nsources:\n- https://docs.toolrouter.ai/api-reference/endpoint/account/authentication.md\n- https://docs.toolrouter.ai/api-reference/endpoint/account/get_credentials_status.md\n- https://docs.toolrouter.ai/api-reference/endpoint/account/update_credentials.md\n- https://docs.toolrouter.ai/quickstart.md\ndescription: ToolRouter Account Management API uses API key authentication.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'All Account Management API requests must include an API key in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key from the ToolRouter dashboard (Log into your ToolRouter Dashboard → Navigate to your account settings → Generate\n    a new API key).\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other\
  \ schemes are documented.\ndocs: https://docs.toolrouter.ai/api-reference/endpoint/account/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/toolrouter/authentication/toolrouter-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Workflows
- Startups
- Automation
- Founders
---
