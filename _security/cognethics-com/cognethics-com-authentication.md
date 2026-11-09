---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cognethics-com-well-known-openapi.json
  format: json
  label: Cognethics Developer API .well-known API
  slug: cognethics-developer-api-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cognethics-com/openapi/_original/cognethics-com-well-known-openapi.json
auth_types: []
description: Authentication methods published by Cognethics
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cognethics Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognethics declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cognethics
provider_slug: cognethics-com
scheme_count: 3
schemes:
- authorize_url: https://your-tenant.cognethics.com/api/mcp/oauth/authorize/
  evidence: OAuth 2.1 with PKCE-S256 and Dynamic Client Registration (RFC 7591) for AI clients.
  flows:
  - authorization_code
  how_to_obtain: Register a client via POST https://{tenant}.cognethics.com/api/mcp/oauth/register/ or use Dynamic Client Registration.
  name: OAuth 2.1 with PKCE and Dynamic Client Registration
  scopes:
  - mcp:read
  - mcp:write
  - mcp:execute
  - spare_parts.view
  - spare_parts.add
  - spare_parts.change
  - spare_parts.delete
  type: oauth2
- evidence: SCIM v2 endpoints are protected by a per‑tenant bearer token, generated in Admin → Enterprise SSO → SCIM
  header: Authorization
  how_to_obtain: Mint a token in the Cognethics console (Admin → Enterprise SSO → SCIM).
  location: header
  name: SCIM bearer token
  type: http-bearer
- evidence: Cognethics acts as a Service Provider (SP) for SAML 2.0, accepting authentication assertions from your identity provider (IdP).
  how_to_obtain: Configure IdP metadata and upload SP metadata via the Cognethics console; authentication occurs via SAML POST to the ACS endpoint.
  name: SAML 2.0 Single Sign‑On
  type: other
slug: cognethics-com-authentication
source_filename: cognethics-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.cognethics.com/auth/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.cognethics.com/auth/\nsources:\n- https://developers.cognethics.com/auth/\n- https://developers.cognethics.com/auth/enterprise/\n- https://developers.cognethics.com/auth/enterprise/saml/\n- https://developers.cognethics.com/auth/enterprise/scim/\ndescription: Authentication methods published by Cognethics\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE and Dynamic Client Registration\n  evidence: OAuth 2.1 with PKCE-S256 and Dynamic Client Registration (RFC 7591) for AI clients.\n  flows:\n  - authorization_code\n  authorize_url: https://your-tenant.cognethics.com/api/mcp/oauth/authorize/\n  scopes:\n  - mcp:read\n  - mcp:write\n  - mcp:execute\n  - spare_parts.view\n  - spare_parts.add\n  - spare_parts.change\n  - spare_parts.delete\n  how_to_obtain: Register a client via POST https://{tenant}.cognethics.com/api/mcp/oauth/register/ or use Dynamic Client\
  \ Registration.\n- type: http-bearer\n  name: SCIM bearer token\n  evidence: SCIM v2 endpoints are protected by a per‑tenant bearer token, generated in Admin → Enterprise SSO → SCIM\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a token in the Cognethics console (Admin → Enterprise SSO → SCIM).\n- type: other\n  name: SAML 2.0 Single Sign‑On\n  evidence: Cognethics acts as a Service Provider (SP) for SAML 2.0, accepting authentication assertions from your identity provider (IdP).\n  how_to_obtain: Configure IdP metadata and upload SP metadata via the Cognethics console; authentication occurs via SAML POST to the ACS endpoint.\ndocs: https://developers.cognethics.com/auth/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/cognethics-com/authentication/cognethics-com-authentication.yml
summary_line: 3 schemes
tags:
- Enterprise
- Artificial Intelligence
- Knowledge Management
- Security
- Compliance
---
