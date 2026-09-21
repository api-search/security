---
anonymous_access: true
api_key_in: []
auth_types:
- none
- http
description: Authentication profile for A2APark's two published surfaces. There is no OpenAPI, so this is read from the agent card (which declares no security) and the A2AParkBench README (which documents the feed token flow), and confirmed by live probes on 2026-09-19.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: A2Apark Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: A2APark secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: A2APark
provider_slug: a2apark-com
scheme_count: 2
schemes:
- description: The agent card declares security [] and securitySchemes {} and supportsAuthenticatedExtendedCard false. A message/send with no credentials returned a completed Task. Anyone can start a ride; the agentName passed to start_ride only labels the scorecard. The Park therefore has no identity for the calling agent and the site warns "Do not enter secrets or personal data."
  name: anonymous
  probe:
    credentials: none
    method: POST message/send
    status: 200
    url: https://a2apark.com/a2a
  sources:
  - https://a2apark.com/.well-known/agent-card.json
  surface: A2A endpoint https://a2apark.com/a2a
  type: none
- description: A per-repository compound token obtained once by POSTing {license_key, instance_name} to /api/license/activate (license_key is the Lemon Squeezy key from the purchase receipt; instance_name is owner/repository). One Team licence activates up to five repositories. The token is sent as a Bearer credential on GET /api/feed/manifest and is stored as the A2APARKBENCH_TOKEN GitHub Actions secret (MUTANT_WEB_TOKEN remains a compatibility alias). The feed validates the exact licence instance and product on every access; subscription expiry stops future pack downloads without invalidating a cached pack.
  name: feedToken
  probes:
  - body: '{"error":"Bearer feed token is required"}'
    method: GET
    status: 401
    url: https://bench.a2apark.com/api/feed/manifest
  - body: '{"error":"license_key and instance_name are required"}'
    method: POST (empty body)
    status: 422
    url: https://bench.a2apark.com/api/license/activate
  scheme: bearer
  sources:
  - https://github.com/MutantWeb/ci#packs
  - https://bench.a2apark.com/activate
  surface: A2AParkBench feed API https://bench.a2apark.com/api
  type: http
slug: a2apark-com-authentication
source_filename: a2apark-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource:\n- https://a2apark.com/.well-known/agent-card.json\n- https://github.com/MutantWeb/ci#packs\n- https://bench.a2apark.com/activate\ndocs: https://github.com/MutantWeb/ci#packs\ndescription: >-\n  Authentication profile for A2APark's two published surfaces. There is no OpenAPI, so this is read from\n  the agent card (which declares no security) and the A2AParkBench README (which documents the feed\n  token flow), and confirmed by live probes on 2026-09-19.\nsummary:\n  types: [none, http]\nschemes:\n- name: anonymous\n  type: none\n  surface: A2A endpoint https://a2apark.com/a2a\n  description: >-\n    The agent card declares security [] and securitySchemes {} and supportsAuthenticatedExtendedCard false.\n    A message/send with no credentials returned a completed Task. Anyone can start a ride; the agentName\n    passed to start_ride only labels the scorecard. The Park therefore has no identity for the calling\n    agent and\
  \ the site warns \"Do not enter secrets or personal data.\"\n  sources: [https://a2apark.com/.well-known/agent-card.json]\n  probe: {url: 'https://a2apark.com/a2a', method: POST message/send, status: 200, credentials: none}\n- name: feedToken\n  type: http\n  scheme: bearer\n  surface: A2AParkBench feed API https://bench.a2apark.com/api\n  description: >-\n    A per-repository compound token obtained once by POSTing {license_key, instance_name} to\n    /api/license/activate (license_key is the Lemon Squeezy key from the purchase receipt; instance_name\n    is owner/repository). One Team licence activates up to five repositories. The token is sent as a Bearer\n    credential on GET /api/feed/manifest and is stored as the A2APARKBENCH_TOKEN GitHub Actions secret\n    (MUTANT_WEB_TOKEN remains a compatibility alias). The feed validates the exact licence instance and\n    product on every access; subscription expiry stops future pack downloads without invalidating a cached\n    pack.\n  sources:\
  \ [https://github.com/MutantWeb/ci#packs, https://bench.a2apark.com/activate]\n  probes:\n  - {url: 'https://bench.a2apark.com/api/feed/manifest', method: GET, status: 401, body: '{\"error\":\"Bearer feed token is required\"}'}\n  - {url: 'https://bench.a2apark.com/api/license/activate', method: POST (empty body), status: 422, body: '{\"error\":\"license_key and instance_name are required\"}'}\noauth: false\nopenid_connect: false\napi_keys: false\nnotes: >-\n  No OAuth 2.0, OIDC or API-key scheme anywhere; /.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all 404 on both hosts. No\n  scopes/ artifact is written because there is no scope surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a2apark-com/refs/heads/main/authentication/a2apark-com-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Agent Evaluation
- AI Agents
- A2A
- Agent Safety
- Benchmarking
- Browser Agents
- Testing
- CI/CD
- Simulation
---
