---
anonymous_access: false
api_key_in: []
api_specs:
- filename: endpointblank-agent-oauth-api-openapi.yml
  format: yaml
  label: Bengal Technologies Agent Oauth API
  slug: endpointblank-agent-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-agent-oauth-api-openapi.yml
- filename: endpointblank-api-packages-api-openapi.yml
  format: yaml
  label: Bengal Technologies Api Packages API
  slug: endpointblank-api-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-api-packages-api-openapi.yml
- filename: endpointblank-applications-api-openapi.yml
  format: yaml
  label: Bengal Technologies Applications API
  slug: endpointblank-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-applications-api-openapi.yml
- filename: endpointblank-authorize-api-openapi.yml
  format: yaml
  label: Bengal Technologies Authorize API
  slug: endpointblank-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-authorize-api-openapi.yml
- filename: endpointblank-callback-api-openapi.yml
  format: yaml
  label: Bengal Technologies Callback API
  slug: endpointblank-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-callback-api-openapi.yml
- filename: endpointblank-clients-api-openapi.yml
  format: yaml
  label: Bengal Technologies Clients API
  slug: endpointblank-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-clients-api-openapi.yml
- filename: endpointblank-credentials-api-openapi.yml
  format: yaml
  label: Bengal Technologies Credentials API
  slug: endpointblank-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-credentials-api-openapi.yml
- filename: endpointblank-endpoints-api-openapi.yml
  format: yaml
  label: Bengal Technologies Endpoints API
  slug: endpointblank-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-endpoints-api-openapi.yml
- filename: endpointblank-environments-api-openapi.yml
  format: yaml
  label: Bengal Technologies Environments API
  slug: endpointblank-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-environments-api-openapi.yml
- filename: endpointblank-organization-api-openapi.yml
  format: yaml
  label: Bengal Technologies Organization API
  slug: endpointblank-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-organization-api-openapi.yml
- filename: endpointblank-well-known-api-openapi.yml
  format: yaml
  label: Bengal Technologies .well Known API
  slug: endpointblank-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/endpointblank-well-known-api-openapi.yml
auth_types: []
description: Authentication methods as published on the EndPointBlank documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Endpointblank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bengal Technologies declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bengal Technologies
provider_slug: endpointblank
scheme_count: 2
schemes:
- authorize_url: https://app.endpointblank.com/agent-oauth/authorize
  evidence: EndPointBlank is an OAuth 2.1 authorization server for AI agents such as MCP clients.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Dynamic client registration via POST to https://app.endpointblank.com/agent-oauth/register returns a client_id; no client secret is issued.
  name: Agent OAuth
  type: oauth2
- evidence: Send no client secret and no Authorization header.
  how_to_obtain: Use the client_id obtained from registration; include it in the request body.
  name: Token endpoint
  token_url: https://app.endpointblank.com/agent-oauth/token
  type: oauth2
slug: endpointblank-authentication
source_filename: endpointblank-authentication.yml
source_heading: Authentication Profile
source_url: https://endpointblank.com/docs/agent-sign-in
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://endpointblank.com/docs/agent-sign-in\nsources:\n- https://endpointblank.com/docs/agent-sign-in\n- https://endpointblank.com/docs/credentials\n- https://endpointblank.com/docs/quickstart\n- https://endpointblank.com/docs/api-concepts\ndescription: Authentication methods as published on the EndPointBlank documentation.\nschemes:\n- type: oauth2\n  name: Agent OAuth\n  evidence: EndPointBlank is an OAuth 2.1 authorization server for AI agents such as MCP clients.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://app.endpointblank.com/agent-oauth/authorize\n  how_to_obtain: Dynamic client registration via POST to https://app.endpointblank.com/agent-oauth/register returns a client_id; no client secret\n    is issued.\n- type: oauth2\n  name: Token endpoint\n  evidence: Send no client secret and no Authorization header.\n  token_url: https://app.endpointblank.com/agent-oauth/token\n\
  \  how_to_obtain: Use the client_id obtained from registration; include it in the request body.\ndocs: https://endpointblank.com/docs/agent-sign-in\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/authentication/endpointblank-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API Management
- Versioning
- Authentication
- Monitoring
---
