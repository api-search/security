---
anonymous_access: true
api_key_in: []
api_specs:
- filename: finn-tannlege-com-openapi.yml
  format: yaml
  label: Finn-tannlege REST API
  slug: finn-tannlege-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finn-tannlege-com/refs/heads/main/openapi/finn-tannlege-com-openapi.yml
auth_types:
- none
- apiKey
description: 'Authentication profile for every finn-tannlege.com surface. The OpenAPI declares no securitySchemes and its info.description states "All read endpoints are public; no authentication required" (derive-authentication.py therefore produced nothing, and this file is written from the provider''s documents instead). The agent card and the MCP server card both declare schemes ["none"]. The one credential that exists is an optional, free consumer identity key documented in llms.txt; it grants no access and raises no limit. Confirmed live on 2026-09-19: anonymous calls to REST, A2A message/send and the MCP handshake all succeeded.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Finn Tannlege Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finn-tannlege secures its APIs with none and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finn-tannlege
provider_slug: finn-tannlege-com
scheme_count: 2
schemes:
- description: Every published operation is callable without credentials. The only per-client control is a flat per-IP rate limit (rate-limits/finn-tannlege-com-rate-limits.yml).
  name: anonymous
  probes:
  - credentials: none
    method: GET
    status: 200
    url: https://finn-tannlege.com/api/tannlege/agents?limit=1
  - credentials: none
    method: POST message/send
    status: 200
    url: https://finn-tannlege.com/a2a
  - credentials: none
    method: POST initialize + tools/list
    status: 200
    url: https://finn-tannlege.com/mcp
  sources:
  - https://finn-tannlege.com/openapi.json
  - https://finn-tannlege.com/.well-known/agent-card.json
  - https://finn-tannlege.com/.well-known/mcp/server-card.json
  surface: REST https://finn-tannlege.com/api/tannlege, A2A https://finn-tannlege.com/a2a, MCP https://finn-tannlege.com/mcp
  type: none
- description: '"Frivillig og helt gratis identitetsnøkkel for AI-agenter" - a voluntary, free identity key. Minted by POST https://finn-tannlege.com/api/keys with an optional JSON body {label, contact_email}; no login or account; the key is returned once and cannot be retrieved again. Sending it as X-API-Key records the call in an aggregated usage ledger (endpoint or tool name and date only - never content or arguments). On this vertical the rate limit is a flat per-IP quota that the key does NOT raise; the provider notes that the higher keyed limit available on some sister verticals is not connected here. The agent card''s securitySchemes declares this scheme as consumerApiKey and adds that the same header name denotes a separate producer/write key elsewhere on the platform, but finn-tannlege.com has no write API so here it means only the consumer key. No security requirement in the card or the OpenAPI references it.'
  erase:
    body: '{"key": "..."} or the key as X-API-Key'
    effect: GDPR erasure of label and e-mail
    method: POST
    url: https://finn-tannlege.com/api/keys/erase
  header: X-API-Key
  in: header
  name: consumerApiKey
  obtain:
    body: '{"label": "my-agent", "contact_email": "..."} (both optional)'
    method: POST
    url: https://finn-tannlege.com/api/keys
  probe_note: Not exercised - minting a key creates a record on the provider's side, and an OPTIONS on /api/keys (204) was the only request made. GET /api/keys returns the site's 404, consistent with a POST-only route.
  required: false
  revoke:
    body: '{"key": "..."} or the key as X-API-Key'
    effect: stops the key; history retained
    method: POST
    url: https://finn-tannlege.com/api/keys/revoke
  sources:
  - https://finn-tannlege.com/llms.txt
  - https://finn-tannlege.com/.well-known/agent-card.json
  surface: any REST, A2A or MCP call
  type: apiKey
slug: finn-tannlege-com-authentication
source_filename: finn-tannlege-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource:\n- https://finn-tannlege.com/llms.txt\n- https://finn-tannlege.com/.well-known/agent-card.json\n- https://finn-tannlege.com/.well-known/mcp/server-card.json\n- https://finn-tannlege.com/openapi.json\ndocs: https://finn-tannlege.com/llms.txt\ndescription: >-\n  Authentication profile for every finn-tannlege.com surface. The OpenAPI declares no securitySchemes and\n  its info.description states \"All read endpoints are public; no authentication required\"\n  (derive-authentication.py therefore produced nothing, and this file is written from the provider's\n  documents instead). The agent card and the MCP server card both declare schemes [\"none\"]. The one\n  credential that exists is an optional, free consumer identity key documented in llms.txt; it grants no\n  access and raises no limit. Confirmed live on 2026-09-19: anonymous calls to REST, A2A message/send and\n  the MCP handshake all succeeded.\nsummary:\n  types: [none,\
  \ apiKey]\n  required: false\nschemes:\n- name: anonymous\n  type: none\n  surface: REST https://finn-tannlege.com/api/tannlege, A2A https://finn-tannlege.com/a2a, MCP https://finn-tannlege.com/mcp\n  description: >-\n    Every published operation is callable without credentials. The only per-client control is a flat\n    per-IP rate limit (rate-limits/finn-tannlege-com-rate-limits.yml).\n  sources: [https://finn-tannlege.com/openapi.json, https://finn-tannlege.com/.well-known/agent-card.json, https://finn-tannlege.com/.well-known/mcp/server-card.json]\n  probes:\n  - {url: 'https://finn-tannlege.com/api/tannlege/agents?limit=1', method: GET, status: 200, credentials: none}\n  - {url: 'https://finn-tannlege.com/a2a', method: POST message/send, status: 200, credentials: none}\n  - {url: 'https://finn-tannlege.com/mcp', method: POST initialize + tools/list, status: 200, credentials: none}\n- name: consumerApiKey\n  type: apiKey\n  in: header\n  header: X-API-Key\n  required: false\n  surface:\
  \ any REST, A2A or MCP call\n  description: >-\n    \"Frivillig og helt gratis identitetsnøkkel for AI-agenter\" - a voluntary, free identity key. Minted\n    by POST https://finn-tannlege.com/api/keys with an optional JSON body {label, contact_email}; no\n    login or account; the key is returned once and cannot be retrieved again. Sending it as X-API-Key\n    records the call in an aggregated usage ledger (endpoint or tool name and date only - never content or\n    arguments). On this vertical the rate limit is a flat per-IP quota that the key does NOT raise; the\n    provider notes that the higher keyed limit available on some sister verticals is not connected here.\n    The agent card's securitySchemes declares this scheme as consumerApiKey and adds that the same header\n    name denotes a separate producer/write key elsewhere on the platform, but finn-tannlege.com has no\n    write API so here it means only the consumer key. No security requirement in the card or the OpenAPI\n   \
  \ references it.\n  obtain: {method: POST, url: 'https://finn-tannlege.com/api/keys', body: '{\"label\": \"my-agent\", \"contact_email\": \"...\"} (both optional)'}\n  revoke: {method: POST, url: 'https://finn-tannlege.com/api/keys/revoke', body: '{\"key\": \"...\"} or the key as X-API-Key', effect: stops the key; history retained}\n  erase: {method: POST, url: 'https://finn-tannlege.com/api/keys/erase', body: '{\"key\": \"...\"} or the key as X-API-Key', effect: GDPR erasure of label and e-mail}\n  sources: [https://finn-tannlege.com/llms.txt, https://finn-tannlege.com/.well-known/agent-card.json]\n  probe_note: >-\n    Not exercised - minting a key creates a record on the provider's side, and an OPTIONS on /api/keys\n    (204) was the only request made. GET /api/keys returns the site's 404, consistent with a POST-only route.\noauth: false\nopenid_connect: false\napi_keys: true\napi_keys_required: false\nnotes: >-\n  No OAuth 2.0 or OIDC: /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n\
  \  (apex and under /mcp/) and /.well-known/openid-configuration all 404 (well-known/finn-tannlege-com-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finn-tannlege-com/refs/heads/main/authentication/finn-tannlege-com-authentication.yml
summary_line: none/apiKey · 2 schemes
tags:
- Dental
- Healthcare
- Directory
- Norway
- Search
- Open Data
- A2A
- MCP
- AI Agents
- Clinics
---
