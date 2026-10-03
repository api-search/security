---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: polycode-co-uk-admin-api-openapi.yml
  format: yaml
  label: Polycode Admin API
  slug: polycode-co-uk-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-admin-api-openapi.yml
- filename: polycode-co-uk-budget-api-openapi.yml
  format: yaml
  label: Polycode Budget API
  slug: polycode-co-uk-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-budget-api-openapi.yml
- filename: polycode-co-uk-chat-api-openapi.yml
  format: yaml
  label: Polycode Chat API
  slug: polycode-co-uk-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-chat-api-openapi.yml
- filename: polycode-co-uk-diverts-api-openapi.yml
  format: yaml
  label: Polycode Diverts API
  slug: polycode-co-uk-diverts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-diverts-api-openapi.yml
- filename: polycode-co-uk-flag-api-openapi.yml
  format: yaml
  label: Polycode Flag API
  slug: polycode-co-uk-flag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-flag-api-openapi.yml
- filename: polycode-co-uk-graph-api-openapi.yml
  format: yaml
  label: Polycode Graph API
  slug: polycode-co-uk-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-graph-api-openapi.yml
- filename: polycode-co-uk-graphs-api-openapi.yml
  format: yaml
  label: Polycode Graphs API
  slug: polycode-co-uk-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-graphs-api-openapi.yml
- filename: polycode-co-uk-hooks-api-openapi.yml
  format: yaml
  label: Polycode Hooks API
  slug: polycode-co-uk-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-hooks-api-openapi.yml
- filename: polycode-co-uk-keys-api-openapi.yml
  format: yaml
  label: Polycode Keys API
  slug: polycode-co-uk-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-keys-api-openapi.yml
- filename: polycode-co-uk-me-api-openapi.yml
  format: yaml
  label: Polycode Me API
  slug: polycode-co-uk-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-me-api-openapi.yml
- filename: polycode-co-uk-openapi-json-api-openapi.yml
  format: yaml
  label: Polycode Openapi.json API
  slug: polycode-co-uk-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-openapi-json-api-openapi.yml
- filename: polycode-co-uk-project-api-openapi.yml
  format: yaml
  label: Polycode Project API
  slug: polycode-co-uk-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-project-api-openapi.yml
- filename: polycode-co-uk-projects-api-openapi.yml
  format: yaml
  label: Polycode Projects API
  slug: polycode-co-uk-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-projects-api-openapi.yml
- filename: polycode-co-uk-sessions-api-openapi.yml
  format: yaml
  label: Polycode Sessions API
  slug: polycode-co-uk-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-sessions-api-openapi.yml
- filename: polycode-co-uk-status-api-openapi.yml
  format: yaml
  label: Polycode Status API
  slug: polycode-co-uk-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-status-api-openapi.yml
- filename: polycode-co-uk-test-api-openapi.yml
  format: yaml
  label: Polycode Test API
  slug: polycode-co-uk-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-test-api-openapi.yml
- filename: polycode-co-uk-usage-api-openapi.yml
  format: yaml
  label: Polycode Usage API
  slug: polycode-co-uk-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-usage-api-openapi.yml
- filename: polycode-co-uk-visitor-api-openapi.yml
  format: yaml
  label: Polycode Visitor API
  slug: polycode-co-uk-visitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-visitor-api-openapi.yml
auth_types:
- none
- apiKey
- openIdConnect
- hmac
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Polycode Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polycode secures its APIs with none, apiKey, openIdConnect, and hmac across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Polycode
provider_slug: polycode-co-uk
scheme_count: 4
schemes:
- applies_to: 26 GET operations, postChat, postMechanicalCompletion, postFlag, postVisitorLabel, postSessionIntroduction, the A2A JSON-RPC endpoint
  evidence: 'info.description: "No auth today; the API is public."; agent card security: []; live GET /api/status, /api/graphs, /api/budget, /api/projects -> 200 anonymously.'
  name: public
  type: none
- applies_to:
  - whoamiKey
  - postHooksPush
  - getRepoSummary
  - postMechanicalCompletion (graph selection)
  - postChat / A2A (routes to the key's private graph)
  evidence: 'Agent card securitySchemes.apiKey (X-API-Key, "Optional today. Will gate a free monthly token allowance per key, with pay-as-you-go beyond it."); live GET /api/keys/whoami -> 401 {"error":"send the key as X-API-Key"}; account.mjs masks keys as "mga_…<suffix>"; README: "A private graph ... is reached by adding an x-api-key: header".'
  in: header
  issuance: Minted on the logged-in Account page ("generate a key" creates a private graph + key, shown once) or by the operator CLI (issue-key). Keys are 1:1 with a private graph; getKeys lists hash, issued_at and last-4 suffix, never plaintext.
  key_prefix: mga_
  name: apiKey
  parameter: X-API-Key
  type: apiKey
- applies_to: 'Tier-1 operations: getKeys, postKeys, createPrivateGraph, setMyDefaultGraph, clearUserDefault, setUserDefault, deletePrivateGraph, renamePrivateGraph, setRepo, getPromptNote, setPromptNote, postProjectOp (admin/owner), plus web search, projects and the fuller model in the chat UI'
  authorization_endpoint: https://eu-west-24yw02qhzm.auth.eu-west-2.amazoncognito.com/oauth2/authorize
  entry: https://marginalia.polycode.co.uk/auth/login
  evidence: 'GET /auth/login -> 302 to the Cognito authorize URL (response_type=code, redirect_uri /auth/callback); live GET /api/keys -> 401 {"error":"login required"}; app.mjs: "Log in with Google for web search, projects, and the fuller model".'
  name: cognitoLogin
  note: A browser session, not an API authorization flow — no bearer tokens are documented for API callers. The Cognito discovery URL was not probed.
  provider: Amazon Cognito (identity_provider=Google)
  scopes_requested:
  - openid
  - email
  - profile
  type: openIdConnect
- applies_to:
  - postGithubHook
  - postGitlabHook
  evidence: 'Spec summaries: X-Hub-Signature-256 "constant-time-verified against the org webhook secret"; X-Gitlab-Token "constant-time-validated against the binding"; 401 on bad signature or an unbound graph.'
  name: webhookSecrets
  note: Inbound connector authentication for bound repositories, issued by the operator CLI (bind-connector); not a caller credential.
  type: hmac
slug: polycode-co-uk-authentication
source_filename: polycode-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://marginalia.polycode.co.uk/.well-known/agent-card.json\ndocs: https://gitlab.com/polycode-projects/marginalia/-/blob/main/README.md\nnote: >-\n  The OpenAPI declares no securitySchemes (derive-authentication.py found none), so this profile is assembled\n  from the agent card's securitySchemes block, the operation summaries in the spec, the README (\"Talk to it —\n  the A2A API\", \"Repository supervision\"), the account page code, and live anonymous responses on 2026-09-19.\nsummary:\n  types: [none, apiKey, openIdConnect, hmac]\n  api_key_in: [header]\n  oauth2_flows: []\n  default: public — no credential for reads, chat, the A2A endpoint or the mechanical completions shim\nschemes:\n- name: public\n  type: none\n  applies_to: 26 GET operations, postChat, postMechanicalCompletion, postFlag, postVisitorLabel, postSessionIntroduction, the A2A JSON-RPC endpoint\n  evidence: 'info.description: \"No auth today; the API is\
  \ public.\"; agent card security: []; live GET /api/status, /api/graphs, /api/budget, /api/projects -> 200 anonymously.'\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: mga_\n  applies_to: [whoamiKey, postHooksPush, getRepoSummary, postMechanicalCompletion (graph selection), postChat / A2A (routes to the key's private graph)]\n  evidence: >-\n    Agent card securitySchemes.apiKey (X-API-Key, \"Optional today. Will gate a free monthly token allowance per key,\n    with pay-as-you-go beyond it.\"); live GET /api/keys/whoami -> 401 {\"error\":\"send the key as X-API-Key\"}; account.mjs\n    masks keys as \"mga_…<suffix>\"; README: \"A private graph ... is reached by adding an x-api-key: header\".\n  issuance: Minted on the logged-in Account page (\"generate a key\" creates a private graph + key, shown once) or by the operator CLI (issue-key). Keys are 1:1 with a private graph; getKeys lists hash, issued_at and last-4 suffix, never plaintext.\n- name: cognitoLogin\n\
  \  type: openIdConnect\n  provider: Amazon Cognito (identity_provider=Google)\n  authorization_endpoint: https://eu-west-24yw02qhzm.auth.eu-west-2.amazoncognito.com/oauth2/authorize\n  scopes_requested: [openid, email, profile]\n  entry: https://marginalia.polycode.co.uk/auth/login\n  applies_to: 'Tier-1 operations: getKeys, postKeys, createPrivateGraph, setMyDefaultGraph, clearUserDefault, setUserDefault, deletePrivateGraph, renamePrivateGraph, setRepo, getPromptNote, setPromptNote, postProjectOp (admin/owner), plus web search, projects and the fuller model in the chat UI'\n  evidence: 'GET /auth/login -> 302 to the Cognito authorize URL (response_type=code, redirect_uri /auth/callback); live GET /api/keys -> 401 {\"error\":\"login required\"}; app.mjs: \"Log in with Google for web search, projects, and the fuller model\".'\n  note: A browser session, not an API authorization flow — no bearer tokens are documented for API callers. The Cognito discovery URL was not probed.\n- name: webhookSecrets\n\
  \  type: hmac\n  applies_to: [postGithubHook, postGitlabHook]\n  evidence: 'Spec summaries: X-Hub-Signature-256 \"constant-time-verified against the org webhook secret\"; X-Gitlab-Token \"constant-time-validated against the binding\"; 401 on bad signature or an unbound graph.'\n  note: Inbound connector authentication for bound repositories, issued by the operator CLI (bind-connector); not a caller credential.\ntiers:\n- {tier: 0, name: visitor / anonymous, access: public reads, chat on the shared graph, A2A}\n- {tier: 1, name: logged in (Google via Cognito), access: private graphs, API keys, per-user default graph, web search and the fuller model in chat}\n- {tier: admin, name: operator, access: admin operations (postWorkItem, postAdminTurn, postDelivery, refreshInsights on the shared graph)}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/authentication/polycode-co-uk-authentication.yml
summary_line: none/apiKey/openIdConnect/hmac · 4 schemes
tags:
- Chat
- Memory
- Agents
- A2A
- Knowledge Graph
- Research
- Artificial Intelligence
- Open Source
- Consulting
- United Kingdom
---
