---
anonymous_access: false
api_key_in: []
api_specs:
- filename: host-tracker-com-openapi-generated.yml
  format: yaml
  label: HostTracker API
  slug: host-tracker-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/host-tracker-com/openapi/_ae-authored/host-tracker-com-openapi-generated.yml
auth_types: []
description: Authentication methods for HostTracker API and MCP server
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: HostTracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: HostTracker declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: HostTracker
provider_slug: host-tracker-com
scheme_count: 3
schemes:
- evidence: 'The API (api2.host-tracker.com) is also reachable with a per-user API token: sign in, then mint one under Integrations > API in the account, scoped per resource family'
  header: Authorization
  how_to_obtain: Sign in to the HostTracker web UI, then mint a token under Integrations → API
  location: header
  name: API token
  type: http-bearer
- authorize_url: https://www.host-tracker.com/oauth/authorize
  evidence: It accepts the same bearer tokens AND supports the full OAuth 2.1 flow below — MCP clients (Claude, ChatGPT, and others) can connect with no manual token handling.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Perform OAuth 2.1 Authorization Code flow with PKCE as described in the auth.md document
  location: header
  name: MCP bearer token (OAuth 2.1)
  scopes:
  - check
  - monitor:read
  token_url: https://api2.host-tracker.com/oauth/token
  type: http-bearer
- evidence: The customer dashboard uses session-cookie authentication, issued by signing in as a human through the web UI at /user/signin.
  how_to_obtain: Sign in via the web UI at /user/signin to receive a session cookie
  location: cookie
  name: Session cookie
  type: other
slug: host-tracker-com-authentication
source_filename: host-tracker-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.host-tracker.com/en/ic/email-auth-check
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.host-tracker.com/en/ic/email-auth-check\nsources:\n- https://www.host-tracker.com/en/ic/email-auth-check\n- https://www.host-tracker.com/auth.md\n- https://docs.host-tracker.com/getting-started/quickstart/\ndescription: Authentication methods for HostTracker API and MCP server\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: 'The API (api2.host-tracker.com) is also reachable with a per-user API token: sign in, then mint one under Integrations > API in the\n    account, scoped per resource family'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to the HostTracker web UI, then mint a token under Integrations → API\n- type: http-bearer\n  name: MCP bearer token (OAuth 2.1)\n  evidence: It accepts the same bearer tokens AND supports the full OAuth 2.1 flow below — MCP clients (Claude, ChatGPT, and others) can connect\n    with no manual\
  \ token handling.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  token_url: https://api2.host-tracker.com/oauth/token\n  authorize_url: https://www.host-tracker.com/oauth/authorize\n  scopes:\n  - check\n  - monitor:read\n  how_to_obtain: Perform OAuth 2.1 Authorization Code flow with PKCE as described in the auth.md document\n- type: other\n  name: Session cookie\n  evidence: The customer dashboard uses session-cookie authentication, issued by signing in as a human through the web UI at /user/signin.\n  location: cookie\n  how_to_obtain: Sign in via the web UI at /user/signin to receive a session cookie\ndocs: https://www.host-tracker.com/en/ic/email-auth-check\n"
source_yaml_url: https://artifacts.apis.io/host-tracker-com/authentication/host-tracker-com-authentication.yml
summary_line: 3 schemes
tags:
- Monitoring
- Uptime
- Websites
- Alerts
- Software-as-a-Service
---
