---
api_key_in:
- header
api_specs:
- filename: stacklok-toolhive-api-openapi.yml
  format: yaml
  label: ToolHive API
  slug: toolhive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-toolhive-api-openapi.yml
- filename: stacklok-registry-api-openapi.yml
  format: yaml
  label: ToolHive Registry API
  slug: toolhive-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-registry-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Stacklok Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stacklok secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stacklok
provider_slug: stacklok
scheme_count: 1
schemes:
- description: 'OAuth 2.0 / OIDC Bearer token authentication. Format: "Bearer {token}"'
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/stacklok-registry-api-openapi.yml
  type: apiKey
slug: stacklok-authentication
source_filename: stacklok-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stacklok-registry-api-openapi.yml, openapi/stacklok-toolhive-api-openapi.yml\ndocs: https://docs.stacklok.com\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  detail: >-\n    The ToolHive Registry API requires OAuth 2.0 / OIDC Bearer access tokens in the\n    Authorization header (Authorization: Bearer {token}). OAuth discovery metadata is\n    published at /.well-known/oauth-protected-resource (RFC 9728). Enterprise deployments\n    integrate external identity providers (Okta, Auth0, Microsoft Entra ID) for OIDC\n    sign-in; an anonymous mode is available for local development. The local ToolHive\n    control API (thv serve) does not declare an in-spec security scheme.\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'OAuth 2.0 / OIDC Bearer token authentication. Format: \"Bearer {token}\"'\n  sources:\n  - openapi/stacklok-registry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/authentication/stacklok-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Open Source
- MCP
- AI Agents
- API Governance
- Security
- Model Context Protocol
- Developer Tools
---
