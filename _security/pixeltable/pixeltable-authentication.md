---
api_key_in:
- header
auth_types:
- none
- apiKey
- session
description: ''
kind: authentication
layout: security
method: searched
name: Pixeltable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixeltable secures its APIs with none, apiKey, and session across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pixeltable
provider_slug: pixeltable
scheme_count: 5
schemes:
- name: open_source_library
  note: The open-source library needs no credential of any kind. AI provider keys (OpenAI, Anthropic, etc.) are the user's own and are held in ~/.pixeltable/config.toml — they authenticate to third parties, not to Pixeltable.
  published: pip install pixeltable — no auth required
  required: false
  source: https://www.pixeltable.com/.well-known/agent.json
  surface: pixeltable Python library
  type: none
- api: pixeltable-webmcp
  name: webmcp_anonymous
  note: Confirmed anonymous. An unauthenticated JSON-RPC tools/list returned HTTP 200 with the full tool set on 2026-08-17. No OAuth challenge was issued and neither /.well-known/oauth-authorization-server nor /.well-known/oauth-protected-resource is served (both 404), which is consistent with a read-only server that requires no authorization.
  required: false
  surface: https://pixeltable.com/mcp
  type: none
  verified: probed
- api: pixeltable-ask
  name: ask_anonymous
  note: Confirmed anonymous. An unauthenticated POST with a `query` body returned HTTP 200 and grounded results. Protected by a per-IP rate limit rather than a credential.
  required: false
  surface: https://pixeltable.com/ask
  type: none
  verified: probed
- api: pixeltable-cloud-control-plane
  docs: https://pixeltable.com/developers/llms.txt
  in: header
  name: cloud_api_key
  note: CLAIM NOT REPRODUCIBLE ANONYMOUSLY. The provider marks this scheme "available", but a request to https://pixeltable.com/api/v1 carrying an X-api-key header returned HTTP 401 with {"message":"Authentication required","reason":"no_session_cookie_provided"} — the endpoint asked for a session cookie, not an API key. Either the key-authenticated routes live elsewhere (undocumented) or the documented header does not yet gate this path. Not resolvable without a real key; recorded honestly.
  parameter_name: X-api-key
  published: 'cloud_api: {type: api_key, header: X-api-key, status: available}'
  required: true
  source: https://www.pixeltable.com/.well-known/agent.json
  status_claimed: available
  surface: Pixeltable Cloud API
  type: apiKey
  verified: probed
- api: pixeltable-cloud-control-plane
  login_url: https://pixeltable.com/login
  name: workos_authkit_session
  note: Confirmed. https://pixeltable.com/signup and /login both 302 to signin.pixeltable.com with a WorkOS client_id (client_01JJMGYGHGE0KMSZWF0WZGHMC0) and a redirect_uri of https://pixeltable.com/api/auth/callback. The security page states Pixeltable "leverage[s] industry-standard authentication practices through WorkOS AuthKit". Bearer tokens issued by WorkOS authenticate the control plane per the developer llms.txt.
  provider: WorkOS AuthKit
  required: true
  signup_url: https://pixeltable.com/signup
  sso: Single Sign-On supported where applicable; SAML SSO is a Pro "contact us" / Enterprise feature per the pricing page.
  surface: Pixeltable Cloud dashboard and pxt CLI
  type: session
  verified: probed
slug: pixeltable-authentication
source_filename: pixeltable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: 'https://www.pixeltable.com/.well-known/agent.json, https://pixeltable.com/developers/llms.txt,\n  https://pixeltable.com/security, plus live probes'\nnote: '0-working/derive-authentication.py produced no profile for this provider (0 auth profiles) because\n  there is no OpenAPI in the repo to read securitySchemes from — Pixeltable publishes none. This artifact is\n  therefore SEARCHED from the provider''s own capability manifest and developer documentation, and each claim\n  was checked against a live probe where a probe was possible. Pixeltable has FOUR distinct auth postures\n  across its surfaces, which is the important finding: two agent surfaces are fully anonymous while the cloud\n  control plane is session-gated.'\nsummary:\n  types:\n  - none\n  - apiKey\n  - session\n  api_key_in:\n  - header\n  api_key_header: X-api-key\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\n  anonymous_surfaces: 2\n  gated_surfaces:\
  \ 1\nschemes:\n- name: open_source_library\n  surface: pixeltable Python library\n  type: none\n  required: false\n  published: 'pip install pixeltable — no auth required'\n  source: https://www.pixeltable.com/.well-known/agent.json\n  note: 'The open-source library needs no credential of any kind. AI provider keys (OpenAI, Anthropic, etc.)\n    are the user''s own and are held in ~/.pixeltable/config.toml — they authenticate to third parties, not to\n    Pixeltable.'\n- name: webmcp_anonymous\n  surface: https://pixeltable.com/mcp\n  api: pixeltable-webmcp\n  type: none\n  required: false\n  verified: probed\n  note: 'Confirmed anonymous. An unauthenticated JSON-RPC tools/list returned HTTP 200 with the full tool set\n    on 2026-08-17. No OAuth challenge was issued and neither\n    /.well-known/oauth-authorization-server nor /.well-known/oauth-protected-resource is served (both 404),\n    which is consistent with a read-only server that requires no authorization.'\n- name: ask_anonymous\n\
  \  surface: https://pixeltable.com/ask\n  api: pixeltable-ask\n  type: none\n  required: false\n  verified: probed\n  note: Confirmed anonymous. An unauthenticated POST with a `query` body returned HTTP 200 and grounded\n    results. Protected by a per-IP rate limit rather than a credential.\n- name: cloud_api_key\n  surface: Pixeltable Cloud API\n  api: pixeltable-cloud-control-plane\n  type: apiKey\n  in: header\n  parameter_name: X-api-key\n  required: true\n  status_claimed: available\n  published: 'cloud_api: {type: api_key, header: X-api-key, status: available}'\n  source: https://www.pixeltable.com/.well-known/agent.json\n  docs: https://pixeltable.com/developers/llms.txt\n  verified: probed\n  note: 'CLAIM NOT REPRODUCIBLE ANONYMOUSLY. The provider marks this scheme \"available\", but a request to\n    https://pixeltable.com/api/v1 carrying an X-api-key header returned HTTP 401 with\n    {\"message\":\"Authentication required\",\"reason\":\"no_session_cookie_provided\"} — the endpoint\
  \ asked for a\n    session cookie, not an API key. Either the key-authenticated routes live elsewhere (undocumented) or the\n    documented header does not yet gate this path. Not resolvable without a real key; recorded honestly.'\n- name: workos_authkit_session\n  surface: Pixeltable Cloud dashboard and pxt CLI\n  api: pixeltable-cloud-control-plane\n  type: session\n  provider: WorkOS AuthKit\n  required: true\n  signup_url: https://pixeltable.com/signup\n  login_url: https://pixeltable.com/login\n  sso: 'Single Sign-On supported where applicable; SAML SSO is a Pro \"contact us\" / Enterprise feature per the\n    pricing page.'\n  verified: probed\n  note: 'Confirmed. https://pixeltable.com/signup and /login both 302 to signin.pixeltable.com with a WorkOS\n    client_id (client_01JJMGYGHGE0KMSZWF0WZGHMC0) and a redirect_uri of\n    https://pixeltable.com/api/auth/callback. The security page states Pixeltable \"leverage[s]\n    industry-standard authentication practices through WorkOS\
  \ AuthKit\". Bearer tokens issued by WorkOS\n    authenticate the control plane per the developer llms.txt.'\nplanned:\n- name: public_rest_oauth\n  type: oauth2\n  status: planned\n  published: 'public_rest_api: {type: oauth_scoped, status: planned}'\n  source: https://www.pixeltable.com/.well-known/agent.json\n  note: 'A public REST API with OpenAPI and scoped OAuth is stated as in active development. No authorization\n    server metadata is published yet (/.well-known/oauth-authorization-server 404s), so there are no scopes to\n    capture — scopes/ is deliberately absent for this provider.'\nx-evidence:\n- url: https://www.pixeltable.com/.well-known/agent.json\n  http_status: 200\n  fetched: '2026-08-17'\n- url: https://www.pixeltable.com/mcp\n  method: POST\n  http_status: 200\n  fetched: '2026-08-17'\n  note: anonymous tools/list succeeded\n- url: https://www.pixeltable.com/api/v1\n  method: GET\n  http_status: 401\n  fetched: '2026-08-17'\n  note: 'with X-api-key header; body reason\
  \ no_session_cookie_provided'\n- url: https://pixeltable.com/signup\n  http_status: 200\n  fetched: '2026-08-17'\n  note: redirects to signin.pixeltable.com (WorkOS AuthKit)\n- url: https://www.pixeltable.com/.well-known/oauth-authorization-server\n  http_status: 404\n  fetched: '2026-08-17'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixeltable/refs/heads/main/authentication/pixeltable-authentication.yml
summary_line: none/apiKey/session · 5 schemes
tags:
- Company
- Ai Data
- Multimodal AI
- AI Data Infrastructure
- Vector Search
- Embeddings
- RAG
- Agent Memory
- MCP
- Open-Source
- Python
- Data Orchestration
- Computed Columns
- Video Processing
- Machine-Learning
---
