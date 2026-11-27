---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for TheSignup API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: TheSignup Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheSignup declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TheSignup
provider_slug: thesignup-app
scheme_count: 2
schemes:
- evidence: API keys are long-lived bearer tokens, one per organization. Use them for first-party scripts, server-to-server integrations, and any agent acting as the org itself.
  header: Authorization
  how_to_obtain: Generate one via Account → Settings → API keys → New key.
  location: header
  name: API Key
  scopes:
  - signups:*
  - participants:*
  - analytics:read
  - ai:draft
  - reminders:send
  type: http-bearer
- authorize_url: https://thesignup.app/oauth/authorize
  evidence: Three-legged OAuth 2.1 + PKCE for third‑party apps acting on behalf of users.
  flows:
  - authorization_code
  - refresh_token
  - device_code
  how_to_obtain: Register an app via POST https://thesignup.app/oauth/register or use dynamic client registration.
  name: OAuth 2.1
  scopes:
  - signups:read
  - signups:write
  - participants:read
  - participants:write
  - register:write
  - analytics:read
  - ai:draft
  - reminders:send
  type: oauth2
slug: thesignup-app-authentication
source_filename: thesignup-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.thesignup.app/docs/auth/api-keys
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.thesignup.app/docs/auth/api-keys\nsources:\n- https://docs.thesignup.app/docs/auth/api-keys\n- https://docs.thesignup.app/docs/auth/oauth\n- https://docs.thesignup.app/docs/api/me/get\n- https://docs.thesignup.app/docs/api/webhooks/id/rotate/post\ndescription: Authentication methods for TheSignup API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: API keys are long-lived bearer tokens, one per organization. Use them for first-party scripts, server-to-server integrations, and\n    any agent acting as the org itself.\n  location: header\n  header: Authorization\n  scopes:\n  - signups:*\n  - participants:*\n  - analytics:read\n  - ai:draft\n  - reminders:send\n  how_to_obtain: Generate one via Account → Settings → API keys → New key.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Three-legged OAuth 2.1 + PKCE for third‑party apps acting on behalf of users.\n\
  \  flows:\n  - authorization_code\n  - refresh_token\n  - device_code\n  authorize_url: https://thesignup.app/oauth/authorize\n  scopes:\n  - signups:read\n  - signups:write\n  - participants:read\n  - participants:write\n  - register:write\n  - analytics:read\n  - ai:draft\n  - reminders:send\n  how_to_obtain: Register an app via POST https://thesignup.app/oauth/register or use dynamic client registration.\ndocs: https://docs.thesignup.app/docs/auth/api-keys\n"
source_yaml_url: https://artifacts.apis.io/thesignup-app/authentication/thesignup-app-authentication.yml
summary_line: 2 schemes
tags:
- Event Signups
- Potluck
- Class Parties
- No‑App Signups
---
