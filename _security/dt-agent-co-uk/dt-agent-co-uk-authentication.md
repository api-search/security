---
anonymous_access: true
api_key_in: []
auth_types:
- none
description: Authentication profile for Neva's one published surface, the A2A JSON-RPC endpoint at the root of neva.dt-agent.co.uk. There is no OpenAPI and no documentation, so this is read from the agent card (which declares no security at all) and confirmed by live anonymous probes on 2026-09-19.
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Dt Agent Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neva secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Neva
provider_slug: dt-agent-co-uk
scheme_count: 1
schemes:
- description: 'The card carries no security, securitySchemes or supportsAuthenticatedExtendedCard key, and the server accepts unauthenticated JSON-RPC: tasks/get answered -32001 Task not found and a malformed message/send answered -32602 with Pydantic field detail, both without any credential. A well-formed message/send then fails with -32603 wrapping an upstream 401 "API key is invalid" - that is the agent''s own credential to its model provider, not a requirement on the caller; no header, token or key is asked of the client at any point. agent/getAuthenticatedExtendedCard returns -32603 "Authenticated card not supported".'
  name: anonymous
  probes:
  - body: '{"error":{"code":-32001,"message":"Task not found"}}'
    credentials: none
    method: POST tasks/get
    status: 200
    url: https://neva.dt-agent.co.uk/
  - body: -32602 Invalid parameters, data[0].loc [params, message, messageId]
    credentials: none
    method: POST message/send (no messageId)
    status: 200
    url: https://neva.dt-agent.co.uk/
  - body: '-32603 Error code: 401 ... authentication_error ... API key is invalid. (upstream, not caller)'
    credentials: none
    method: POST message/send (well-formed)
    status: 200
    url: https://neva.dt-agent.co.uk/
  sources:
  - https://neva.dt-agent.co.uk/.well-known/agent-card.json
  surface: A2A endpoint https://neva.dt-agent.co.uk/
  type: none
slug: dt-agent-co-uk-authentication
source_filename: dt-agent-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource:\n- https://neva.dt-agent.co.uk/.well-known/agent-card.json\n- https://neva.dt-agent.co.uk/\ndocs: null\ndescription: >-\n  Authentication profile for Neva's one published surface, the A2A JSON-RPC endpoint at the root of\n  neva.dt-agent.co.uk. There is no OpenAPI and no documentation, so this is read from the agent card (which\n  declares no security at all) and confirmed by live anonymous probes on 2026-09-19.\nsummary:\n  types: [none]\nschemes:\n- name: anonymous\n  type: none\n  surface: A2A endpoint https://neva.dt-agent.co.uk/\n  description: >-\n    The card carries no security, securitySchemes or supportsAuthenticatedExtendedCard key, and the server\n    accepts unauthenticated JSON-RPC: tasks/get answered -32001 Task not found and a malformed message/send\n    answered -32602 with Pydantic field detail, both without any credential. A well-formed message/send\n    then fails with -32603 wrapping an upstream 401 \"API\
  \ key is invalid\" - that is the agent's own credential\n    to its model provider, not a requirement on the caller; no header, token or key is asked of the client\n    at any point. agent/getAuthenticatedExtendedCard returns -32603 \"Authenticated card not supported\".\n  sources: [https://neva.dt-agent.co.uk/.well-known/agent-card.json]\n  probes:\n  - {url: 'https://neva.dt-agent.co.uk/', method: POST tasks/get, status: 200, credentials: none, body: '{\"error\":{\"code\":-32001,\"message\":\"Task not found\"}}'}\n  - {url: 'https://neva.dt-agent.co.uk/', method: POST message/send (no messageId), status: 200, credentials: none, body: '-32602 Invalid parameters, data[0].loc [params, message, messageId]'}\n  - {url: 'https://neva.dt-agent.co.uk/', method: POST message/send (well-formed), status: 200, credentials: none, body: '-32603 Error code: 401 ... authentication_error ... API key is invalid. (upstream, not caller)'}\noauth: false\nopenid_connect: false\napi_keys: false\nnotes: >-\n\
  \  No OAuth 2.0, OIDC or API-key scheme anywhere; /.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all 404 on neva.dt-agent.co.uk\n  and dt-agent.co.uk (well-known/dt-agent-co-uk-well-known.yml). No scopes/ artifact is written because there\n  is no scope surface. The derive-authentication.py baseline was not run because there is no OpenAPI for it\n  to read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dt-agent-co-uk/refs/heads/main/authentication/dt-agent-co-uk-authentication.yml
summary_line: none · 1 scheme
tags:
- A2A
- AI Agents
- Agent Services
- Software Development
- JSON-RPC
- Prototyping
- Integration
- Collaboration
---
