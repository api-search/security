---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outpost-ai-oauth-api-openapi.yml
  format: yaml
  label: Outpost OAuth API
  slug: outpost-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-oauth-api-openapi.yml
- filename: outpost-ai-payments-api-openapi.yml
  format: yaml
  label: Outpost Payments API
  slug: outpost-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-payments-api-openapi.yml
- filename: outpost-ai-webhooks-api-openapi.yml
  format: yaml
  label: Outpost Webhooks API
  slug: outpost-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Outpost API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Outpost Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outpost declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Outpost
provider_slug: outpost-ai
scheme_count: 1
schemes:
- evidence: Outpost uses OAuth2 client_credentials for server-to-server calls.
  flows:
  - client_credentials
  how_to_obtain: Generate a client_id and api_token in the merchant portal, then exchange them for an access_token via the token endpoint.
  name: OAuth2
  token_url: https://access.outpostanywhere.com/oauth2/token
  type: oauth2
slug: outpost-ai-authentication
source_filename: outpost-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://outpost.ai/docs/authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://outpost.ai/docs/authentication\nsources:\n- https://outpost.ai/docs/authentication\n- https://outpost.ai/docs/account-setup\ndescription: Authentication schemes for Outpost API\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: Outpost uses OAuth2 client_credentials for server-to-server calls.\n  flows:\n  - client_credentials\n  token_url: https://access.outpostanywhere.com/oauth2/token\n  how_to_obtain: Generate a client_id and api_token in the merchant portal, then exchange them for an access_token via the token endpoint.\ndocs: https://outpost.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/outpost-ai/authentication/outpost-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Tax
- Commerce
- SaaS
---
