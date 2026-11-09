---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bluenexus-ai-openapi-generated.yml
  format: yaml
  label: BlueNexus AI API
  slug: bluenexus-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bluenexus-ai/openapi/_ae-authored/bluenexus-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for BlueNexus AI
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bluenexus Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlueNexus AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BlueNexus AI
provider_slug: bluenexus-ai
scheme_count: 2
schemes:
- authorize_url: GET /v1/auth/authorize
  evidence: The primary auth method for third-party apps. BlueNexus implements OAuth 2.1 with mandatory PKCE (S256 only — PLAIN is not allowed).
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Dynamic Client Registration via POST /v1/auth/register or manual registration via the dashboard or API.
  name: OAuth 2.1 with PKCE
  scopes:
  - universal-mcp-read
  - universal-mcp-read-write
  - llm-all
  - agents-all
  - agents-use
  - connections
  - account
  - user-data
  - providers
  - openid
  - profile
  - email
  type: oauth2
- evidence: Personal Access Tokens (PATs) are long-lived tokens for programmatic API access.
  header: Authorization
  how_to_obtain: Created via POST /v1/auth/pat or the dashboard.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: bluenexus-ai-authentication
source_filename: bluenexus-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bluenexus.ai/core-concepts/authentication-and-authorization/
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bluenexus.ai/core-concepts/authentication-and-authorization/\nsources:\n- https://docs.bluenexus.ai/core-concepts/authentication-and-authorization/\n- https://docs.bluenexus.ai/guides/authentication/oauth-for-your-app/\n- https://docs.bluenexus.ai/guides/authentication/white-label/\n- https://docs.bluenexus.ai/guides/authentication/personal-access-tokens/\ndescription: Authentication methods for BlueNexus AI\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: The primary auth method for third-party apps. BlueNexus implements OAuth 2.1 with mandatory PKCE (S256 only — PLAIN is not allowed).\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: GET /v1/auth/authorize\n  scopes:\n  - universal-mcp-read\n  - universal-mcp-read-write\n  - llm-all\n  - agents-all\n  - agents-use\n  - connections\n  - account\n  - user-data\n  - providers\n\
  \  - openid\n  - profile\n  - email\n  how_to_obtain: Dynamic Client Registration via POST /v1/auth/register or manual registration via the dashboard or API.\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Personal Access Tokens (PATs) are long-lived tokens for programmatic API access.\n  location: header\n  header: Authorization\n  how_to_obtain: Created via POST /v1/auth/pat or the dashboard.\ndocs: https://docs.bluenexus.ai/core-concepts/authentication-and-authorization/\n"
source_yaml_url: https://artifacts.apis.io/bluenexus-ai/authentication/bluenexus-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Platform
- Agent Management
- Collaboration
- Real-Time
---
