---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Kinjay supports one method: the OAuth 2.1 authorization-code flow with PKCE, completed by the user in a browser.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kinjay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kinjay declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kinjay
provider_slug: kinjay-com
scheme_count: 1
schemes:
- evidence: 'Kinjay supports one method: the OAuth 2.1 authorization-code flow with PKCE, completed by the user in a browser.'
  flows:
  - authorization_code
  how_to_obtain: Register the agent's own OAuth client with the authorization server as advertised in its metadata, then start the authorization‑code flow with PKCE and request the scopes listed in the metadata's `scopes_supported`.
  name: OAuth 2.1 authorization-code
  scopes:
  - openid
  type: oauth2
slug: kinjay-com-authentication
source_filename: kinjay-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.kinjay.com/auth.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.kinjay.com/auth.md\nsources:\n- https://mcp.kinjay.com/auth.md\ndescription: 'Kinjay supports one method: the OAuth 2.1 authorization-code flow with PKCE, completed by the user in a browser.'\nschemes:\n- type: oauth2\n  name: OAuth 2.1 authorization-code\n  evidence: 'Kinjay supports one method: the OAuth 2.1 authorization-code flow with PKCE, completed by the user in a browser.'\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  how_to_obtain: Register the agent's own OAuth client with the authorization server as advertised in its metadata, then start the authorization‑code\n    flow with PKCE and request the scopes listed in the metadata's `scopes_supported`.\nnote: 'The access token is sent as `Authorization: Bearer <token>` in the request header.'\ndocs: https://mcp.kinjay.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/kinjay-com/authentication/kinjay-com-authentication.yml
summary_line: 1 scheme
tags:
- Health
- Family
- SMS
- Medical Records
- Privacy
---
