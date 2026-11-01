---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes supported by Strands Agents Box egress gateway as described in the documentation.
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Strandsagents Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strands Agents declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Strands Agents
provider_slug: strandsagents
scheme_count: 6
schemes:
- evidence: 'When a permitted request to `api.github.com` carries the placeholder where the binding puts the credential, by default `Authorization: Bearer`, the gateway replaces it with the real token.'
  header: Authorization
  location: header
  name: Bearer token (default)
  type: http-bearer
- evidence: '`secret.header = "x-api-key"` → `x-api-key: <secret>`'
  header: x-api-key
  location: header
  name: Custom header
  type: apiKey
- evidence: '`secret.prefix = "token "` → `Authorization: token <secret>`'
  header: Authorization
  location: header
  name: Custom prefix
  type: http-bearer
- evidence: '`secret.placement = "basic_auth"` → `Authorization: Basic …`, with the secret as the `user:password` pair'
  header: Authorization
  location: header
  name: HTTP Basic
  type: http-basic
- evidence: '`secret.placement = "query_param"`, `secret.param = "key"` → `?key=<secret>`'
  location: query
  name: Query parameter
  type: apiKey
- evidence: '`secret.ref = "aws://…"` or `"credsd://…"` → A SigV4 signature'
  location: header
  name: AWS SigV4
  type: other
slug: strandsagents-authentication
source_filename: strandsagents-authentication.yml
source_heading: Authentication Profile
source_url: https://strandsagents.com/docs/user-guide/box/guides/network-and-credentials/index.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://strandsagents.com/docs/user-guide/box/guides/network-and-credentials/index.md\nsources:\n- https://strandsagents.com/docs/user-guide/box/guides/network-and-credentials/index.md\n- https://strandsagents.com/blog/introducing-strands-harness/index.md\n- https://strandsagents.com/docs/user-guide/box/guides/network-and-credentials/\n- https://strandsagents.com/docs/user-guide/harness/quickstart/index.md\ndescription: Authentication schemes supported by Strands Agents Box egress gateway as described in the documentation.\nschemes:\n- type: http-bearer\n  name: Bearer token (default)\n  evidence: 'When a permitted request to `api.github.com` carries the placeholder where the binding puts the credential, by default `Authorization:\n    Bearer`, the gateway replaces it with the real token.'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: Custom header\n  evidence:\
  \ '`secret.header = \"x-api-key\"` → `x-api-key: <secret>`'\n  location: header\n  header: x-api-key\n- type: http-bearer\n  name: Custom prefix\n  evidence: '`secret.prefix = \"token \"` → `Authorization: token <secret>`'\n  location: header\n  header: Authorization\n- type: http-basic\n  name: HTTP Basic\n  evidence: '`secret.placement = \"basic_auth\"` → `Authorization: Basic …`, with the secret as the `user:password` pair'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: Query parameter\n  evidence: '`secret.placement = \"query_param\"`, `secret.param = \"key\"` → `?key=<secret>`'\n  location: query\n- type: other\n  name: AWS SigV4\n  evidence: '`secret.ref = \"aws://…\"` or `\"credsd://…\"` → A SigV4 signature'\n  location: header\ndocs: https://strandsagents.com/docs/user-guide/box/guides/network-and-credentials/index.md\n"
source_yaml_url: https://artifacts.apis.io/strandsagents/authentication/strandsagents-authentication.yml
summary_line: 6 schemes
tags:
- Company
- AI
- OpenSource
- Toolkit
- Agents
---
