---
anonymous_access: false
api_key_in: []
api_specs:
- filename: onetapvote-com-openapi-generated.yml
  format: yaml
  label: OneTapVote API
  slug: onetapvote-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onetapvote-com/openapi/_ae-authored/onetapvote-com-openapi-generated.yml
auth_types: []
description: Authentication methods for OneTapVote API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: OneTapVote Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneTapVote declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OneTapVote
provider_slug: onetapvote-com
scheme_count: 2
schemes:
- evidence: 'Option 1: OAuth 2.1 (MCP connectors, recommended)'
  flows:
  - authorization_code
  how_to_obtain: 'Register the client via Dynamic Client Registration at the registration_endpoint (no initial access token needed; public client uses token_endpoint_auth_method: none), then send the person to the authorization_endpoint to obtain an authorization code with PKCE, exchange the code at the token_endpoint for an access token.'
  name: OAuth 2.1
  type: oauth2
- evidence: 'Send `Authorization: Bearer otv_live_…` to the REST API or the MCP server.'
  header: Authorization
  how_to_obtain: The person creates a key in their OneTapVote dashboard (Account settings, API tab) and gives it to you.
  location: header
  name: API key
  type: apiKey
slug: onetapvote-com-authentication
source_filename: onetapvote-com-authentication.yml
source_heading: Authentication Profile
source_url: https://onetapvote.com/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://onetapvote.com/auth.md\nsources:\n- https://onetapvote.com/auth.md\n- https://onetapvote.com/feedback-flow/use-cases/saas-onboarding-feedback\ndescription: Authentication methods for OneTapVote API\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'Option 1: OAuth 2.1 (MCP connectors, recommended)'\n  flows:\n  - authorization_code\n  how_to_obtain: 'Register the client via Dynamic Client Registration at the registration_endpoint (no initial access token needed; public client\n    uses token_endpoint_auth_method: none), then send the person to the authorization_endpoint to obtain an authorization code with PKCE, exchange\n    the code at the token_endpoint for an access token.'\n- type: apiKey\n  name: API key\n  evidence: 'Send `Authorization: Bearer otv_live_…` to the REST API or the MCP server.'\n  location: header\n  header: Authorization\n  how_to_obtain: The\
  \ person creates a key in their OneTapVote dashboard (Account settings, API tab) and gives it to you.\ndocs: https://onetapvote.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/onetapvote-com/authentication/onetapvote-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Reviews
- Polls
- Google
- Software-as-a-Service
---
