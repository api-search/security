---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agent Letter Desk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Letter Desk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Letter Desk
provider_slug: agentletterdesk-com
scheme_count: 1
schemes:
- authorize_url: https://agentletterdesk.com/authorize
  evidence: 'Authorization: OAuth 2.1 with the authorization code grant and PKCE (S256).'
  flows:
  - authorization_code
  how_to_obtain: Register your client via a Client ID Metadata Document or dynamic client registration at https://agentletterdesk.com/oauth/register, then follow the authorization code flow with PKCE.
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - letters.read
  - letters.write
  type: oauth2
slug: agentletterdesk-com-authentication
source_filename: agentletterdesk-com-authentication.yml
source_heading: Authentication Profile
source_url: https://agentletterdesk.com/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentletterdesk.com/.well-known/oauth-protected-resource/mcp\nsources:\n- https://agentletterdesk.com/.well-known/oauth-protected-resource/mcp\n- https://agentletterdesk.com/auth.md\nschemes:\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: 'Authorization: OAuth 2.1 with the authorization code grant and PKCE (S256).'\n  flows:\n  - authorization_code\n  authorize_url: https://agentletterdesk.com/authorize\n  scopes:\n  - letters.read\n  - letters.write\n  how_to_obtain: Register your client via a Client ID Metadata Document or dynamic client registration at https://agentletterdesk.com/oauth/register,\n    then follow the authorization code flow with PKCE.\ndocs: https://agentletterdesk.com/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/agentletterdesk-com/authentication/agentletterdesk-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Mail
- Certified Mail
- LetterService
- Automation
- Company
---
