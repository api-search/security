---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fiddler Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fiddler Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fiddler Labs
provider_slug: fiddler-labs
scheme_count: 1
schemes:
- description: All Fiddler REST API and MCP requests authenticate with a Bearer access key (token prefix `fid_`) passed in the Authorization header. Keys are created and managed under Settings > Credentials (Users & Access Keys). Access is governed by role-based access control (RBAC). The Python client accepts the same token via its connection setup.
  header: Authorization
  header_format: 'Authorization: Bearer [example key]'
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs.fiddler.ai/api/rest-api/rest-api
  token_prefix: fid_
  type: http
slug: fiddler-labs-authentication
source_filename: fiddler-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fiddler.ai/api/rest-api/rest-api\ndocs: https://docs.fiddler.ai/developers/python-client-guides/installation-and-setup\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  token_prefix: fid_\n  location: header\n  header: Authorization\n  header_format: 'Authorization: Bearer [example key]'\n  description: >-\n    All Fiddler REST API and MCP requests authenticate with a Bearer access key\n    (token prefix `fid_`) passed in the Authorization header. Keys are created\n    and managed under Settings > Credentials (Users & Access Keys). Access is\n    governed by role-based access control (RBAC). The Python client accepts the\n    same token via its connection setup.\n  sources:\n  - docs.fiddler.ai/api/rest-api/rest-api\nrbac: true\nnotes: >-\n  No OAuth2 or OpenID Connect flows are documented; authentication is a\n  long-lived\
  \ Bearer access key. There is no OpenAPI spec published publicly, so\n  this profile is derived from the REST API and client documentation rather than\n  a machine-readable securityScheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiddler-labs/refs/heads/main/authentication/fiddler-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Observability
- ML Monitoring
- LLM Observability
- Agentic AI
- AI Security
- AI Governance
- Model Monitoring
- Explainability
- Guardrails
---
