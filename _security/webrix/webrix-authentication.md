---
anonymous_access: false
api_key_in: []
api_specs:
- filename: webrix-api-openapi.json
  format: json
  label: Willow API API
  slug: willow-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/webrix/openapi/_original/webrix-api-openapi.json
auth_types: []
description: Authentication schemes published for Willow AI Governance Control Plane
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Webrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Willow AI Governance Control Plane declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Willow AI Governance Control Plane
provider_slug: webrix
scheme_count: 2
schemes:
- evidence: 'By default, Willow sends the user''s key as the raw value of the Authorization header, with no Bearer prefix: Authorization: <user-api-key>'
  header: Authorization
  how_to_obtain: User supplies a per‑user API key; Willow forwards it in the Authorization header.
  location: header
  name: Authorization
  type: apiKey
- authorize_url: https://<org>.connect.your-domain.com/authorize
  evidence: Willow exposes a full OAuth 2.0 / OpenID Connect authorization server that HTTP MCP clients use to authenticate users.
  flows:
  - authorization_code
  - client_credentials
  - refresh_token
  how_to_obtain: Clients register via the dynamic client registration endpoint (/register) to receive a client_id and client_secret.
  name: Willow OAuth Authorization Server
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: webrix-authentication
source_filename: webrix-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.withwillow.ai/docs/admin/sso-and-auth/enterprise-managed-authentication
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.withwillow.ai/docs/admin/sso-and-auth/enterprise-managed-authentication\nsources:\n- https://docs.withwillow.ai/docs/admin/sso-and-auth/enterprise-managed-authentication\n- https://docs.withwillow.ai/docs/advanced-capabilities/oauth-authorization-server\n- https://docs.withwillow.ai/docs/deployment/run-hosted-oauth\n- https://docs.withwillow.ai/docs/developers/accept-api-keys\ndescription: Authentication schemes published for Willow AI Governance Control Plane\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'By default, Willow sends the user''s key as the raw value of the Authorization header, with no Bearer prefix: Authorization: <user-api-key>'\n  location: header\n  header: Authorization\n  how_to_obtain: User supplies a per‑user API key; Willow forwards it in the Authorization header.\n- type: oauth2\n  name: Willow OAuth Authorization Server\n  evidence:\
  \ Willow exposes a full OAuth 2.0 / OpenID Connect authorization server that HTTP MCP clients use to authenticate users.\n  flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  authorize_url: https://<org>.connect.your-domain.com/authorize\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Clients register via the dynamic client registration endpoint (/register) to receive a client_id and client_secret.\ndocs: https://docs.withwillow.ai/docs/admin/sso-and-auth/enterprise-managed-authentication\n"
source_yaml_url: https://artifacts.apis.io/webrix/authentication/webrix-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Governance
- Platform
- Enterprise
---
