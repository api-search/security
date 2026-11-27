---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alloy-cx-openapi-generated.yml
  format: yaml
  label: Alloy API
  slug: alloy-cx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alloy-cx/openapi/_ae-authored/alloy-cx-openapi-generated.yml
auth_types: []
description: Alloy uses cookie‑based session authentication and optional LDAP form credentials.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Alloy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alloy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Alloy
provider_slug: alloy-cx
scheme_count: 2
schemes:
- evidence: Sessions use cookie‑based auth backed by `express-session` with Redis session storage. The session cookie name defaults to `sessionId` and can be overridden by `SESSION_COOKIE_NAME`.
  how_to_obtain: The server sets the `sessionId` cookie after a successful login flow.
  location: cookie
  name: session cookie
  type: other
- evidence: An enabled `ldap-single` provider renders a working `Username`, `Password`, and `Login` form. It submits to `POST /api/auth/ldap-single`.
  how_to_obtain: POST `username`, `password`, and optional `inviteCode`/`returnPath` to `/api/auth/ldap-single`.
  location: body
  name: ldap‑single
  type: other
slug: alloy-cx-authentication
source_filename: alloy-cx-authentication.yml
source_heading: Authentication Profile
source_url: https://alloy.cx/docs/reference/tech-docs/auth-and-session
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://alloy.cx/docs/reference/tech-docs/auth-and-session\nsources:\n- https://alloy.cx/docs/reference/tech-docs/auth-and-session\n- https://alloy.cx/docs/getting-started/what-alloy-is\n- https://alloy.cx/docs/getting-started/meet-ally\n- https://alloy.cx/docs/getting-started/add-your-first-ai-teammate\ndescription: Alloy uses cookie‑based session authentication and optional LDAP form credentials.\nschemes:\n- type: other\n  name: session cookie\n  evidence: Sessions use cookie‑based auth backed by `express-session` with Redis session storage. The session cookie name defaults to `sessionId`\n    and can be overridden by `SESSION_COOKIE_NAME`.\n  location: cookie\n  how_to_obtain: The server sets the `sessionId` cookie after a successful login flow.\n- type: other\n  name: ldap‑single\n  evidence: An enabled `ldap-single` provider renders a working `Username`, `Password`, and `Login`\
  \ form. It submits to `POST /api/auth/ldap-single`.\n  location: body\n  how_to_obtain: POST `username`, `password`, and optional `inviteCode`/`returnPath` to `/api/auth/ldap-single`.\nnote: No OAuth2 flows are described on the referenced pages.\ndocs: https://alloy.cx/docs/reference/tech-docs/auth-and-session\n"
source_yaml_url: https://artifacts.apis.io/alloy-cx/authentication/alloy-cx-authentication.yml
summary_line: 2 schemes
tags:
- Real Estate
- Artificial Intelligence
- Investment
- Automation
- CRM
---
