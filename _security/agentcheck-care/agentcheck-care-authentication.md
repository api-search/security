---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentcheck-care-openapi.yml
  format: yaml
  label: AgentCheck Checkup API
  slug: agentcheck-checkup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentcheck-care/refs/heads/main/openapi/agentcheck-care-openapi.yml
auth_types:
- apiKey
- token-in-path
- token-in-query
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: probed
name: Agentcheck Care Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentCheck secures its APIs with apiKey, token-in-path, and token-in-query across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AgentCheck
provider_slug: agentcheck-care
scheme_count: 5
schemes:
- applies_to:
  - GET /api/credits/balance (credit_balance_api_credits_balance_get)
  evidence: Anonymous GET https://agentcheck.care/api/credits/balance returned HTTP 401, application/json, {"detail":"Missing X-API-Key header"} on 2026-09-19.
  header: X-API-Key
  in: header
  issuance: undocumented — no page describes how to obtain an API key or what credits are
  name: X-API-Key
  sources:
  - https://agentcheck.care/api/credits/balance
  type: apiKey
- applies_to:
  - GET /api/stats/internal (get_internal_stats_api_stats_internal_get)
  evidence: The operation description says "Requires ADMIN_STATS_TOKEN"; anonymous GET returned HTTP 401 {"error":"Unauthorized"} (a different envelope from the X-API-Key 401). Operator-only; not a developer credential.
  in: unknown
  name: ADMIN_STATS_TOKEN
  sources:
  - openapi/_original/agentcheck-care-openapi.json
  type: apiKey
- applies_to:
  - GET /exam/{token}
  - GET /exam/{token}/status
  - POST /exam/{token}/relaunch
  - POST /exam/{token}/v1/chat/completions
  evidence: The "exam" mode generates a per-checkup secure URL that the customer pastes into their bot as an OpenAI-compatible endpoint (home page step 1; the chat_completions operation description). The token in the path IS the credential. Anonymous GET /exam/nonexistent/status returned 404 {"detail":"Exam session not found"}.
  in: path
  name: exam-session-token
  parameter: token
  sources:
  - https://agentcheck.care/
  - openapi/_original/agentcheck-care-openapi.json
  type: token-in-path
- applies_to:
  - GET /report/{checkup_id} (magic_link_report_report__checkup_id__get)
  evidence: '"Serve a persisted report via magic link token + optional access code." The privacy policy (3.1) says reports are reachable only via a unique magic link carrying a cryptographic token and tells users to treat the link like a password. Anonymous GET /report/nonexistent returned 404 {"detail":"Report not found"}.'
  in: query
  name: report-magic-link
  parameters:
  - token
  - code
  sources:
  - https://agentcheck.care/privacy
  - openapi/_original/agentcheck-care-openapi.json
  type: token-in-query
- applies_to:
  - POST /api/stripe-webhook (stripe_webhook_api_stripe_webhook_post)
  name: stripe-webhook
  note: Receiver for Stripe payment events. Signature verification is not described anywhere public and is not asserted here; the endpoint is Stripe-facing, not developer-facing.
  type: inbound-webhook
slug: agentcheck-care-authentication
source_filename: agentcheck-care-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live anonymous probes of https://agentcheck.care on 2026-09-19, read against openapi/_original/agentcheck-care-openapi.json\ndocs: https://agentcheck.care/docs\nspec: openapi/agentcheck-care-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - token-in-path\n  - token-in-query\n  transport: HTTPS only; Cloudflare in front of a FastAPI origin\n  note: >-\n    The served OpenAPI declares NO securitySchemes and NO security requirements on any of its 35\n    operations, so derive-authentication.py produced nothing. The authentication model below is what the\n    live API told an anonymous caller plus what the operation descriptions say. Most of the surface —\n    tiers, free-scan pool, public stats, validate-bot, start-checkup (free), create-checkout, the A2A\n    endpoint and the agent card — is deliberately anonymous: the product has no login and no account.\n    Three credential-shaped mechanisms exist and none is documented on a\
  \ page a developer can find.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  header: X-API-Key\n  applies_to:\n  - GET /api/credits/balance (credit_balance_api_credits_balance_get)\n  evidence: >-\n    Anonymous GET https://agentcheck.care/api/credits/balance returned HTTP 401, application/json,\n    {\"detail\":\"Missing X-API-Key header\"} on 2026-09-19.\n  issuance: undocumented — no page describes how to obtain an API key or what credits are\n  sources:\n  - https://agentcheck.care/api/credits/balance\n- name: ADMIN_STATS_TOKEN\n  type: apiKey\n  in: unknown\n  applies_to:\n  - GET /api/stats/internal (get_internal_stats_api_stats_internal_get)\n  evidence: >-\n    The operation description says \"Requires ADMIN_STATS_TOKEN\"; anonymous GET returned HTTP 401\n    {\"error\":\"Unauthorized\"} (a different envelope from the X-API-Key 401). Operator-only; not a\n    developer credential.\n  sources:\n  - openapi/_original/agentcheck-care-openapi.json\n- name: exam-session-token\n\
  \  type: token-in-path\n  in: path\n  parameter: token\n  applies_to:\n  - GET /exam/{token}\n  - GET /exam/{token}/status\n  - POST /exam/{token}/relaunch\n  - POST /exam/{token}/v1/chat/completions\n  evidence: >-\n    The \"exam\" mode generates a per-checkup secure URL that the customer pastes into their bot as an\n    OpenAI-compatible endpoint (home page step 1; the chat_completions operation description). The\n    token in the path IS the credential. Anonymous GET /exam/nonexistent/status returned 404\n    {\"detail\":\"Exam session not found\"}.\n  sources:\n  - https://agentcheck.care/\n  - openapi/_original/agentcheck-care-openapi.json\n- name: report-magic-link\n  type: token-in-query\n  in: query\n  parameters:\n  - token\n  - code\n  applies_to:\n  - GET /report/{checkup_id} (magic_link_report_report__checkup_id__get)\n  evidence: >-\n    \"Serve a persisted report via magic link token + optional access code.\" The privacy policy (3.1)\n    says reports are reachable only\
  \ via a unique magic link carrying a cryptographic token and tells\n    users to treat the link like a password. Anonymous GET /report/nonexistent returned 404\n    {\"detail\":\"Report not found\"}.\n  sources:\n  - https://agentcheck.care/privacy\n  - openapi/_original/agentcheck-care-openapi.json\n- name: stripe-webhook\n  type: inbound-webhook\n  applies_to:\n  - POST /api/stripe-webhook (stripe_webhook_api_stripe_webhook_post)\n  note: >-\n    Receiver for Stripe payment events. Signature verification is not described anywhere public and is\n    not asserted here; the endpoint is Stripe-facing, not developer-facing.\nanonymous_surface:\n  operations:\n  - get_tiers_api_tiers_get\n  - free_scans_endpoint_api_free_scans_get\n  - free_scan_status_api_free_scan_status_get\n  - get_public_stats_api_stats_public_get\n  - health_api_health_get\n  - validate_bot_api_validate_bot_post\n  - start_checkup_api_checkup_post\n  - create_checkout_api_checkout_post\n  - upgrade_checkout_api_checkout_get\n\
  \  - a2a_endpoint_a2a_post\n  - agent_card__well_known_agent_card_json_get\n  note: Every one of these answered an anonymous request without a challenge (200, 302 or a 404 on an unknown id). The A2A card declares no securitySchemes, consistent with the open endpoint.\ncustomer_credentials_in_requests:\n  note: >-\n    CheckupRequest and CheckoutRequest carry an optional `api_key` field — the CUSTOMER's key for their\n    own bot's chat API, which AgentCheck uses to call the bot under test. The privacy policy (1.3) states\n    it is held in memory for the session only and never written to disk. This is a credential the caller\n    sends, not one AgentCheck issues.\ngaps:\n- No securitySchemes in the OpenAPI; a generated client will treat /api/credits/balance as anonymous and get a 401.\n- No developer page documents the X-API-Key credential or how to obtain one.\n- No OAuth, no OIDC, no RFC 9728 protected-resource metadata (all /.well-known OAuth paths 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentcheck-care/refs/heads/main/authentication/agentcheck-care-authentication.yml
summary_line: apiKey/token-in-path/token-in-query · 5 schemes
tags:
- AI Agents
- AI Safety
- Security Testing
- Prompt Injection
- LLM Evaluation
- A2A
- agent-native
- Chatbots
- Compliance
- Developer Tools
---
