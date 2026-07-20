---
api_key_in:
- header
- env
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Judgment Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Judgment Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Judgment Labs
provider_slug: judgment-labs
scheme_count: 1
schemes:
- applies_to:
  - https://api.judgmentlabs.ai
  - https://mcp.judgmentlabs.ai
  credentials:
  - env: JUDGMENT_API_KEY
    role: organization API key (bearer token)
  - env: JUDGMENT_ORG_ID
    role: organization identifier
  evidence:
  - mcp.judgmentlabs.ai returns HTTP 401 without credentials
  - Official Judgment Agent Skill instructs setting JUDGMENT_API_KEY and JUDGMENT_ORG_ID
  in: header
  name: JudgmentApiKey
  scheme: bearer
  type: apiKey
slug: judgment-labs-authentication
source_filename: judgment-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.judgmentlabs.ai/documentation\ndocs: https://docs.judgmentlabs.ai/documentation\nsummary:\n  types: [apiKey]\n  api_key_in: [header, env]\n  oauth2_flows: []\n  note: >-\n    Judgment authenticates with an organization-scoped API key plus an organization ID. The\n    key is presented as a bearer token on requests to the platform API and MCP server; both\n    values are typically supplied to the SDK/CLI via environment variables. No OAuth2 / OIDC\n    flow or granular scope surface is published (there is no public OpenAPI to derive from).\nschemes:\n- name: JudgmentApiKey\n  type: apiKey\n  in: header\n  scheme: bearer\n  credentials:\n  - env: JUDGMENT_API_KEY\n    role: organization API key (bearer token)\n  - env: JUDGMENT_ORG_ID\n    role: organization identifier\n  applies_to:\n  - https://api.judgmentlabs.ai\n  - https://mcp.judgmentlabs.ai\n  evidence:\n  - 'mcp.judgmentlabs.ai returns HTTP 401 without credentials'\n\
  \  - 'Official Judgment Agent Skill instructs setting JUDGMENT_API_KEY and JUDGMENT_ORG_ID'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judgment-labs/refs/heads/main/authentication/judgment-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Agents
- Artificial Intelligence
- Agent Evaluation
- Observability
- Tracing
- Monitoring
- LLM
- Developer Tools
- MCP
---
