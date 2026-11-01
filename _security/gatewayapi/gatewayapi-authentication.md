---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gatewayapi-rest-api-openapi.yml
  format: yaml
  label: GatewayAPI REST API
  slug: gatewayapi-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatewayapi/openapi/gatewayapi-rest-api-openapi.yml
- filename: gatewayapi-openapi-generated.yml
  format: yaml
  label: GatewayAPI API
  slug: gatewayapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatewayapi/openapi/_ae-authored/gatewayapi-openapi-generated.yml
auth_types: []
description: Authentication methods documented for GatewayAPI
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Gatewayapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: GatewayAPI declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: GatewayAPI
provider_slug: gatewayapi
scheme_count: 4
schemes:
- evidence: The simplest form used for authentication is to just set the Authorization header with the token itself using the Token authorization scheme.
  header: Authorization
  how_to_obtain: API tokens are generated when creating an account and can be created or revoked from the dashboard.
  location: header
  name: Token
  type: other
- evidence: The HTTP Basic authentication scheme is another method supported for backwards compatibility with older integrations.
  header: Authorization
  how_to_obtain: Legacy credentials (username and password) are provided in the dashboard under “Developer”, “Credentials”.
  location: header
  name: Basic
  type: http-basic
- evidence: The username is sent as user , and the password as password .
  how_to_obtain: Credentials (username and password) are available in the dashboard under “Developer”, “Credentials”.
  location: query
  name: Legacy query credentials
  type: apiKey
- evidence: GatewayAPI supports OAuth 1.0a for legacy integrations. No user interaction is required for the authentication, so this part is skipped from OAuth.
  header: Authorization
  how_to_obtain: Create an API key (consumer key) in the dashboard; the token and secret are left empty for the two‑legged flow.
  location: header
  name: OAuth 1.0a (two‑legged)
  type: other
slug: gatewayapi-authentication
source_filename: gatewayapi-authentication.yml
source_heading: Authentication Profile
source_url: https://gatewayapi.com/docs/authentication/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gatewayapi.com/docs/authentication/\nsources:\n- https://gatewayapi.com/docs/authentication/\n- https://gatewayapi.com/docs/authentication/\n- https://gatewayapi.com/docs/apis/legacy/authentication/\n- https://gatewayapi.com/eu-setup/\ndescription: Authentication methods documented for GatewayAPI\nschemes:\n- type: other\n  name: Token\n  evidence: The simplest form used for authentication is to just set the Authorization header with the token itself using the Token authorization\n    scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: API tokens are generated when creating an account and can be created or revoked from the dashboard.\n- type: http-basic\n  name: Basic\n  evidence: The HTTP Basic authentication scheme is another method supported for backwards compatibility with older integrations.\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Legacy credentials (username and password) are provided in the dashboard under “Developer”, “Credentials”.\n- type: apiKey\n  name: Legacy query credentials\n  evidence: The username is sent as user , and the password as password .\n  location: query\n  how_to_obtain: Credentials (username and password) are available in the dashboard under “Developer”, “Credentials”.\n- type: other\n  name: OAuth 1.0a (two‑legged)\n  evidence: GatewayAPI supports OAuth 1.0a for legacy integrations. No user interaction is required for the authentication, so this part is skipped\n    from OAuth.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key (consumer key) in the dashboard; the token and secret are left empty for the two‑legged flow.\nnote: No OAuth2 flows are documented; only OAuth 1.0a is mentioned.\ndocs: https://gatewayapi.com/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/gatewayapi/authentication/gatewayapi-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Messaging
- SMS
- API
- Communications
---
