---
anonymous_access: false
api_key_in: []
auth_types: []
description: Mailbox MCP uses OAuth2 with dynamic client registration; clients provide the connector URL, are redirected to sign in, and receive an access token used as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailbox MCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailbox MCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mailbox MCP
provider_slug: mailbox-mcp-com
scheme_count: 1
schemes:
- evidence: This server does dynamic client registration, the part of the OAuth specification that lets a client introduce itself and be issued credentials on the spot.
  flows:
  - authorization_code
  how_to_obtain: Client sends the connector URL, is redirected to the provider’s sign‑in page, authorizes, and receives an access token.
  name: OAuth2 Dynamic Registration
  type: oauth2
slug: mailbox-mcp-com-authentication
source_filename: mailbox-mcp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mailbox-mcp.com/docs/
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailbox-mcp.com/docs/\nsources:\n- https://mailbox-mcp.com/docs/\ndescription: Mailbox MCP uses OAuth2 with dynamic client registration; clients provide the connector URL, are redirected to sign in, and receive\n  an access token used as a Bearer token in the Authorization header.\nschemes:\n- type: oauth2\n  name: OAuth2 Dynamic Registration\n  evidence: This server does dynamic client registration, the part of the OAuth specification that lets a client introduce itself and be issued\n    credentials on the spot.\n  flows:\n  - authorization_code\n  how_to_obtain: Client sends the connector URL, is redirected to the provider’s sign‑in page, authorizes, and receives an access token.\nnote: No explicit token or authorize URLs, header names, or scopes are listed on the page.\ndocs: https://mailbox-mcp.com/docs/\n"
source_yaml_url: https://artifacts.apis.io/mailbox-mcp-com/authentication/mailbox-mcp-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- AI Integration
- Calendar
- Attachments
---
