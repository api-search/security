---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Agentbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentbox secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agentbox
provider_slug: agentbox
scheme_count: 3
schemes:
- description: The header the Tyk gateway recognises as the authorization field. An anonymous request to any path returns HTTP 401 {"error":"Authorization field missing"}; sending X-API-Key with any value advances the request past the gateway to the backend application, which then answers on its own (404 "URL not found" for an unknown path) and attaches x-ratelimit-* headers.
  evidence:
  - body: '{"error":"Authorization field missing"}'
    probe: GET https://api.agentboxcrm.com.au/listings?version=2 (anonymous)
    status: 401
  - note: passes the gateway; backend responds with x-ratelimit-limit / x-ratelimit-remaining / x-ratelimit-reset
    probe: 'GET https://api.agentboxcrm.com.au/listings?version=2 [X-API-Key: test]'
    status: 404
  in: header
  name: X-API-Key
  parameter_name: X-API-Key
  required: true
  type: apiKey
- description: Per-agency client identifier sent alongside X-API-Key. Alone it does not satisfy the gateway - a request carrying only X-Client-ID is still rejected 401 - so it is an application-level tenant identifier rather than the gateway credential.
  evidence:
  - probe: 'GET https://api.agentboxcrm.com.au/ [X-Client-ID: test]'
    status: 401
  - kind: third-party-client
    note: sends both X-Client-ID and X-API-Key on every request
    source: https://github.com/nad-au/agentbox
  - kind: third-party-client
    note: same header pair plus Content-Type/Accept application/json
    source: https://github.com/real-coder-pty-ltd/stafflink-gf-agentbox
  in: header
  name: X-Client-ID
  parameter_name: X-Client-ID
  required: true
  type: apiKey
- description: Issued with the API Key and Client ID, scoping the credential to one agency office's data. Not observed as a request header in the public third-party clients; it is part of the credential triple support issues per office.
  evidence:
  - kind: third-party-docs
    note: 'instructs the agency to email salessupportanz@reapit.com and request all three: API Key, Client ID and Office ID'
    source: https://auctionslive.com/knowledge-hub/obtaining-reapit-agentbox-api-credentials
  in: credential-issuance
  name: Office ID
  required: true
  type: tenant-identifier
slug: agentbox-authentication
source_filename: agentbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live probes of https://api.agentboxcrm.com.au plus published third-party\n  integration guides\ndocs: https://www.agentbox.com.au/integrator-application\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Agentbox publishes no OpenAPI, so this profile is not derived from a spec. It\n    is established by direct probe of the production gateway and corroborated by\n    multiple independent third-party integration guides that all describe the same\n    credential triple.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  required: true\n  description: >-\n    The header the Tyk gateway recognises as the authorization field. An anonymous\n    request to any path returns HTTP 401 {\"error\":\"Authorization field missing\"};\n    sending X-API-Key with any value advances the request past\
  \ the gateway to the\n    backend application, which then answers on its own (404 \"URL not found\" for an\n    unknown path) and attaches x-ratelimit-* headers.\n  evidence:\n  - probe: 'GET https://api.agentboxcrm.com.au/listings?version=2 (anonymous)'\n    status: 401\n    body: '{\"error\":\"Authorization field missing\"}'\n  - probe: 'GET https://api.agentboxcrm.com.au/listings?version=2 [X-API-Key: test]'\n    status: 404\n    note: passes the gateway; backend responds with x-ratelimit-limit /\n      x-ratelimit-remaining / x-ratelimit-reset\n- name: X-Client-ID\n  type: apiKey\n  in: header\n  parameter_name: X-Client-ID\n  required: true\n  description: >-\n    Per-agency client identifier sent alongside X-API-Key. Alone it does not\n    satisfy the gateway - a request carrying only X-Client-ID is still rejected\n    401 - so it is an application-level tenant identifier rather than the gateway\n    credential.\n  evidence:\n  - probe: 'GET https://api.agentboxcrm.com.au/ [X-Client-ID:\
  \ test]'\n    status: 401\n  - source: https://github.com/nad-au/agentbox\n    kind: third-party-client\n    note: sends both X-Client-ID and X-API-Key on every request\n  - source: https://github.com/real-coder-pty-ltd/stafflink-gf-agentbox\n    kind: third-party-client\n    note: same header pair plus Content-Type/Accept application/json\n- name: Office ID\n  type: tenant-identifier\n  in: credential-issuance\n  required: true\n  description: >-\n    Issued with the API Key and Client ID, scoping the credential to one agency\n    office's data. Not observed as a request header in the public third-party\n    clients; it is part of the credential triple support issues per office.\n  evidence:\n  - source: https://auctionslive.com/knowledge-hub/obtaining-reapit-agentbox-api-credentials\n    kind: third-party-docs\n    note: 'instructs the agency to email salessupportanz@reapit.com and request all\n      three: API Key, Client ID and Office ID'\ncredential_issuance:\n  self_serve: false\n\
  \  gate: application-approval\n  steps:\n  - Third party completes the Reapit Sales Integrator Application at\n    https://www.agentbox.com.au/integrator-application and is reviewed by the vendor.\n  - Each agency customer separately emails Reapit | Agentbox support\n    (salessupportanz@reapit.com, or support@agentbox.com.au for portal feeds) to\n    have credentials issued for its own office.\n  contacts:\n  - salessupportanz@reapit.com\n  - support@agentbox.com.au\noauth:\n  supported: false\n  evidence:\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n    is served on any host (see well-known/agentbox-well-known.yml).\n  - No authorization or token endpoint is documented anywhere on the public surface.\nscopes:\n  published: false\n  note: Key-based auth with per-office credential issuance; no OAuth scope surface\n    exists, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentbox/refs/heads/main/authentication/agentbox-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Real-Estate
- Australia
- Property Listings
- PropTech
- CRM
- REAXML
- Portal Feeds
- Rentals
- Commercial Real Estate
- New Zealand
---
