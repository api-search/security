---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Elderlycarematch Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elderly Care Match declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Elderly Care Match
provider_slug: elderlycarematch-com
scheme_count: 0
schemes: []
slug: elderlycarematch-com-authentication
source_filename: elderlycarematch-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://www.elderlycarematch.com/.well-known/agent-card.json\ndocs:\n- https://www.elderlycarematch.com/llms.txt\n- https://www.elderlycarematch.com/a2a/v1\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  headline: >-\n    No authentication of any kind. The A2A agent card declares no securitySchemes and no security\n    requirement, the GET descriptor at /a2a/v1 names none, the site's llms.txt says \"no authentication\n    required\" in as many words, and an anonymous SendMessage returned real search results. There is no\n    signup, no key, no token, and no OAuth/OIDC discovery document on the host (openid-configuration,\n    oauth-authorization-server and oauth-protected-resource all 404). The surface is read-only public\n    directory data, and the one skill that touches a family (request-placement-help) returns a URL for the\n    family to fill in themselves rather\
  \ than accepting anything.\nschemes: []\ndeclared_in_card:\n  securitySchemes: absent\n  security: absent\nobserved:\n- url: https://www.elderlycarematch.com/a2a/v1\n  method: POST\n  credential_sent: none\n  http_status: 200\n  result: JSON-RPC result with a completed Task and one artifact (five facility listings)\n  fetched: '2026-09-19'\n- url: https://www.elderlycarematch.com/.well-known/oauth-authorization-server\n  http_status: 404\n- url: https://www.elderlycarematch.com/.well-known/oauth-protected-resource\n  http_status: 404\n- url: https://www.elderlycarematch.com/.well-known/openid-configuration\n  http_status: 404\nnote: >-\n  The human site has accounts (family, care provider, licensed agent, administrator roles per the privacy\n  policy) behind server-side auth on /business/, /agent/, /dashboard/ and the other robots-disallowed\n  prefixes, and the internal /api/ router serving them is disallowed to every crawler. None of that is a\n  public API surface and none of it was\
  \ probed. This profile records only the public agent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elderlycarematch-com/refs/heads/main/authentication/elderlycarematch-com-authentication.yml
summary_line: 0 schemes
tags:
- Senior Care
- Elder Care
- Assisted Living
- Memory Care
- Adult Family Homes
- Nursing Homes
- Care Directory
- Healthcare
- Agents
- A2A
- Agent-Native
- Washington State
- United States
---
