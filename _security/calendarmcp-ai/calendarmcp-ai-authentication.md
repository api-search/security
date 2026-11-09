---
anonymous_access: false
api_key_in: []
api_specs:
- filename: calendarmcp-ai-openapi-generated.yml
  format: yaml
  label: CalendarMCP API
  slug: calendarmcp-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendarmcp-ai/openapi/_ae-authored/calendarmcp-ai-openapi-generated.yml
auth_types: []
description: Authentication methods published by CalendarMCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Calendarmcp Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: CalendarMCP declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CalendarMCP
provider_slug: calendarmcp-ai
scheme_count: 2
schemes:
- evidence: Recover without guessing Open the dashboard while signed in and identify the failing account, not merely the key that reported an error. If the account says Revoked, use its reconnect action and complete Google consent for that same account.
  flows:
  - authorization_code
  how_to_obtain: User grants consent via Google OAuth flow; a refresh token is issued and used for subsequent calls.
  name: Google OAuth
  type: oauth2
- evidence: Update the bearer token in each client configuration.
  header: Authorization
  how_to_obtain: Create or rotate an API key in the CalendarMCP dashboard; the key is used as a bearer token.
  location: header
  name: CalendarMCP API key
  type: http-bearer
slug: calendarmcp-ai-authentication
source_filename: calendarmcp-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://calendarmcp.ai/blog/calendar-mcp-oauth-revoked-reconnect
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://calendarmcp.ai/blog/calendar-mcp-oauth-revoked-reconnect\nsources:\n- https://calendarmcp.ai/blog/calendar-mcp-oauth-revoked-reconnect\n- https://calendarmcp.ai/blog/calendar-mcp-api-key-rotation-guide\n- https://calendarmcp.ai/blog/one-api-key-many-google-calendars\ndescription: Authentication methods published by CalendarMCP\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: Recover without guessing Open the dashboard while signed in and identify the failing account, not merely the key that reported an\n    error. If the account says Revoked, use its reconnect action and complete Google consent for that same account.\n  flows:\n  - authorization_code\n  how_to_obtain: User grants consent via Google OAuth flow; a refresh token is issued and used for subsequent calls.\n- type: http-bearer\n  name: CalendarMCP API key\n  evidence: Update the bearer token in each\
  \ client configuration.\n  location: header\n  header: Authorization\n  how_to_obtain: Create or rotate an API key in the CalendarMCP dashboard; the key is used as a bearer token.\ndocs: https://calendarmcp.ai/blog/calendar-mcp-oauth-revoked-reconnect\n"
source_yaml_url: https://artifacts.apis.io/calendarmcp-ai/authentication/calendarmcp-ai-authentication.yml
summary_line: 2 schemes
tags:
- Calendar
- Artificial Intelligence
- MCP
- Google Calendar
- Integration
---
