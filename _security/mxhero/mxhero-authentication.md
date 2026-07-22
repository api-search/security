---
api_key_in: []
auth_types:
- token
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mxhero Authentication
name_suffix: Authentication
oauth_flows: []
overview: mxHero secures its APIs with token and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: mxHero
provider_slug: mxhero
scheme_count: 2
schemes:
- location: passed as the required -t argument to the stdio binary / bearer token to the HTTP endpoint
  name: mcp-access-token
  note: mxHERO Vector Search credentials (personal access token). Demo tokens available.
  scheme: bearer
  sources:
  - https://github.com/mxaiorg/mxmcp
  token_endpoint: https://lab4-mcp.mxhero.com/tokens
  type: token
  used_by: Mail2Cloud Advanced MCP server (email_search)
- name: mxhero-v3-api-key
  note: mxHERO documentation references an mxHERO V3 API Key for managing datasets and S/MIME through the V3 API. Endpoint reference is not publicly published.
  sources:
  - https://mxhero.helpjuice.com/general-information
  type: apiKey
  used_by: mxHERO V3 REST API (dataset and S/MIME management)
slug: mxhero-authentication
source_filename: mxhero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/mxaiorg/mxmcp\ndocs: https://mxhero.helpjuice.com/en_US/mxhero-ai\nnote: >-\n  No OpenAPI is published, so this profile is captured from mxHERO's public\n  documentation and the official MCP server repositories rather than derived\n  from a spec.\nsummary:\n  types:\n  - token\n  - apiKey\nschemes:\n- name: mcp-access-token\n  type: token\n  scheme: bearer\n  used_by: Mail2Cloud Advanced MCP server (email_search)\n  location: passed as the required -t argument to the stdio binary / bearer token to the HTTP endpoint\n  token_endpoint: https://lab4-mcp.mxhero.com/tokens\n  note: mxHERO Vector Search credentials (personal access token). Demo tokens available.\n  sources:\n  - https://github.com/mxaiorg/mxmcp\n- name: mxhero-v3-api-key\n  type: apiKey\n  used_by: mxHERO V3 REST API (dataset and S/MIME management)\n  note: >-\n    mxHERO documentation references an mxHERO V3 API Key for managing datasets\n   \
  \ and S/MIME through the V3 API. Endpoint reference is not publicly published.\n  sources:\n  - https://mxhero.helpjuice.com/general-information\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mxhero/refs/heads/main/authentication/mxhero-authentication.yml
summary_line: token/apiKey · 2 schemes
tags:
- Company
- Email
- Cloud Storage
- Content Management
- Email to Cloud
- Artificial Intelligence
- MCP
- Email Search
- Compliance
- Collaboration
---
