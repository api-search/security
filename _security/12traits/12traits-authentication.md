---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 12Traits Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solsten declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Solsten
provider_slug: 12traits
scheme_count: 2
schemes:
- applies_to: all documented /v1 operations
  description: 'Per-dashboard API key. Quoting the reference: "The Solsten API uses API Keys to authenticate requests. You can view and manage your API Keys in the Solsten Dashboard. Each dashboard has its own API Key."'
  evidence: https://docs.api.solsten.io/#authentication
  format: 'Authorization: Bearer {API_KEY}'
  id: bearer_api_key
  in: header
  name: Authorization
  scheme: bearer
  type: http
- applies_to: POST /v1/playfab
  concerns:
  - A credential in a URL query string is logged by intermediaries and stored in webhook configuration UIs. This is a documented provider design, not an inference.
  description: The PlayFab webhook ingestion endpoint takes the same API key as a query-string parameter rather than a header, because PlayFab's webhook configuration only allows a URL to be set.
  evidence: https://docs.api.solsten.io/#microsoft-azure-playfab
  format: https://api.solsten.io/v1/playfab?api_key={SOLSTEN_API_KEY}
  id: query_api_key
  in: query
  name: api_key
  type: apiKey
slug: 12traits-authentication
source_filename: 12traits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.api.solsten.io/#authentication\ndocs: https://docs.api.solsten.io/#authentication\nname: Solsten API authentication\nsummary: >-\n  A single authentication model: a per-dashboard API Key presented as an HTTP Bearer token.\n  There is no OAuth, no OpenID Connect, no mTLS and no scope system. The API key is issued and\n  rotated from the Solsten Dashboard, and Solsten states that each dashboard has its own key,\n  which makes the key the tenant boundary as well as the credential.\napi: Solsten API\nbase_url: https://api.solsten.io/v1\nschemes:\n- id: bearer_api_key\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  format: 'Authorization: Bearer {API_KEY}'\n  description: >-\n    Per-dashboard API key. Quoting the reference: \"The Solsten API uses API Keys to authenticate\n    requests. You can view and manage your API Keys in the Solsten Dashboard. Each dashboard has\n    its own API Key.\"\n\
  \  applies_to: all documented /v1 operations\n  evidence: https://docs.api.solsten.io/#authentication\n- id: query_api_key\n  type: apiKey\n  in: query\n  name: api_key\n  format: https://api.solsten.io/v1/playfab?api_key={SOLSTEN_API_KEY}\n  description: >-\n    The PlayFab webhook ingestion endpoint takes the same API key as a query-string parameter\n    rather than a header, because PlayFab's webhook configuration only allows a URL to be set.\n  applies_to: POST /v1/playfab\n  evidence: https://docs.api.solsten.io/#microsoft-azure-playfab\n  concerns:\n  - >-\n    A credential in a URL query string is logged by intermediaries and stored in webhook\n    configuration UIs. This is a documented provider design, not an inference.\nkey_management:\n  issuance: Solsten Dashboard (https://dashboard.solsten.io/)\n  self_serve: unknown\n  scoped: false\n  rotation_documented: false\n  key_prefix_documented: false\n  per_tenant: true\ntransport:\n  https_required: true\n  evidence_quote: >-\n\
  \    \"All API requests must be made over HTTPS. Calls made over plain HTTP will fail. API requests\n    without authentication will also fail.\"\n  evidence: https://docs.api.solsten.io/#authentication\nobserved:\n- url: https://api.solsten.io/v1/openapi.json\n  status: 401\n  body: '{\"code\":401,\"message\":\"api key is not valid\"}'\n  note: >-\n    An unauthenticated request to a /v1 path returns a JSON 401 with the documented error envelope,\n    confirming the auth requirement is enforced at the edge and matching the published error shape.\ngaps:\n- No documented key rotation or expiry policy.\n- No scopes, roles or least-privilege model — one key grants the whole documented surface for a dashboard.\n- No OAuth or OIDC surface exists, so scopes/ is not applicable for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/12traits/refs/heads/main/authentication/12traits-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Audience Intelligence
- Psychographics
- Consumer Insights
- Analytics
- Artificial Intelligence
- Gaming
- Market Research
- Personalization
- Behavioral Data
---
