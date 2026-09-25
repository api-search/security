---
anonymous_access: false
api_key_in: []
api_specs:
- filename: typesafe-ai-openapi.yml
  format: yaml
  label: TypeSafe System One API
  slug: system-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesafe-ai/refs/heads/main/openapi/typesafe-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Typesafe Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: TypeSafe AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TypeSafe AI
provider_slug: typesafe-ai
scheme_count: 1
schemes:
- applied_note: The served spec declares components.securitySchemes.HTTPBearer but sets NO root `security` requirement and no per-operation `security`, so the scheme is defined and never applied. Both operations do require it in practice (401 Unauthorized on a missing or invalid key, per the published error table). The gap is fixed without mutating the original in overlays/typesafe-ai-openapi-overlay.yaml.
  applied_to: all operations
  documented: true
  format: Bearer <API_KEY>
  header: Authorization
  in: header
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/typesafe-ai-openapi.yml
  - https://docs.typesafe.ai/api
  type: http
slug: typesafe-ai-authentication
source_filename: typesafe-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://docs.typesafe.ai/api (Evaluation endpoint), https://docs.typesafe.ai/introduction/quickstart,\n  https://docs.typesafe.ai/sdk/python, https://docs.typesafe.ai/sdk/javascript and\n  https://docs.typesafe.ai/agent-skill — corroborated by the securitySchemes block in\n  openapi/typesafe-ai-openapi.yml (derived first, then upgraded from the docs).\ndocs: https://docs.typesafe.ai/api\nsummary:\n  types:\n  - http\n  model: static-bearer-api-key\n  model_note: >-\n    One mechanism, one credential, no negotiation. The API key IS the bearer token — there is no\n    token exchange, no OAuth flow, no refresh, no expiry documented, and no scope system. For an\n    agent this is the simplest possible auth story and also the least granular: a key is all-or-nothing\n    over both operations.\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  scopes: false\n  scopes_note: >-\n    No scopes/ artifact is written and\
  \ no OAuthScopes pointer is emitted. Nothing in the spec or the\n    docs declares an oauth2 securityScheme or a permission surface, so an empty scopes file would\n    assert a structure TypeSafe does not have.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <API_KEY>'\n  documented: true\n  applied_to: all operations\n  applied_note: >-\n    The served spec declares components.securitySchemes.HTTPBearer but sets NO root `security`\n    requirement and no per-operation `security`, so the scheme is defined and never applied. Both\n    operations do require it in practice (401 Unauthorized on a missing or invalid key, per the\n    published error table). The gap is fixed without mutating the original in\n    overlays/typesafe-ai-openapi-overlay.yaml.\n  sources:\n  - openapi/typesafe-ai-openapi.yml\n  - https://docs.typesafe.ai/api\ncredential:\n  kind: api-key\n  issuance: >-\n    Self-serve from the console once an\
  \ account exists — https://console.typesafe.ai/keys (the page\n    302s to /login when unauthenticated). Account creation is gated: the marketing site's primary\n    call to action is \"Join Waitlist\" and Jev is described as early access.\n  env_var: TYPESAFE_API_KEY\n  env_var_note: >-\n    Both official SDKs read TYPESAFE_API_KEY from the environment with no argument, and the published\n    Agent Skill instructs agents to use the same variable. That single convention is what makes the\n    key usable by an agent without prompting a human for it.\n  rotation_documented: false\n  expiry_documented: false\n  prefix_documented: false\n  prefix_note: >-\n    No key prefix is published (no \"ts_live_\"-style discriminator documented), so a leaked key\n    cannot be recognised by shape and there is no published test-vs-live key distinction. See\n    sandbox/typesafe-ai-sandbox.yml.\ntransport:\n  https_required: true\n  tls: TLSv1.3 observed on api.typesafe.ai\n  hsts: false\n  hsts_note:\
  \ >-\n    api.typesafe.ai serves no Strict-Transport-Security header (typesafe.ai and docs.typesafe.ai\n    both do). See security/typesafe-ai-domain-security.yml.\nfailure_modes:\n- status: 401\n  meaning: Missing or invalid API key. Check the Authorization header.\n  source: https://docs.typesafe.ai/api\n- status: 422\n  meaning: Request body failed validation; the body details the offending field.\n  source: openapi/typesafe-ai-openapi.yml\nagent_notes: >-\n  A bearer key in a header, one env var, no refresh and no scopes means an agent can authenticate in\n  one line and can NOT be granted least privilege. There is nothing to restrict a key to\n  GET /v1/models, so any agent holding a key can spend tokens on POST /v1/systemone. Cost, not data\n  loss, is the exposure — see plans/typesafe-ai-plans-pricing.yml for the published per-token price.\ncross_links:\n  conventions: conventions/typesafe-ai-conventions.yml\n  errors: errors/typesafe-ai-problem-types.yml\n  overlay: overlays/typesafe-ai-openapi-overlay.yaml\n\
  \  domain_security: security/typesafe-ai-domain-security.yml\n  rate_limits: rate-limits/typesafe-ai-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typesafe-ai/refs/heads/main/authentication/typesafe-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine Learning
- Classification
- Content Moderation
- Decision Support
- Structured Outputs
- Inference
- LLM Alternative
- Agent Skills
- MCP
- Agent-Native
- Developer Tools
- A2A
---
