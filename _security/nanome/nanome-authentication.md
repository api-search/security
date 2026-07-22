---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nanome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nanome secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nanome
provider_slug: nanome
scheme_count: 1
schemes:
- description: 'Long-lived Nanome API key passed as an HTTP `Authorization: Bearer {token}` header. Keys are created from the mara.nanome.ai account settings (System tab -> API Keys -> Create) and stored client-side (the official plugin saves to ~/.nanome/config.json). All Workspaces API (workspaces.nanome.ai) and account API (api.nanome.ai) calls use the same bearer token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - skills/nanome-auth.md
  - skills/nanome-workspace.md
  type: http
slug: nanome-authentication
source_filename: nanome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/nanome-ai/claude-code-nanome-plugin (nanome-plugin/skills/nanome-auth/SKILL.md)\ndocs: https://mara.nanome.ai/settings\nsummary:\n  types: [http]\n  http_scheme: bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Long-lived Nanome API key passed as an HTTP `Authorization: Bearer {token}` header.\n      Keys are created from the mara.nanome.ai account settings (System tab -> API Keys -> Create)\n      and stored client-side (the official plugin saves to ~/.nanome/config.json). All Workspaces\n      API (workspaces.nanome.ai) and account API (api.nanome.ai) calls use the same bearer token.\n    sources: [skills/nanome-auth.md, skills/nanome-workspace.md]\nnotes:\n  - Session validity can be checked with GET https://api.nanome.ai/user/session (200 = valid token).\n  - The workspace API base URL is discoverable at https://mara.nanome.ai/info\
  \ (workspace_api_url field).\n  - A missing/expired key surfaces as HTTP 401/403 on API calls; re-create the key in account settings.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanome/refs/heads/main/authentication/nanome-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Drug Discovery
- Molecular Visualization
- Life Sciences
- Cheminformatics
- Structural Biology
- Virtual Reality
- Collaboration
- Artificial Intelligence
---
