---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apiway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apiway declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Apiway
provider_slug: apiway
scheme_count: 2
schemes:
- authorize_url: https://apiway.ai/login?provider=google
  evidence: Apiway accepts Google OAuth and email + password (with one-time-code email verification on registration).
  flows:
  - authorization_code
  how_to_obtain: Select Google OAuth on the login page and follow the provider's consent flow.
  name: Google OAuth
  type: oauth2
- evidence: Auth uses Supabase Auth (cookies + JWT).
  how_to_obtain: After successful login (via Google OAuth or email/password), a JWT is set in a cookie and can be used as a Bearer token.
  name: Supabase JWT
  type: http-bearer
slug: apiway-authentication
source_filename: apiway-authentication.yml
source_heading: Authentication Profile
source_url: https://apiway.ai/docs/getting-started/sign-up
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apiway.ai/docs/getting-started/sign-up\nsources:\n- https://apiway.ai/docs/getting-started/sign-up\n- https://apiway.ai/presentation-templates/company/marketing-agency\n- https://apiway.ai/docs/getting-started/what-is-apiway\n- https://apiway.ai/docs/getting-started/what-is-apiway.md\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: Apiway accepts Google OAuth and email + password (with one-time-code email verification on registration).\n  flows:\n  - authorization_code\n  authorize_url: https://apiway.ai/login?provider=google\n  how_to_obtain: Select Google OAuth on the login page and follow the provider's consent flow.\n- type: http-bearer\n  name: Supabase JWT\n  evidence: Auth uses Supabase Auth (cookies + JWT).\n  how_to_obtain: After successful login (via Google OAuth or email/password), a JWT is set in a cookie and can be used as a Bearer token.\ndocs:\
  \ https://apiway.ai/docs/getting-started/sign-up\n"
source_yaml_url: https://artifacts.apis.io/apiway/authentication/apiway-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Workspace
- Automation
- No-code
---
