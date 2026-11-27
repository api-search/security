---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lightbringer-com-oauth-api-openapi.yml
  format: yaml
  label: Lightbringer OAuth API
  slug: lightbringer-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-oauth-api-openapi.yml
- filename: lightbringer-com-public-api-openapi.yml
  format: yaml
  label: Lightbringer Public API
  slug: lightbringer-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-public-api-openapi.yml
- filename: lightbringer-com-well-known-api-openapi.yml
  format: yaml
  label: Lightbringer .well Known API
  slug: lightbringer-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-well-known-api-openapi.yml
auth_types: []
description: Authentication methods published by Lightbringer
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lightbringer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightbringer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lightbringer
provider_slug: lightbringer-com
scheme_count: 2
schemes:
- authorize_url: https://app.lightbringer.com/api/oauth/authorize
  evidence: '"grant_types_supported":["authorization_code","refresh_token"]'
  flows:
  - authorization_code
  name: OAuth2
  scopes:
  - mcp:read
  - mcp:write
  type: oauth2
- evidence: '"bearer_methods_supported":["header"]'
  header: Authorization
  location: header
  name: Bearer Token
  type: http-bearer
slug: lightbringer-com-authentication
source_filename: lightbringer-com-authentication.yml
source_heading: Authentication Profile
source_url: https://app.lightbringer.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.lightbringer.com/.well-known/oauth-authorization-server\nsources:\n- https://app.lightbringer.com/.well-known/oauth-authorization-server\n- https://app.lightbringer.com/.well-known/oauth-protected-resource\ndescription: Authentication methods published by Lightbringer\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"grant_types_supported\":[\"authorization_code\",\"refresh_token\"]'\n  flows:\n  - authorization_code\n  authorize_url: https://app.lightbringer.com/api/oauth/authorize\n  scopes:\n  - mcp:read\n  - mcp:write\n- type: http-bearer\n  name: Bearer Token\n  evidence: '\"bearer_methods_supported\":[\"header\"]'\n  location: header\n  header: Authorization\ndocs: https://app.lightbringer.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/lightbringer-com/authentication/lightbringer-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Patents
- Deep Tech
- Startups
- Platform
---
