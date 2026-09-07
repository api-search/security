---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cognizant-technology-neuro-san-agent-service.json
  format: json
  label: Cognizant Neuro SAN Agent Service
  slug: cognizant-neuro-san-agent-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognizant-technology/refs/heads/main/openapi/cognizant-technology-neuro-san-agent-service.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Cognizant Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognizant Technology Solutions declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cognizant Technology Solutions
provider_slug: cognizant-technology
scheme_count: 0
schemes: []
slug: cognizant-technology-authentication
source_filename: cognizant-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://github.com/cognizant-ai-lab/neuro-san/blob/main/README.md +\n  https://github.com/cognizant-ai-lab/neuro-san/blob/main/docs/mcp_service.md +\n  openapi/cognizant-technology-neuro-san-agent-service.json\ndocs: https://github.com/cognizant-ai-lab/neuro-san#readme\nnote: >-\n  HEADLINE FINDING, recorded plainly: the published NeuroSan OpenAPI declares NO\n  securitySchemes and applies no security to any of its four operations, and the MCP service\n  documentation shows unauthenticated curl calls carrying only Content-Type and\n  MCP-Protocol-Version headers. The contract as published describes an OPEN surface.\n  That is not the whole picture, and the difference matters. Neuro SAN is self-hosted\n  software, so the deployment boundary — not the contract — is where an operator is expected\n  to put authentication. The provider does document two real, first-party authorization\n  mechanisms in prose, neither of which\
  \ appears in the machine-readable contract. Both are\n  listed below as documented-but-unspecified so an agent author knows they exist and knows\n  they cannot be discovered from the spec.\nschemes: []\nschemes_note: >-\n  Empty by observation, not by omission. components.securitySchemes is absent from the\n  published OpenAPI and no top-level or operation-level `security` block appears.\ndocumented_but_not_in_contract:\n- name: per-user authorization for agent networks\n  kind: external-authorization\n  source: neuro-san README feature list\n  detail: >-\n    \"per-user authorization for Agent Networks - optional implementations include: OpenFGA\".\n    An optional, pluggable authorization layer the operator wires in. Not described in the\n    OpenAPI, so an agent cannot discover whether a given deployment enforces it.\n  enforced_by: operator\n- name: Bring-Your-Own-Key (BYOK)\n  kind: client-supplied-credential\n  source: neuro-san README feature list\n  detail: >-\n    \"Secure Bring-Your-Own-Key\
  \ (BYOK) support for client-provided API keys so your deployments\n    do not have to shoulder everyone else's token costs.\" These are LLM-PROVIDER keys\n    (OpenAI and similar) that the caller supplies, not credentials for the neuro-san API\n    itself — an important distinction. They travel over the private sly_data channel rather\n    than an Authorization header, which is why they never surface as a securityScheme.\n  enforced_by: client\n  transport: sly_data (private channel, deliberately excluded from the LLM chat stream)\n  evidence: >-\n    neuro_san/registries/music_nerd_pro_sly_api_key.hocon and the paired test fixtures\n    (tests/fixtures/music_nerd_pro_sly_api_key/{no_user_api_key,with_user_api_key}.hocon)\n    are the provider's own worked examples of an agent network that takes a user-supplied API\n    key through sly_data.\nserver_side_credentials:\n  note: >-\n    The credentials an OPERATOR must set to run a server are environment variables for\n    downstream LLM\
  \ providers, not credentials for this API.\n  environment_variables:\n  - OPENAI_API_KEY\n  - AGENT_TOOL_PATH\n  - AGENT_MANIFEST_FILE\n  - PYTHONPATH\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key_header: null\ntransport_security:\n  https_enforced: false\n  detail: >-\n    The provider's own documented examples use http://localhost:8080. TLS termination is the\n    operator's responsibility; nothing in the contract or docs requires it.\nagent_guidance: >-\n  An agent integrating with a neuro-san deployment cannot learn the auth model from the\n  contract and must ask the operator. Assume no authentication is declared, expect the\n  deployment to sit behind whatever the operator put in front of it, and expect any\n  LLM-provider key to be passed through sly_data rather than a header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognizant-technology/refs/heads/main/authentication/cognizant-technology-authentication.yml
summary_line: 0 schemes
tags:
- AI Platform
- Consulting
- Digital Transformation
- IT Services
- Multi-Agent
- Neuro AI
- Fortune 500
---
