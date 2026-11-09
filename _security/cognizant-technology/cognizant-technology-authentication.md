---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cognizant-technology-agentservice-api-openapi.yml
  format: yaml
  label: Cognizant Technology Solutions Agent Service API
  slug: cognizant-technology-agentservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cognizant-technology/openapi/cognizant-technology-agentservice-api-openapi.yml
- filename: cognizant-technology-conciergeservice-api-openapi.yml
  format: yaml
  label: Cognizant Technology Solutions Concierge Service API
  slug: cognizant-technology-conciergeservice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cognizant-technology/openapi/cognizant-technology-conciergeservice-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
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
source_yaml: "generated: '2026-11-04'\nmethod: none\nsource: https://github.com/cognizant-ai-lab/neuro-san/blob/main/README.md + https://github.com/cognizant-ai-lab/neuro-san/blob/main/docs/mcp_service.md\n  + openapi/cognizant-technology-neuro-san-agent-service.json\ndocs: https://github.com/cognizant-ai-lab/neuro-san#readme\nnote: 'HEADLINE FINDING, recorded plainly: the published NeuroSan OpenAPI declares NO securitySchemes and applies\n  no security to any of its four operations, and the MCP service documentation shows unauthenticated curl calls\n  carrying only Content-Type and MCP-Protocol-Version headers. The contract as published describes an OPEN surface.\n  That is not the whole picture, and the difference matters. Neuro SAN is self-hosted software, so the deployment\n  boundary — not the contract — is where an operator is expected to put authentication. The provider does document\n  two real, first-party authorization mechanisms in prose, neither of which appears in the machine-readable\
  \ contract.\n  Both are listed below as documented-but-unspecified so an agent author knows they exist and knows they cannot\n  be discovered from the spec.'\nschemes: []\nschemes_note: Empty by observation, not by omission. components.securitySchemes is absent from the published OpenAPI\n  and no top-level or operation-level `security` block appears.\ndocumented_but_not_in_contract:\n- name: per-user authorization for agent networks\n  kind: external-authorization\n  source: neuro-san README feature list\n  detail: '\"per-user authorization for Agent Networks - optional implementations include: OpenFGA\". An optional,\n    pluggable authorization layer the operator wires in. Not described in the OpenAPI, so an agent cannot discover\n    whether a given deployment enforces it.'\n  enforced_by: operator\n- name: Bring-Your-Own-Key (BYOK)\n  kind: client-supplied-credential\n  source: neuro-san README feature list\n  detail: '\"Secure Bring-Your-Own-Key (BYOK) support for client-provided\
  \ API keys so your deployments do not have\n    to shoulder everyone else''s token costs.\" These are LLM-PROVIDER keys (OpenAI and similar) that the caller\n    supplies, not credentials for the neuro-san API itself — an important distinction. They travel over the private\n    sly_data channel rather than an Authorization header, which is why they never surface as a securityScheme.'\n  enforced_by: client\n  transport: sly_data (private channel, deliberately excluded from the LLM chat stream)\n  evidence: neuro_san/registries/music_nerd_pro_sly_api_key.hocon and the paired test fixtures (tests/fixtures/music_nerd_pro_sly_api_key/{no_user_api_key,with_user_api_key}.hocon)\n    are the provider's own worked examples of an agent network that takes a user-supplied API key through sly_data.\nserver_side_credentials:\n  note: The credentials an OPERATOR must set to run a server are environment variables for downstream LLM providers,\n    not credentials for this API.\n  environment_variables:\n\
  \  - OPENAI_API_KEY\n  - AGENT_TOOL_PATH\n  - AGENT_MANIFEST_FILE\n  - PYTHONPATH\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key_header: null\ntransport_security:\n  https_enforced: false\n  detail: The provider's own documented examples use http://localhost:8080. TLS termination is the operator's responsibility;\n    nothing in the contract or docs requires it.\nagent_guidance: An agent integrating with a neuro-san deployment cannot learn the auth model from the contract and\n  must ask the operator. Assume no authentication is declared, expect the deployment to sit behind whatever the\n  operator put in front of it, and expect any LLM-provider key to be passed through sly_data rather than a header.\nmethod_note: 'method: none because the published contract declares no securitySchemes and no security requirement\n  on any operation - checked, nothing there. The documented_but_not_in_contract list below records the operator-side\n  mechanisms the docs describe; none\
  \ of them is a scheme a client can read from the contract, which is why schemes[]\n  stays empty rather than being filled from prose.'\n"
source_yaml_url: https://artifacts.apis.io/cognizant-technology/authentication/cognizant-technology-authentication.yml
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
