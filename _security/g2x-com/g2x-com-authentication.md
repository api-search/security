---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for G2X MCP server
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: g2x-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: g2x-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: g2x-com
provider_slug: g2x-com
scheme_count: 1
schemes:
- evidence: Read the authorization server's metadata and follow its authorization-code flow with PKCE, using S256.
  flows:
  - authorization_code
  how_to_obtain: Register with dynamic client registration (RFC 7591) at the registration_endpoint the authorization server's metadata lists.
  name: OAuth 2.1 Authorization Code with PKCE
  type: oauth2
slug: g2x-com-authentication
source_filename: g2x-com-authentication.yml
source_heading: Authentication Profile
source_url: https://g2x.com/docs/developers/authentication
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://g2x.com/docs/developers/authentication\nsources:\n- https://g2x.com/docs/developers/authentication\ndescription: Authentication schemes for G2X MCP server\nschemes:\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: Read the authorization server's metadata and follow its authorization-code flow with PKCE, using S256.\n  flows:\n  - authorization_code\n  how_to_obtain: Register with dynamic client registration (RFC 7591) at the registration_endpoint the authorization server's metadata lists.\ndocs: https://g2x.com/docs/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/g2x-com/authentication/g2x-com-authentication.yml
summary_line: 1 scheme
tags:
- GovCon
- Market Intelligence
- Bid Management
- Pipeline Management
- AI Platform
- Procurement
---
