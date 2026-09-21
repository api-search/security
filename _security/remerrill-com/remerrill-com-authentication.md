---
anonymous_access: false
api_key_in: []
api_specs:
- filename: remerrill-com-openapi.yml
  format: yaml
  label: R.E. Merrill Pump Line Finder API
  slug: pump-line-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remerrill-com/refs/heads/main/openapi/remerrill-com-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Remerrill Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: R.E. Merrill & Associates, Inc. declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: R.E. Merrill & Associates, Inc.
provider_slug: remerrill-com
scheme_count: 0
schemes: []
slug: remerrill-com-authentication
source_filename: remerrill-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live calls to POST https://www.remerrill.com/api/line-finder and POST https://www.remerrill.com/api/a2a, 2026-09-19\nderived_from: openapi/remerrill-com-openapi.yml\ndocs:\n- https://www.remerrill.com/llms.txt\n- https://www.remerrill.com/.well-known/agent-card.json\nsummary: >-\n  No authentication on any surface. The provider's documented curl examples send no credential and both\n  endpoints answered them anonymously with 200; the agent card declares no securitySchemes or security\n  requirements; no OAuth/OIDC discovery document is served (/.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all 404). derive-authentication.py\n  found zero securitySchemes in the OpenAPI and wrote nothing, which is correct — this file records the\n  absence so an agent knows it needs no key.\nschemes: []\nsecurity_schemes_count: 0\napplies_to:\n  findPumpLines: none\n  sendA2AMessage:\
  \ none\nsigning:\n  note: >-\n    The one cryptographic control is on the PROVIDER's side, not the caller's: the agent card is JWS-signed\n    (ES256, kid remerrill-a2a-2026-08) with the public key set at https://www.remerrill.com/.well-known/jwks.json,\n    so a client can verify the card's origin. Nothing signs requests.\ntransport:\n  https: true\n  hsts: 'max-age=63072000 on every response'\n  http_redirect: 'http://remerrill.com and the apex 308 to https://www.remerrill.com'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remerrill-com/refs/heads/main/authentication/remerrill-com-authentication.yml
summary_line: 0 schemes
tags:
- Industrial Pumps
- Pump Selection
- Industrial Equipment
- Chemical Processing
- Manufacturing
- Distribution
- Agents
- A2A
- agent-native
- Texas
- United States
---
