---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Vectoree Auth APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vectoree Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vectoree declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vectoree
provider_slug: vectoree
scheme_count: 1
schemes:
- evidence: 'Send the project API Key with `auth:*` as `Authorization: Bearer`.'
  header: Authorization
  how_to_obtain: 'Server calls use a project API key with `auth:*` as `Authorization: Bearer`.'
  location: header
  name: Project API Key
  type: http-bearer
slug: vectoree-authentication
source_filename: vectoree-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.vectoree.ai/auth.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.vectoree.ai/auth.md\nsources:\n- https://docs.vectoree.ai/auth.md\n- https://docs.vectoree.ai/api-reference/client/initiate-oauth-flow-pkce.md\n- https://docs.vectoree.ai/api-reference/client/exchange-oauth-code-for-tokens-pkce.md\n- https://docs.vectoree.ai/api-reference/client/shared-oauth-callback-handler.md\ndescription: Authentication schemes for Vectoree Auth APIs\nschemes:\n- type: http-bearer\n  name: Project API Key\n  evidence: 'Send the project API Key with `auth:*` as `Authorization: Bearer`.'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Server calls use a project API key with `auth:*` as `Authorization: Bearer`.'\nnote: OAuth flows (PKCE) are described in separate endpoints but no OAuth2 security scheme is defined on the API; token exchange is performed\n  via the `/api/auth/oauth/exchange` endpoint.\ndocs: https://docs.vectoree.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/vectoree/authentication/vectoree-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Backend-as-a-Service
- OpenAI-Compatible
- Agents
---
