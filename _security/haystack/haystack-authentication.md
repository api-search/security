---
api_key_in: []
api_specs:
- filename: haystack-config-api-openapi.yml
  format: yaml
  label: Haystack Config API
  slug: haystack-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack/refs/heads/main/openapi/haystack-config-api-openapi.yml
- filename: haystack-dashboard-api-openapi.yml
  format: yaml
  label: Haystack Dashboard API
  slug: haystack-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack/refs/heads/main/openapi/haystack-dashboard-api-openapi.yml
- filename: haystack-openai-api-openapi.yml
  format: yaml
  label: Haystack Openai API
  slug: haystack-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack/refs/heads/main/openapi/haystack-openai-api-openapi.yml
- filename: haystack-status-api-openapi.yml
  format: yaml
  label: Haystack Status API
  slug: haystack-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack/refs/heads/main/openapi/haystack-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Haystack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Haystack declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Haystack
provider_slug: haystack
scheme_count: 0
schemes: []
slug: haystack-authentication
source_filename: haystack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: 'derive-authentication.py over openapi/haystack-hayhooks-openapi.json returned\n  zero schemes; upgraded by reading\n  https://deepset-ai.github.io/hayhooks/reference/api-reference/#authentication, which\n  states the position explicitly.'\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\nschemes: []\nfinding: none\ndetail: 'Hayhooks does not include built-in authentication. This is a stated design\n  position, not an omission from the spec: the API reference says \"Currently, Hayhooks does\n  not include built-in authentication\" and directs operators to reverse-proxy\n  authentication, network-level security, or custom middleware. All 19 operations in the\n  generated OpenAPI - including POST /deploy_files and POST /deploy-yaml, which execute\n  operator-supplied Python - are unauthenticated by default. The Haystack SECURITY.md makes\n  the same trust-boundary argument: Haystack is \"a framework intended to run\
  \ inside a\n  trusted execution environment\".'\ndocs: https://deepset-ai.github.io/hayhooks/reference/api-reference/\nmcp_auth: none\nmcp_note: 'The Hayhooks MCP server inherits this: no auth, no OAuth metadata, no\n  /.well-known/oauth-protected-resource. It binds to localhost by default.'\nsecurity_guidance:\n- https://github.com/deepset-ai/haystack/blob/main/SECURITY.md\n- https://deepset-ai.github.io/hayhooks/deployment/deployment_guidelines/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haystack/refs/heads/main/authentication/haystack-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- Agents
- RAG
- Retrieval
- Orchestration
- Open Source
- Model Context Protocol
- Search
---
