---
anonymous_access: false
api_key_in: []
auth_types: []
description: LearnOS authentication methods as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LearnOS Authentication
name_suffix: Authentication
oauth_flows: []
overview: LearnOS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LearnOS
provider_slug: learnosapp-com
scheme_count: 2
schemes:
- evidence: This opens a browser, runs OAuth 2.1 + PKCE against Supabase Auth, and stores access + refresh tokens in ~/.config/learnos/credentials.json (mode 0600 ).
  how_to_obtain: Run `learnos login` which opens a browser for OAuth 2.1 with PKCE.
  name: Supabase Auth (OAuth 2.1 + PKCE)
  type: oauth2
- evidence: 'Fallback: personal access token export LEARNOS_TOKEN = los_... Issue a token from Settings → Personal access tokens .'
  header: LEARNOS_TOKEN
  how_to_obtain: Create a token in Settings → Personal access tokens.
  location: environment variable
  name: Personal access token
  type: apiKey
slug: learnosapp-com-authentication
source_filename: learnosapp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://learnosapp.com/docs/cli/auth
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://learnosapp.com/docs/cli/auth\nsources:\n- https://learnosapp.com/docs/cli/auth\n- https://learnosapp.com/docs/getting-started\ndescription: LearnOS authentication methods as documented\nschemes:\n- type: oauth2\n  name: Supabase Auth (OAuth 2.1 + PKCE)\n  evidence: This opens a browser, runs OAuth 2.1 + PKCE against Supabase Auth, and stores access + refresh tokens in ~/.config/learnos/credentials.json\n    (mode 0600 ).\n  how_to_obtain: Run `learnos login` which opens a browser for OAuth 2.1 with PKCE.\n- type: apiKey\n  name: Personal access token\n  evidence: 'Fallback: personal access token export LEARNOS_TOKEN = los_... Issue a token from Settings → Personal access tokens .'\n  location: environment variable\n  header: LEARNOS_TOKEN\n  how_to_obtain: Create a token in Settings → Personal access tokens.\ndocs: https://learnosapp.com/docs/cli/auth\n"
source_yaml_url: https://artifacts.apis.io/learnosapp-com/authentication/learnosapp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Education
- Artificial Intelligence
- Learning
- Platform
---
