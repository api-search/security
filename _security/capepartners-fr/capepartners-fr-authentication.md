---
anonymous_access: false
api_key_in:
- path
- header
api_specs:
- filename: capepartners-fr-openapi.yml
  format: yaml
  label: Cape Partners Sniffer Agent API
  slug: cape-partners-sniffer-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capepartners-fr/refs/heads/main/openapi/capepartners-fr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Capepartners Fr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cape Partners secures its APIs with apiKey across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cape Partners
provider_slug: capepartners-fr
scheme_count: 6
schemes:
- declared_in_spec_as: apiKey in header X-Session-Id (documentary only)
  description: The workspace session UUID is a capability token carried in the URL PATH. A valid request must present a well-formed UUID-v4 in the {session_id} path segment AND either no Origin/Referer or a first-party one (capepartners.fr, www.capepartners.fr, sniffer.capepartners.fr, localhost, 127.0.0.1). A malformed id answers 400 "Invalid session identifier"; a known-foreign Origin/Referer answers 403 "Cross-origin request rejected"; a headless agent should simply send no Origin/Referer. Applies to every /api/*/{session_id} operation and to body-keyed writes that carry session_id.
  in: path
  issued_by: POST /api/workspace/join (returns session_id / uuid). An agent (no Turnstile token) must present an ACCEPTED exchange manifest key as exchange_key before a NEW uuid is issued — otherwise 403 handshake_required. A join never takes over an existing workspace (403 workspace_not_yours).
  name: SessionToken
  parameter: '{session_id}'
  sources:
  - openapi/capepartners-fr-openapi.yml
  - https://www.capepartners.fr/api
  - https://www.capepartners.fr/.well-known/ai-plugin.json
  type: apiKey
- declared_in_spec_as: apiKey in header X-Nda-Signed (documentary only)
  description: 'NDA-gated resources — GET /api/matched-names/{session_id}, GET /api/seller-name/{session_id}, GET /api/infomemo/{session_id}, GET /api/infomemo/{session_id}/download, and GET /api/search/{session_id} — serve data only after a signature is recorded via POST /api/nda/sign. Unsigned answers 403 with nda_required:true. A signature alone is not sufficient: the session''s registered email must also be a validated mailbox (fix_required names the field). Signing requires a declared HUMAN supervisor bound at registration; an agent-initiated signature is recorded as pending and unlocks nothing until the supervisor approves via an emailed link.'
  in: server-side
  name: NdaSigned
  parameter: nda_signatures record for {session_id}
  sources:
  - openapi/capepartners-fr-openapi.yml
  - https://www.capepartners.fr/api
  - https://www.capepartners.fr/llms.txt
  type: precondition
- declared_in: a2a/capepartners-fr-agent-card.json (securitySchemes.exchangeKey, apiKeySecurityScheme)
  description: 'The capability key issued when an agent sends its first message — its msgid — or the stronger answer_key given on first read. Authorizes the caller''s own tasks/thread and nothing else. "The id identifies, the key authorizes": a task id alone is never enough, and a non-matching key is reported exactly like a missing task (TASK_NOT_FOUND / 404 "no record for that key"). Sending the first message needs no key at all.'
  in: header
  name: exchangeKey
  parameter: X-A2A-Key
  sources:
  - a2a/capepartners-fr-agent-card.json
  - https://www.capepartners.fr/agent-exchange.html
  surface: A2A (POST /a2a, POST /a2a/message:send, GET /a2a/tasks, GET /a2a/tasks/{id}) and the REST twins (GET /api/exchange/answer/{msgid}, POST /api/exchange/reply body.key)
  type: apiKey
- declared_in: a2a/capepartners-fr-agent-card.json (securitySchemes.bearerKey, httpAuthSecurityScheme)
  description: The same exchange capability key, presented as an HTTP bearer credential instead of X-A2A-Key.
  name: bearerKey
  parameter: 'Authorization: Bearer <msgid or answer_key>'
  scheme: bearer
  sources:
  - a2a/capepartners-fr-agent-card.json
  surface: A2A
  type: http
- description: An opaque, operator-issued token bound to an exchange participant (issued by POST /engage/issue, admin-gated). Gives read-only assistants that cannot POST or hold a session a UUID-free view of a thread or of pre-NDA redacted matches. An unbound token answers 400; an unknown or revoked token answers 401. The raw session UUID is never exposed through this gateway.
  in: path
  name: engageToken
  parameter: '{token}'
  sources:
  - openapi/capepartners-fr-openapi.yml
  - https://www.capepartners.fr/engage
  - https://www.capepartners.fr/llms.txt
  surface: GET /engage/{token}/thread, POST /engage/{token}/reply, GET /engage/{token}/matches, GET /engage/{token}/summary
  type: apiKey
- description: Registration is human-gated by Cloudflare Turnstile. A human solving the widget sends turnstileToken, which the server verifies when present (403 on failure). An agent POSTing directly sends none and is classified as an agent; POST /api/submit then requires a declared human supervisor in the body ({"supervisor":{"name","email","company"}}) or answers 403 "Human verification failed". Consumer webmail addresses (gmail/outlook/hotmail/yahoo) are rejected on join — a verified business email is required.
  in: body
  name: turnstile
  parameter: turnstileToken (optional) or supervisor {name, email, company}
  sources:
  - https://www.capepartners.fr/api
  - https://www.capepartners.fr/llms.txt
  surface: POST /api/submit, POST /api/workspace/join
  type: human-verification
slug: capepartners-fr-authentication
source_filename: capepartners-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/capepartners-fr-openapi.yml (securitySchemes) upgraded from the provider's own auth documentation — https://www.capepartners.fr/api (auth + guards blocks), https://www.capepartners.fr/.well-known/ai-plugin.json (auth.instructions), https://www.capepartners.fr/llms.txt, https://www.capepartners.fr/agent-exchange.html and the Agent Card securitySchemes.\ndocs: https://www.capepartners.fr/api\nspec: openapi/capepartners-fr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\n  - header\n  oauth2_flows: []\n  transport: HTTPS only; Cloudflare in front; Referrer-Policy strict-origin-when-cross-origin on every response\n  note: 'No API key at any tier and no OAuth. The provider''s auth model (its own words, /api and ai-plugin.json) is \"path-capability-token + NDA\": a workspace session UUID-v4 carried in the URL path is the credential for the workspace API, a recorded human NDA/Terms signature is a second\
  \ precondition for confidential resources, and the agent exchange / A2A surface uses a separate capability key (the msgid issued with the first message, or the answer_key given on first read) sent as X-A2A-Key or a Bearer token. The OpenAPI models the first two as apiKey-in-header schemes only because securitySchemes cannot express a path credential — the header names X-Session-Id and X-Nda-Signed are NOT literal headers, and the spec says so in each description.'\nschemes:\n- name: SessionToken\n  type: apiKey\n  in: path\n  parameter: '{session_id}'\n  declared_in_spec_as: apiKey in header X-Session-Id (documentary only)\n  description: The workspace session UUID is a capability token carried in the URL PATH. A valid request must present a well-formed UUID-v4 in the {session_id} path segment AND either no Origin/Referer or a first-party one (capepartners.fr, www.capepartners.fr, sniffer.capepartners.fr, localhost, 127.0.0.1). A malformed id answers 400 \"Invalid session identifier\"\
  ; a known-foreign Origin/Referer answers 403 \"Cross-origin request rejected\"; a headless agent should simply send no Origin/Referer. Applies to every /api/*/{session_id} operation and to body-keyed writes that carry session_id.\n  issued_by: POST /api/workspace/join (returns session_id / uuid). An agent (no Turnstile token) must present an ACCEPTED exchange manifest key as exchange_key before a NEW uuid is issued — otherwise 403 handshake_required. A join never takes over an existing workspace (403 workspace_not_yours).\n  sources:\n  - openapi/capepartners-fr-openapi.yml\n  - https://www.capepartners.fr/api\n  - https://www.capepartners.fr/.well-known/ai-plugin.json\n- name: NdaSigned\n  type: precondition\n  in: server-side\n  parameter: nda_signatures record for {session_id}\n  declared_in_spec_as: apiKey in header X-Nda-Signed (documentary only)\n  description: 'NDA-gated resources — GET /api/matched-names/{session_id}, GET /api/seller-name/{session_id}, GET /api/infomemo/{session_id},\
  \ GET /api/infomemo/{session_id}/download, and GET /api/search/{session_id} — serve data only after a signature is recorded via POST /api/nda/sign. Unsigned answers 403 with nda_required:true. A signature alone is not sufficient: the session''s registered email must also be a validated mailbox (fix_required names the field). Signing requires a declared HUMAN supervisor bound at registration; an agent-initiated signature is recorded as pending and unlocks nothing until the supervisor approves via an emailed link.'\n  sources:\n  - openapi/capepartners-fr-openapi.yml\n  - https://www.capepartners.fr/api\n  - https://www.capepartners.fr/llms.txt\n- name: exchangeKey\n  type: apiKey\n  in: header\n  parameter: X-A2A-Key\n  surface: 'A2A (POST /a2a, POST /a2a/message:send, GET /a2a/tasks, GET /a2a/tasks/{id}) and the REST twins (GET /api/exchange/answer/{msgid}, POST /api/exchange/reply body.key)'\n  description: 'The capability key issued when an agent sends its first message — its msgid —\
  \ or the stronger answer_key given on first read. Authorizes the caller''s own tasks/thread and nothing else. \"The id identifies, the key authorizes\": a task id alone is never enough, and a non-matching key is reported exactly like a missing task (TASK_NOT_FOUND / 404 \"no record for that key\"). Sending the first message needs no key at all.'\n  declared_in: a2a/capepartners-fr-agent-card.json (securitySchemes.exchangeKey, apiKeySecurityScheme)\n  sources:\n  - a2a/capepartners-fr-agent-card.json\n  - https://www.capepartners.fr/agent-exchange.html\n- name: bearerKey\n  type: http\n  scheme: bearer\n  parameter: 'Authorization: Bearer <msgid or answer_key>'\n  surface: A2A\n  description: The same exchange capability key, presented as an HTTP bearer credential instead of X-A2A-Key.\n  declared_in: a2a/capepartners-fr-agent-card.json (securitySchemes.bearerKey, httpAuthSecurityScheme)\n  sources:\n  - a2a/capepartners-fr-agent-card.json\n- name: engageToken\n  type: apiKey\n  in: path\n\
  \  parameter: '{token}'\n  surface: 'GET /engage/{token}/thread, POST /engage/{token}/reply, GET /engage/{token}/matches, GET /engage/{token}/summary'\n  description: An opaque, operator-issued token bound to an exchange participant (issued by POST /engage/issue, admin-gated). Gives read-only assistants that cannot POST or hold a session a UUID-free view of a thread or of pre-NDA redacted matches. An unbound token answers 400; an unknown or revoked token answers 401. The raw session UUID is never exposed through this gateway.\n  sources:\n  - openapi/capepartners-fr-openapi.yml\n  - https://www.capepartners.fr/engage\n  - https://www.capepartners.fr/llms.txt\n- name: turnstile\n  type: human-verification\n  in: body\n  parameter: turnstileToken (optional) or supervisor {name, email, company}\n  surface: POST /api/submit, POST /api/workspace/join\n  description: Registration is human-gated by Cloudflare Turnstile. A human solving the widget sends turnstileToken, which the server verifies\
  \ when present (403 on failure). An agent POSTing directly sends none and is classified as an agent; POST /api/submit then requires a declared human supervisor in the body ({\"supervisor\":{\"name\",\"email\",\"company\"}}) or answers 403 \"Human verification failed\". Consumer webmail addresses (gmail/outlook/hotmail/yahoo) are rejected on join — a verified business email is required.\n  sources:\n  - https://www.capepartners.fr/api\n  - https://www.capepartners.fr/llms.txt\nguards:\n  uuid: 400 — Invalid session identifier (UUID-v4 required), checked before anything else is touched\n  cross_origin: 403 — a present Origin/Referer must be a Cape Partners first-party host; absent is allowed\n  rate_limit: 429 — rolling per-IP 60 requests / 60 s per endpoint family on confidential reads, retry_after (seconds) in the JSON body\n  nda: 403 — nda_required:true until a human-approved signature is recorded; then the registered email must be a validated mailbox\n  turnstile: 403 — Human verification\
  \ failed on POST /api/submit and POST /api/workspace/join unless a human supervisor is declared\ncredentials:\n  - id: workspace-session-uuid\n    where: URL path segment {session_id} (and body session_id on some writes)\n    prefix: null\n    format: UUID v4\n    use: Every workspace operation (session, matches, valuation, pairings, deal flow, interest signals, activity, info memos, mandate)\n    issued_by: POST /api/workspace/join\n    note: 'The provider''s homepage tells agents to \"treat it like a password\" — anyone holding the UUID can read name, email, company and financials. Do not log it or put it in a Referer (the server sets Referrer-Policy strict-origin-when-cross-origin for this reason).'\n  - id: exchange-key\n    where: X-A2A-Key header, Authorization Bearer, or body.key on POST /api/exchange/reply\n    prefix: null\n    format: msgid from the submission receipt, or answer_key from the first read\n    use: Reading and answering the agent's own exchange thread / A2A tasks;\
  \ presented as exchange_key on POST /api/workspace/join to upgrade to a workspace\n    issued_by: The first SendMessage / POST /api/exchange/manifest (no credential needed to obtain it)\n  - id: engage-token\n    where: URL path segment {token}\n    prefix: null\n    format: opaque\n    use: Read-only broker gateway for assistants that cannot POST\n    issued_by: Operator, out of band (POST /engage/issue is admin-gated)\noauth: null\nscopes: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capepartners-fr/refs/heads/main/authentication/capepartners-fr-authentication.yml
summary_line: apiKey · 6 schemes
tags:
- Mergers and Acquisitions
- Deal Flow
- Valuation
- Investment
- Financial Services
- Agents
- A2A
- France
- Technology
- Software-as-a-Service
---
