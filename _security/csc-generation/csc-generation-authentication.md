---
api_key_in:
- unpublished — rejected before the scheme is disclosed
auth_types:
- apiKey
- agent-profile-handshake
description: ''
kind: authentication
layout: security
method: probed
name: Csc Generation Authentication
name_suffix: Authentication
oauth_flows: []
overview: CSC Generation secures its APIs with apiKey and agent-profile-handshake across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CSC Generation
provider_slug: csc-generation
scheme_count: 2
schemes:
- brand: Backcountry
  endpoint: https://api.firmly.online/api/2026-01-23/ucp/mcp/domain/backcountry.com
  enrollment: not publicly documented; no self-service sign-up surface found
  name: firmly-merchant-api-key
  observed:
    code: api_key_required
    http_status: 401
    message: API key is required for this merchant and destination
    severity: recoverable
  type: apiKey
- brand: Seattle Coffee Gear
  endpoint: https://www.seattlecoffeegear.com/api/ucp/mcp
  http_header: UCP-Agent
  name: ucp-agent-profile
  note: The store authenticates the calling AGENT PLATFORM by dereferencing its published profile document rather than by a bearer credential; payment authorization is separate and requires contemporaneous human approval.
  observed:
    code: invalid_profile_url
    http_status: 422
    message: 'Unable to fetch agent profile: Missing profile uri'
  parameter: meta.ucp-agent.profile
  type: handshake
  value: URL to the calling agent platform's own UCP profile document
slug: csc-generation-authentication
source_filename: csc-generation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: >-\n  live probes of the two UCP endpoints declared by CSC Generation brand merchant\n  profiles, plus https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json\nnote: >-\n  Derived mechanically from OpenAPI securitySchemes was not possible — CSC Generation\n  publishes no OpenAPI. This profile records what the live endpoints actually\n  enforced when probed anonymously on 2026-08-01.\nsummary:\n  types: [apiKey, agent-profile-handshake]\n  api_key_in: [unpublished — rejected before the scheme is disclosed]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: firmly-merchant-api-key\n    type: apiKey\n    brand: Backcountry\n    endpoint: https://api.firmly.online/api/2026-01-23/ucp/mcp/domain/backcountry.com\n    observed:\n      http_status: 401\n      code: api_key_required\n      message: API key is required for this merchant and destination\n      severity: recoverable\n    enrollment:\
  \ not publicly documented; no self-service sign-up surface found\n  - name: ucp-agent-profile\n    type: handshake\n    brand: Seattle Coffee Gear\n    endpoint: https://www.seattlecoffeegear.com/api/ucp/mcp\n    parameter: meta.ucp-agent.profile\n    http_header: UCP-Agent\n    value: URL to the calling agent platform's own UCP profile document\n    observed:\n      http_status: 422\n      code: invalid_profile_url\n      message: 'Unable to fetch agent profile: Missing profile uri'\n    note: >-\n      The store authenticates the calling AGENT PLATFORM by dereferencing its\n      published profile document rather than by a bearer credential; payment\n      authorization is separate and requires contemporaneous human approval.\npayment_authorization:\n  - brand: Backcountry\n    handler: ai.firmly.card\n    version: '2026-04-08'\n    instruments: [card]\n    card_brands: [visa, mastercard, amex, discover]\n    encryption: RSA-OAEP-256\n    public_key_url: https://api.firmly.online/api/2026-01-23/ucp/rest/domain/backcountry.com/payment-handlers/ai.firmly.card/key\n\
  \  - brand: Seattle Coffee Gear\n    handlers_declared_in: well-known/csc-generation-seattle-coffee-gear-ucp.json\n    note: >-\n      includes com.google.pay among the declared payment handlers; Shop Pay via the\n      Shop skill is the store's recommended route for buy-for-me agents\ndocs:\n  - https://www.seattlecoffeegear.com/llms.txt\n  - https://www.seattlecoffeegear.com/agents.md\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n    - {url: 'https://api.firmly.online/api/2026-01-23/ucp/mcp/domain/backcountry.com', method: 'POST tools/list', http_status: 401}\n    - {url: 'https://www.seattlecoffeegear.com/api/ucp/mcp', method: 'POST tools/list', http_status: 422}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csc-generation/refs/heads/main/authentication/csc-generation-authentication.yml
summary_line: apiKey/agent-profile-handshake · 2 schemes
tags:
- Company
- Retail
- E-Commerce
- Agent Commerce
- Artificial Intelligence
- Universal Commerce Protocol
- Model Context Protocol
- Holding Company
- Shopping
---
