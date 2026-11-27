---
anonymous_access: false
api_key_in: []
api_specs:
- filename: neverapply-co-expiredjobs-api-openapi.yml
  format: yaml
  label: NeverApply Expired Jobs API
  slug: neverapply-co-expiredjobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-expiredjobs-api-openapi.yml
- filename: neverapply-co-feed-api-openapi.yml
  format: yaml
  label: NeverApply Feed API
  slug: neverapply-co-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-feed-api-openapi.yml
- filename: neverapply-co-jobs-api-openapi.yml
  format: yaml
  label: NeverApply Jobs API
  slug: neverapply-co-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-jobs-api-openapi.yml
- filename: neverapply-co-meta-api-openapi.yml
  format: yaml
  label: NeverApply Meta API
  slug: neverapply-co-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-meta-api-openapi.yml
- filename: neverapply-co-search-api-openapi.yml
  format: yaml
  label: NeverApply Search API
  slug: neverapply-co-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neverapply-co/openapi/neverapply-co-search-api-openapi.yml
auth_types: []
description: NeverApply authentication methods
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NeverApply Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeverApply declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NeverApply
provider_slug: neverapply-co
scheme_count: 2
schemes:
- authorize_url: https://neverapply.co/oauth/authorize
  evidence: Open `https://neverapply.co/oauth/authorize` in the user's browser with `response_type=code`, `client_id`, the exact `redirect_uri`, a fresh unpredictable `state`, requested `scope`, `code_challenge_method=S256`, the derived `code_challenge`, and `resource` from discovery.
  flows:
  - authorization_code
  how_to_obtain: 'Register a public OAuth client with `token_endpoint_auth_method: none` (via CIMD or DCR) and use PKCE. No client secret is required.'
  name: OAuth2 Authorization Code
  scopes:
  - mcp:read
  - mcp:write
  - mcp:apply
  type: oauth2
- evidence: Provide your bearer token in the Authorization header when making requests to protected resources.
  header: Authorization
  how_to_obtain: Create a bearer token from the Developer Dashboard.
  location: header
  name: Bearer Auth
  type: http-bearer
slug: neverapply-co-authentication
source_filename: neverapply-co-authentication.yml
source_heading: Authentication Profile
source_url: https://neverapply.co/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://neverapply.co/auth.md\nsources:\n- https://neverapply.co/auth.md\n- https://neverapply.co/docs/api#/#authentication\n- https://neverapply.co/docs/api#/\n- https://neverapply.co/features/mcp#connector-guide\ndescription: NeverApply authentication methods\nschemes:\n- type: oauth2\n  name: OAuth2 Authorization Code\n  evidence: Open `https://neverapply.co/oauth/authorize` in the user's browser with `response_type=code`, `client_id`, the exact `redirect_uri`,\n    a fresh unpredictable `state`, requested `scope`, `code_challenge_method=S256`, the derived `code_challenge`, and `resource` from discovery.\n  flows:\n  - authorization_code\n  authorize_url: https://neverapply.co/oauth/authorize\n  scopes:\n  - mcp:read\n  - mcp:write\n  - mcp:apply\n  how_to_obtain: 'Register a public OAuth client with `token_endpoint_auth_method: none` (via CIMD or DCR) and use PKCE. No client\
  \ secret is required.'\n- type: http-bearer\n  name: Bearer Auth\n  evidence: Provide your bearer token in the Authorization header when making requests to protected resources.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a bearer token from the Developer Dashboard.\ndocs: https://neverapply.co/auth.md\n"
source_yaml_url: https://artifacts.apis.io/neverapply-co/authentication/neverapply-co-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Job Search
- Automation
- Recruiting
- Software-as-a-Service
---
