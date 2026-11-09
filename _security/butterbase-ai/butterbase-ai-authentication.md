---
anonymous_access: false
api_key_in: []
api_specs:
- filename: butterbase-ai-openapi-generated.yml
  format: yaml
  label: Butterbase API
  slug: butterbase-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/butterbase-ai/openapi/_ae-authored/butterbase-ai-openapi-generated.yml
auth_types: []
description: Butterbase authentication uses JWT bearer tokens for API calls and OAuth2 for social sign‑in.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Butterbase Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Butterbase declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Butterbase
provider_slug: butterbase-ai
scheme_count: 2
schemes:
- evidence: The access token is what your frontend sends with API requests.
  header: Authorization
  how_to_obtain: Obtain via POST /auth/{app_id}/login, POST /auth/{app_id}/magic-link/verify, or other auth endpoints which return an "access_token".
  location: header
  name: JWT access token
  type: http-bearer
- authorize_url: /auth/{app_id}/oauth/{provider}
  evidence: Direct the user’s browser to /auth/{app_id}/oauth/{provider}?redirect_to=https://yourapp.com/callback
  header: Authorization
  how_to_obtain: Configure a provider via the OAuth configuration API or MCP tool, then start the flow by redirecting the user to the authorize URL; the provider redirects back to the callback URL with an authorization code which is exchanged for tokens.
  location: header
  name: Social sign‑in (OAuth)
  scopes:
  - 'google: openid, email, profile'
  - 'github: user:email'
  - 'discord: identify, email'
  - 'facebook: email, public_profile'
  - 'linkedin: openid, profile, email'
  - 'microsoft: openid, email, profile, User.Read'
  - 'apple: name, email'
  - 'x: tweet.read, users.read'
  token_url: /auth/{app_id}/oauth/{provider}/callback
  type: oauth2
slug: butterbase-ai-authentication
source_filename: butterbase-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.butterbase.ai/core-concepts/authentication/
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.butterbase.ai/core-concepts/authentication/\nsources:\n- https://docs.butterbase.ai/core-concepts/authentication/\n- https://docs.butterbase.ai/api-reference/auth-api/\n- https://docs.butterbase.ai/getting-started/agents-quickstart/\n- https://docs.butterbase.ai/getting-started/before-you-start/\ndescription: Butterbase authentication uses JWT bearer tokens for API calls and OAuth2 for social sign‑in.\nschemes:\n- type: http-bearer\n  name: JWT access token\n  evidence: The access token is what your frontend sends with API requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via POST /auth/{app_id}/login, POST /auth/{app_id}/magic-link/verify, or other auth endpoints which return an \"access_token\".\n- type: oauth2\n  name: Social sign‑in (OAuth)\n  evidence: Direct the user’s browser to /auth/{app_id}/oauth/{provider}?redirect_to=https://yourapp.com/callback\n\
  \  location: header\n  header: Authorization\n  token_url: /auth/{app_id}/oauth/{provider}/callback\n  authorize_url: /auth/{app_id}/oauth/{provider}\n  scopes:\n  - 'google: openid, email, profile'\n  - 'github: user:email'\n  - 'discord: identify, email'\n  - 'facebook: email, public_profile'\n  - 'linkedin: openid, profile, email'\n  - 'microsoft: openid, email, profile, User.Read'\n  - 'apple: name, email'\n  - 'x: tweet.read, users.read'\n  how_to_obtain: Configure a provider via the OAuth configuration API or MCP tool, then start the flow by redirecting the user to the authorize\n    URL; the provider redirects back to the callback URL with an authorization code which is exchanged for tokens.\ndocs: https://docs.butterbase.ai/core-concepts/authentication/\n"
source_yaml_url: https://artifacts.apis.io/butterbase-ai/authentication/butterbase-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Backend
- Business
- Agent-Native
- Platform
---
