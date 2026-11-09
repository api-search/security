---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dunsocial-com-openapi-generated.yml
  format: yaml
  label: DunSocial API
  slug: dunsocial-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunsocial-com/openapi/_ae-authored/dunsocial-com-openapi-generated.yml
auth_types: []
description: Authentication - DunSocial Docs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dunsocial Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DunSocial declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DunSocial
provider_slug: dunsocial-com
scheme_count: 1
schemes:
- evidence: 'Authenticate DunSocial API requests with a bearer token: a session token from sign‑in for apps, or a personal access token for CI, scripts, and automation.'
  header: Authorization
  how_to_obtain: Obtain a session token by signing in with email and password via POST https://api.dunsocial.com/api/auth/sign-in/email, or create a personal access token (PAT) via POST https://api.dunsocial.com/api/cli/tokens while signed in.
  location: header
  name: Bearer token
  type: http-bearer
slug: dunsocial-com-authentication
source_filename: dunsocial-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.dunsocial.com/docs/api/getting-started/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.dunsocial.com/docs/api/getting-started/authentication\nsources:\n- https://www.dunsocial.com/docs/api/getting-started/authentication\n- https://www.dunsocial.com/blog/use-separate-dunsocial-cli-tokens-for-each-agency-client.md\n- https://www.dunsocial.com/hub/social-media-automation-for-developers/what-is-a-personal-access-token-and-how-does-it-secure-api-access.md\n- https://www.dunsocial.com/faq/getting-started.md\ndescription: Authentication - DunSocial Docs\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authenticate DunSocial API requests with a bearer token: a session token from sign‑in for apps, or a personal access token for CI,\n    scripts, and automation.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a session token by signing in with email and password via POST https://api.dunsocial.com/api/auth/sign-in/email, or\
  \ create\n    a personal access token (PAT) via POST https://api.dunsocial.com/api/cli/tokens while signed in.\nnote: Workspace identifier is sent in a separate header X-Workspace-Id, but authentication itself is via the Bearer token.\ndocs: https://www.dunsocial.com/docs/api/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/dunsocial-com/authentication/dunsocial-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Social Media
- Scheduler
- Marketing
- Automation
---
