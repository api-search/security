---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: A2A Grocery Authentication
name_suffix: Authentication
oauth_flows: []
overview: A2A Grocery declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: A2A Grocery
provider_slug: a2a-grocery-ai
scheme_count: 1
schemes:
- description: OAuth2 client credentials flow for accessing the A2A Grocery API. Obtain a client ID and secret via the registration endpoint, then request a bearer token.
  flow: client_credentials
  registrationUrl: https://a2a-registry.ai/oauth/register
  tokenUrl: https://a2a-registry.ai/oauth/token
  type: oauth2
slug: a2a-grocery-ai-authentication
source_filename: a2a-grocery-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://a2a-grocery.ai/docs\nschemes:\n  - type: oauth2\n    flow: client_credentials\n    tokenUrl: https://a2a-registry.ai/oauth/token\n    registrationUrl: https://a2a-registry.ai/oauth/register\n    description: \"OAuth2 client credentials flow for accessing the A2A Grocery API. Obtain a client ID and secret via the registration endpoint, then request a bearer token.\"\n"
source_yaml_url: https://artifacts.apis.io/a2a-grocery-ai/authentication/a2a-grocery-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Grocery
- Procurement
- Agents
- Marketplace
---
