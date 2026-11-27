---
anonymous_access: false
api_key_in: []
auth_types:
- hmac-signature
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CreationLoop Authentication
name_suffix: Authentication
oauth_flows: []
overview: CreationLoop secures its APIs with hmac-signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CreationLoop
provider_slug: creationloop-ai
scheme_count: 1
schemes:
- description: Every event in the record arrived authenticated to the submitting agent's signing secret. Events are delivered over one signed webhook; signatures use HMAC-SHA256. The signing key is issued during design-partner onboarding ("We confirm a mutual fit, then issue your agent's signing key.").
  evidence:
  - Every event in the record arrived authenticated to the submitting agent's signing secret. Events are delivered over one signed webhook; signatures use HMAC-SHA256.
  in: header
  name: agentSigningSecret
  type: apiKey
  x-mechanism: HMAC-SHA256 webhook signature
slug: creationloop-ai-authentication
source_filename: creationloop-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://creationcode.ai/llms-full.txt\ndocs: https://creationcode.ai/whitepaper\nnote: No OpenAPI is published, so nothing is derived. CreationLoop documents one ingestion mechanism (a signed webhook from the operator's agent) and an MCP server whose tools serve site copy. The MCP endpoint's authentication is not documented; the pre-flight contract probe listed its 4 tools without credentials. Member sign-in to the marketplace uses passkeys (per the website), which is an end-user login, not API auth.\nsummary:\n  types:\n  - hmac-signature\nschemes:\n- name: agentSigningSecret\n  type: apiKey\n  in: header\n  x-mechanism: HMAC-SHA256 webhook signature\n  description: Every event in the record arrived authenticated to the submitting agent's signing secret. Events are delivered over one signed webhook; signatures use HMAC-SHA256. The signing key is issued during design-partner onboarding (\"We confirm a mutual fit, then issue\
  \ your agent's signing key.\").\n  evidence:\n  - 'Every event in the record arrived authenticated to the submitting agent''s signing secret. Events are delivered over one signed webhook; signatures use HMAC-SHA256.'\n"
source_yaml_url: https://artifacts.apis.io/creationloop-ai/authentication/creationloop-ai-authentication.yml
summary_line: hmac-signature · 1 scheme
tags:
- Company
- Expert Network
- Sales Intelligence
- Marketplace
- B2B Sales
- AI Agents
- MCP
---
