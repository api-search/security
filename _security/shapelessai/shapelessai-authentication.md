---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shapelessai-ads-api-openapi.yml
  format: yaml
  label: ShapelessAI Ads API
  slug: shapelessai-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-ads-api-openapi.yml
- filename: shapelessai-brain-api-openapi.yml
  format: yaml
  label: ShapelessAI Brain API
  slug: shapelessai-brain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-brain-api-openapi.yml
- filename: shapelessai-capabilities-api-openapi.yml
  format: yaml
  label: ShapelessAI Capabilities API
  slug: shapelessai-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-capabilities-api-openapi.yml
- filename: shapelessai-connections-api-openapi.yml
  format: yaml
  label: ShapelessAI Connections API
  slug: shapelessai-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-connections-api-openapi.yml
- filename: shapelessai-groups-api-openapi.yml
  format: yaml
  label: ShapelessAI Groups API
  slug: shapelessai-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-groups-api-openapi.yml
- filename: shapelessai-jobs-api-openapi.yml
  format: yaml
  label: ShapelessAI Jobs API
  slug: shapelessai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-jobs-api-openapi.yml
- filename: shapelessai-manager-api-openapi.yml
  format: yaml
  label: ShapelessAI Manager API
  slug: shapelessai-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-manager-api-openapi.yml
- filename: shapelessai-me-api-openapi.yml
  format: yaml
  label: ShapelessAI Me API
  slug: shapelessai-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-me-api-openapi.yml
- filename: shapelessai-metrics-api-openapi.yml
  format: yaml
  label: ShapelessAI Metrics API
  slug: shapelessai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-metrics-api-openapi.yml
- filename: shapelessai-posts-api-openapi.yml
  format: yaml
  label: ShapelessAI Posts API
  slug: shapelessai-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-posts-api-openapi.yml
- filename: shapelessai-profile-api-openapi.yml
  format: yaml
  label: ShapelessAI Profile API
  slug: shapelessai-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-profile-api-openapi.yml
- filename: shapelessai-shapelessai-api-api-openapi.yml
  format: yaml
  label: ShapelessAI ShapelessAI API
  slug: shapelessai-shapelessai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-shapelessai-api-api-openapi.yml
- filename: shapelessai-strategies-api-openapi.yml
  format: yaml
  label: ShapelessAI Strategies API
  slug: shapelessai-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-strategies-api-openapi.yml
- filename: shapelessai-studio-api-openapi.yml
  format: yaml
  label: ShapelessAI Studio API
  slug: shapelessai-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-studio-api-openapi.yml
- filename: shapelessai-tools-api-openapi.yml
  format: yaml
  label: ShapelessAI Tools API
  slug: shapelessai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-tools-api-openapi.yml
- filename: shapelessai-videos-api-openapi.yml
  format: yaml
  label: ShapelessAI Videos API
  slug: shapelessai-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-videos-api-openapi.yml
- filename: shapelessai-wiki-api-openapi.yml
  format: yaml
  label: ShapelessAI Wiki API
  slug: shapelessai-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-wiki-api-openapi.yml
- filename: shapelessai-workspace-api-openapi.yml
  format: yaml
  label: ShapelessAI Workspace API
  slug: shapelessai-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/shapelessai-workspace-api-openapi.yml
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
- Artificial Intelligence
- Social Media
- Automation
- Software-as-a-Service
---
