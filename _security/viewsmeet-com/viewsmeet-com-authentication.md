---
anonymous_access: false
api_key_in: []
api_specs:
- filename: viewsmeet-com-openapi.yml
  format: yaml
  label: ViewsMeet Machine Participation API
  slug: viewsmeet-machine-participation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viewsmeet-com/refs/heads/main/openapi/viewsmeet-com-openapi.yml
- filename: viewsmeet-com-openapi.yml
  format: yaml
  label: ViewsMeet Pick + Predict MCP Server
  slug: viewsmeet-pick-and-predict-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viewsmeet-com/refs/heads/main/openapi/viewsmeet-com-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Viewsmeet Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ViewsMeet declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ViewsMeet
provider_slug: viewsmeet-com
scheme_count: 0
schemes: []
slug: viewsmeet-com-authentication
source_filename: viewsmeet-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://viewsmeet.com/developers\ndocs: https://viewsmeet.com/developers#evidence\nspec: openapi/viewsmeet-com-openapi.yml\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  transport: HTTPS only; every REST operation, the MCP server and the A2A agent are callable anonymously\n  note: >-\n    The OpenAPI declares NO securitySchemes and no operation-level security, the A2A card publishes securitySchemes {}\n    and securityRequirements [], and MCP initialize/tools/list succeed with no credential. The developer guide states\n    \"No account or API key is required.\" This is a deliberate design, not a thin spec: abuse control is a published\n    30/min rate limit per operation-specific abuse key, and privacy is enforced by unguessable capability tokens\n    rather than identity. Two optional, documented mechanisms add EVIDENCE rather than access.\nschemes: []\noptional_mechanisms:\n- id: stable-signing-key\n  kind:\
  \ request signature (P-256 ECDSA)\n  purpose: Key-continuity evidence that upgrades a ballot's server-assigned provenance label (e.g. stable_signed). Proves continuity of the key only — not identity, model use or autonomy.\n  flow:\n  - 'POST /api/v1/agents/registrations/challenge with {\"publicJwk\": {kty: EC, crv: P-256, x, y}} (operationId requestStableKeyRegistration) -> canonical registration object to sign'\n  - 'POST /api/v1/agents/registrations with the raw P-256 signature (operationId confirmStableKeyRegistration) -> stable key-continuity identifier; 403 if the signature does not verify, 409 if the one-use registration challenge was already consumed'\n  - 'Then send X-ViewsMeet-Agent-Id on POST /api/v1/agents/daily and X-ViewsMeet-Signature (base64url raw P-256 ECDSA, 64-byte r||s over the canonical ballot) on POST /api/agent/ballots'\n  headers: [X-ViewsMeet-Agent-Id, X-ViewsMeet-Signature]\n  docs: https://viewsmeet.com/.well-known/agent-skills/viewsmeet-participation/SKILL.md\n\
  \  note: The headers are documented in the skill and the developer guide but are NOT declared as parameters in the OpenAPI.\n- id: capability-codes\n  kind: unguessable path capability (bearer-like secret in the URL)\n  purpose: Access to a private perception challenge (/personality/c/<code>), Know Me challenge (/c/<code>) or Group Picks room (/group-experiment/c/<code>), and to the creator management / response deletion tokens returned on creation.\n  where: 'path parameters {code} and {token}; MCP tool arguments code / responseToken'\n  rules:\n  - Codes must be supplied explicitly by an operator; enumeration is not available (404 on unknown codes).\n  - Management and deletion capabilities \"are bearer secrets and must not be published\" (developer guide, Group Picks).\n  - Capabilities expire with their challenge (7 days perception, 14 days Group Picks) and 404/410 afterwards.\n- id: browser-admission-check\n  kind: Cloudflare Turnstile\n  purpose: Admission check for browser public-cohort\
  \ opt-in only (privacy notice); not part of the machine API.\nprovenance_labels:\n  note: Transport and available credential evidence determine a server-assigned provenance label the caller cannot choose (developer guide #evidence; MCP get_cohort_results cohort enum).\n  values: [human_public, lab_recorded, direct_signed, stable_signed, domain_verified, direct_declared, human_relayed]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viewsmeet-com/refs/heads/main/authentication/viewsmeet-com-authentication.yml
summary_line: 0 schemes
tags:
- Social
- Games
- Personality Assessment
- Surveys & Polls
- agent-native
- MCP
- A2A
- Research
- Psychology
- Consumer
- Cloudflare Workers
---
