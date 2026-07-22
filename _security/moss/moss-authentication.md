---
api_key_in:
- header
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moss Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moss secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moss
provider_slug: moss
scheme_count: 2
schemes:
- description: 'Project access key sent in the x-project-key header. Requests to the Moss Control Plane API also require an x-service-version: v1 header and a projectId field in the JSON body. Invalid credentials return 403 Forbidden with a JSON error payload.'
  in: header
  name: project-key
  parameter: x-project-key
  sources:
  - https://docs.moss.dev/docs/api-reference/v1/getting-started/authentication.md
  type: apiKey
- description: Project identifier issued by Moss Control, supplied in the JSON request body alongside the x-project-key header.
  in: body
  name: project-id
  parameter: projectId
  type: apiKey
slug: moss-authentication
source_filename: moss-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.moss.dev/docs/api-reference/v1/getting-started/authentication.md\ndocs: https://docs.moss.dev/docs/integrate/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - body\n  oauth2_flows: []\nschemes:\n- name: project-key\n  type: apiKey\n  in: header\n  parameter: x-project-key\n  description: >-\n    Project access key sent in the x-project-key header. Requests to the Moss\n    Control Plane API also require an x-service-version: v1 header and a\n    projectId field in the JSON body. Invalid credentials return 403 Forbidden\n    with a JSON error payload.\n  sources:\n  - https://docs.moss.dev/docs/api-reference/v1/getting-started/authentication.md\n- name: project-id\n  type: apiKey\n  in: body\n  parameter: projectId\n  description: Project identifier issued by Moss Control, supplied in the JSON request body alongside the x-project-key header.\nsdk_env:\n- MOSS_PROJECT_ID\n- MOSS_PROJECT_KEY\n\
  notes: >-\n  SDKs (JS/Python) construct a MossClient with (project_id, project_key) or read\n  MOSS_PROJECT_ID / MOSS_PROJECT_KEY from the environment. Browser/frontend\n  clients use a Custom Authenticator to mint short-lived tokens server-side so\n  the project key never ships to the browser\n  (https://docs.moss.dev/docs/reference/js/custom-authenticator). No OAuth2/OIDC\n  scope surface is documented; auth is project-key based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moss/refs/heads/main/authentication/moss-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Semantic Search
- Vector Search
- Retrieval
- AI Agents
- Voice AI
- Embeddings
- RAG
- Developer Tools
- On-Device AI
---
