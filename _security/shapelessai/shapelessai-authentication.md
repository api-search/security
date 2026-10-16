---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shapelessai-openapi-generated.yml
  format: yaml
  label: ShapelessAI API
  slug: shapelessai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/_ae-authored/shapelessai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Shapelessai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShapelessAI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ShapelessAI
provider_slug: shapelessai
scheme_count: 2
schemes:
- evidence: 'A key is `slk_` followed by 40 base64url characters. Send it on every request:


    ```bash

    curl -H "Authorization: Bearer slk_..." https://shapelessai.com/api/me

    ```'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'It is OAuth 2.1 with dynamic client registration and PKCE, so a host registers itself:

    - Protected-resource metadata: `https://shapelessai.com/.well-known/oauth-protected-resource/mcp`

    - Scopes: `read`, `write`, `publish`, `offline_access`'
  name: OAuth 2.1
  scopes:
  - read
  - write
  - publish
  - offline_access
  type: oauth2
slug: shapelessai-authentication
source_filename: shapelessai-authentication.yml
source_heading: Authentication Profile
source_url: https://shapelessai.com/docs/auth
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://shapelessai.com/docs/auth\nsources:\n- https://shapelessai.com/docs/auth\n- https://shapelessai.com/docs/api\n- https://shapelessai.com/docs/auth.md\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'A key is `slk_` followed by 40 base64url characters. Send it on every request:\n\n\n    ```bash\n\n    curl -H \"Authorization: Bearer slk_...\" https://shapelessai.com/api/me\n\n    ```'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'It is OAuth 2.1 with dynamic client registration and PKCE, so a host registers itself:\n\n    - Protected-resource metadata: `https://shapelessai.com/.well-known/oauth-protected-resource/mcp`\n\n    - Scopes: `read`, `write`, `publish`, `offline_access`'\n  scopes:\n  - read\n  - write\n  - publish\n  - offline_access\ndocs: https://shapelessai.com/docs/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/authentication/shapelessai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Social Media
- Automation
- SaaS
---
