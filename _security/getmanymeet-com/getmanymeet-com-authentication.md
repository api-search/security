---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for ManyMeet MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ManyMeet Authentication
name_suffix: Authentication
oauth_flows: []
overview: ManyMeet declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ManyMeet
provider_slug: getmanymeet-com
scheme_count: 2
schemes:
- evidence: 'Authentication: OAuth 2.0 with dynamic discovery (RFC 8414 + RFC 9728)'
  how_to_obtain: User logs in via ManyMeet login page; a token is issued automatically after the OAuth login flow.
  name: OAuth 2.0
  type: oauth2
- evidence: 'Authorization: Bearer mm_your_key_here'
  header: Authorization
  how_to_obtain: Generate an API key in ManyMeet Profile settings under Agent Access → Generate API Key, then use it as a Bearer token in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: getmanymeet-com-authentication
source_filename: getmanymeet-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getmanymeet.com/guide/manymeet/connect-ai-assistant-oauth/
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getmanymeet.com/guide/manymeet/connect-ai-assistant-oauth/\nsources:\n- https://getmanymeet.com/guide/manymeet/connect-ai-assistant-oauth/\n- https://getmanymeet.com/guide/manymeet/connect-ai-assistant-api-key/\ndescription: Authentication methods for ManyMeet MCP server\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'Authentication: OAuth 2.0 with dynamic discovery (RFC 8414 + RFC 9728)'\n  how_to_obtain: User logs in via ManyMeet login page; a token is issued automatically after the OAuth login flow.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer mm_your_key_here'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in ManyMeet Profile settings under Agent Access → Generate API Key, then use it as a Bearer token in the\n    Authorization header.\ndocs: https://getmanymeet.com/guide/manymeet/connect-ai-assistant-oauth/\n"
source_yaml_url: https://artifacts.apis.io/getmanymeet-com/authentication/getmanymeet-com-authentication.yml
summary_line: 2 schemes
tags:
- Webinar
- Sales
- Marketing Automation
- Zoom Integration
- ManyMeet
---
