---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 42min-us-api-openapi.yml
  format: yaml
  label: 42min API API
  slug: 42min-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/42min-us/openapi/_original/42min-us-api-openapi.yml
auth_types: []
description: Authentication — Help — 42min
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: 42Min Us Authentication
name_suffix: Authentication
oauth_flows: []
overview: 42min declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 42min
provider_slug: 42min-us
scheme_count: 3
schemes:
- evidence: 'Every request to /v1/* must carry a bearer token: Authorization: Bearer <token>'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: Prefix Type Use for 42min_pat_… Personal access token (PAT) Server-side scripts and integrations that act as your own account.
  header: Authorization
  how_to_obtain: Open Admin Center → API and switch to the API keys tab. Click New API key, give it a name, pick the scopes you want it to hold, and optionally set an expiry. Copy the token that appears.
  location: header
  name: Personal Access Token (PAT)
  type: http-bearer
- authorize_url: https://api.42min.us/v1/oauth/authorize
  evidence: OAuth 2.1 + PKCE For third-party applications that act on behalf of a 42min user, use the OAuth 2.1 authorization code flow with PKCE (S256).
  header: Authorization
  how_to_obtain: Register an OAuth client in Admin Center → API → OAuth apps tab, then follow the authorization code flow with PKCE as described.
  location: header
  name: OAuth 2.1
  scopes:
  - event_types:read
  - slots:read
  - bookings:write
  token_url: https://api.42min.us/v1/oauth/token
  type: oauth2
slug: 42min-us-authentication
source_filename: 42min-us-authentication.yml
source_heading: Authentication Profile
source_url: https://42min.us/help/api/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://42min.us/help/api/authentication\nsources:\n- https://42min.us/help/api/authentication\n- https://42min.us/help/getting-started/what-is-42min\n- https://42min.us/help/getting-started/connecting-your-calendar\n- https://42min.us/help/getting-started/setting-your-availability\ndescription: Authentication — Help — 42min\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request to /v1/* must carry a bearer token: Authorization: Bearer <token>'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Personal Access Token (PAT)\n  evidence: Prefix Type Use for 42min_pat_… Personal access token (PAT) Server-side scripts and integrations that act as your own account.\n  location: header\n  header: Authorization\n  how_to_obtain: Open Admin Center → API and switch to the API keys tab. Click New API key, give it a name, pick the scopes you want\
  \ it to hold,\n    and optionally set an expiry. Copy the token that appears.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: OAuth 2.1 + PKCE For third-party applications that act on behalf of a 42min user, use the OAuth 2.1 authorization code flow with PKCE\n    (S256).\n  location: header\n  header: Authorization\n  token_url: https://api.42min.us/v1/oauth/token\n  authorize_url: https://api.42min.us/v1/oauth/authorize\n  scopes:\n  - event_types:read\n  - slots:read\n  - bookings:write\n  how_to_obtain: Register an OAuth client in Admin Center → API → OAuth apps tab, then follow the authorization code flow with PKCE as described.\ndocs: https://42min.us/help/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/42min-us/authentication/42min-us-authentication.yml
summary_line: 3 schemes
tags:
- Scheduling
- Free
- Webhook
- Automation
---
