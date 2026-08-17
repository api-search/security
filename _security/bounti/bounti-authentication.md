---
api_key_in: []
api_specs:
- filename: bounti-llms-full-txt-api-openapi.yml
  format: yaml
  label: Bounti Llms Full.txt API
  slug: bounti-llms-full-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/openapi/bounti-llms-full-txt-api-openapi.yml
- filename: bounti-llms-txt-api-openapi.yml
  format: yaml
  label: Bounti Llms.txt API
  slug: bounti-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/openapi/bounti-llms-txt-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Bounti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bounti secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bounti
provider_slug: bounti
scheme_count: 1
schemes:
- applies_to: Bounti.ai Content API (GET /llms.txt, GET /llms-full.txt)
  evidence: 'The provider''s own AI-plugin manifest declares "auth": {"type": "none"}, the OpenAPI declares no securitySchemes and applies no security to either operation, and both endpoints return 200 to an anonymous GET. This is an intentional agent-facing content surface, not a missing auth model.'
  name: none
  sources:
  - openapi/_original/bounti-openapi.json
  - well-known/bounti-ai-plugin.json
  type: none
slug: bounti-authentication
source_filename: bounti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://bounti.ai/.well-known/ai-plugin.json (provider-declared), https://bounti.ai/.well-known/openapi.json,\n  and live unauthenticated probes of https://claw.bounti.ai/api on 2026-08-14\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    0-working/derive-authentication.py produced no profile for this provider because the published\n    OpenAPI declares no securitySchemes at all. That is not a harvesting gap — it is the correct\n    reading of the contract: Bounti's only public API is deliberately unauthenticated.\nschemes:\n- name: none\n  type: none\n  applies_to: Bounti.ai Content API (GET /llms.txt, GET /llms-full.txt)\n  sources: [openapi/_original/bounti-openapi.json, well-known/bounti-ai-plugin.json]\n  evidence: >-\n    The provider's own AI-plugin manifest declares \"auth\": {\"type\": \"none\"}, the OpenAPI declares no\n    securitySchemes and applies no security to either operation,\
  \ and both endpoints return 200 to an\n    anonymous GET. This is an intentional agent-facing content surface, not a missing auth model.\ngated_surfaces:\n- name: B.Claw product API\n  host: https://claw.bounti.ai\n  path: /api\n  http_status: 401\n  content_type: application/json\n  envelope: '{\"error\":\"unauthorized\",\"message\":\"Authentication required\"}'\n  scheme: undocumented\n  evidence: >-\n    Every path probed under /api (/api, /api/v1, /api/health, /api/docs, /api/openapi.json, /api/mcp,\n    /api/user, /api/me) returned the identical 401 JSON envelope on 2026-08-14. No WWW-Authenticate\n    header is returned, no auth documentation is published, and no OAuth or OIDC discovery document\n    exists on any Bounti host (/.well-known/openid-configuration, /oauth-authorization-server and\n    /oauth-protected-resource all 404 on bounti.ai and return only an SPA HTML shell on claw.bounti.ai).\n    The scheme is therefore recorded as undocumented rather than guessed.\n- name:\
  \ Real-estate product\n  host: https://re.bounti.ai\n  path: /real-estate/sign-in\n  scheme: interactive-login\n  evidence: Human sign-in page; no API surface found behind it.\nthird_party_authorization:\n  model: oauth-outbound\n  note: >-\n    B.Claw connects to the user's own third-party accounts (Gmail, Google Calendar, Follow Up Boss,\n    kvCORE, HubSpot, Salesforce, DocuSign and 30+ others catalogued at https://bounti.ai/integrations)\n    via OAuth authorized inside the product. This is Bounti acting as an OAuth CLIENT against other\n    providers — it is not an authorization surface Bounti exposes to callers, and it grants an agent\n    no way in.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/authentication/bounti-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Real Estate
- Artificial Intelligence
- Marketing
- Sales Enablement
- Virtual Staging
- Content Generation
- AI Agents
---
