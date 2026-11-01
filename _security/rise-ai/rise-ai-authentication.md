---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rise-ai-openapi-generated.yml
  format: yaml
  label: Rise.ai API
  slug: rise-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rise-ai/openapi/_ae-authored/rise-ai-openapi-generated.yml
auth_types: []
description: OAuth 2.0 Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Rise Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rise.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Rise.ai
provider_slug: rise-ai
scheme_count: 1
schemes:
- evidence: The process uses a client_credentials OAuth flow scoped by a unique instanceId for each merchant who installs your app.
  how_to_obtain: Exchange your app credentials (client_id and client_secret) and the merchant's instanceId for an access token via a POST request to the token URL.
  location: body
  name: OAuth 2.0
  token_url: https://platform.rise.ai/oauth2/token
  type: oauth2
slug: rise-ai-authentication
source_filename: rise-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.rise.ai/authentication/oauth
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.rise.ai/authentication/oauth\nsources:\n- https://dev.rise.ai/authentication/oauth\ndescription: OAuth 2.0 Authentication\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The process uses a client_credentials OAuth flow scoped by a unique instanceId for each merchant who installs your app.\n  location: body\n  token_url: https://platform.rise.ai/oauth2/token\n  how_to_obtain: Exchange your app credentials (client_id and client_secret) and the merchant's instanceId for an access token via a POST request\n    to the token URL.\ndocs: https://dev.rise.ai/authentication/oauth\n"
source_yaml_url: https://artifacts.apis.io/rise-ai/authentication/rise-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
