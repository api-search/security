---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Kiwibot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kiwibot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kiwibot
provider_slug: kiwibot
scheme_count: 1
schemes:
- description: 'API consumer identity required on every request. Evidenced by the gateway''s own 401 body: "UNAUTHENTICATED: Method doesn''t allow unregistered callers (callers without established identity). Please use API Key or other form of API consumer identity to call this API."'
  evidence:
    body: '{"code":401,"message":"UNAUTHENTICATED: Method doesn''t allow unregistered callers (callers without established identity). Please use API Key or other form of API consumer identity to call this API."}'
    http_status: 401
    url: https://api.kiwibot.com/deliveries
  id: api_key
  in: unknown
  name: unknown
  type: apiKey
slug: kiwibot-authentication
source_filename: kiwibot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  Anonymous HTTP probes of https://api.kiwibot.com (2026-08-23). No OpenAPI securitySchemes exist\n  to derive from and no public auth documentation was found on any host.\napi: Kiwibot Delivery Platform API\nbase_url: https://api.kiwibot.com\ndocumented: false\ndocs: null\nnote: >-\n  Derived entirely from the gateway's own anonymous responses, because the provider publishes no\n  authentication page. api.kiwibot.com is a Google Cloud Endpoints / ESPv2 deployment: its\n  unauthenticated response is the verbatim Endpoints challenge string, which states the accepted\n  credential form. Whether the key travels as an `x-api-key` header or an `?key=` query parameter\n  is a per-deployment Endpoints choice that cannot be established anonymously and is NOT asserted\n  here.\nschemes:\n- id: api_key\n  type: apiKey\n  name: unknown\n  in: unknown\n  description: >-\n    API consumer identity required on every request. Evidenced\
  \ by the gateway's own 401 body:\n    \"UNAUTHENTICATED: Method doesn't allow unregistered callers (callers without established\n    identity). Please use API Key or other form of API consumer identity to call this API.\"\n  evidence:\n    url: https://api.kiwibot.com/deliveries\n    http_status: 401\n    body: >-\n      {\"code\":401,\"message\":\"UNAUTHENTICATED: Method doesn't allow unregistered callers (callers\n      without established identity). Please use API Key or other form of API consumer identity to\n      call this API.\"}\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes_published: false\nkey_issuance:\n  self_service: false\n  channel: sales/demo form\n  url: https://robot.com/contact\n  note: >-\n    No developer signup, no console, no key-management page was found on any probed host. The only\n    documented route to credentials is the demo request form on robot.com/contact.\ngaps:\n- No authentication documentation published at any public URL.\n- Credential\
  \ placement (header vs query parameter) is undocumented and not anonymously determinable.\n- No OAuth 2.0, OIDC discovery, or scope reference published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiwibot/refs/heads/main/authentication/kiwibot-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Robotics
- Autonomous Vehicles
- Delivery
- Last Mile Delivery
- Logistics
- Warehouse Automation
- Advertising
- ROS
- Open-Source
---
