---
api_key_in:
- header
- query
api_specs:
- filename: dashbot-export-api-openapi.yml
  format: yaml
  label: Dashbot Export API
  slug: dashbot-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/openapi/dashbot-export-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dashbot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dashbot secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dashbot
provider_slug: dashbot
scheme_count: 2
schemes:
- description: API key passed in the Authorization header on the Export API (GET https://api.dimensionlabs.io/export and GET https://api.dimensionlabs.io/index). The OpenAPI models it as a required header PARAMETER rather than a securityScheme, so no formal components.securitySchemes block exists in the published spec. No Bearer or other prefix is documented — the raw key is the header value.
  in: header
  name: AuthorizationHeader
  operations:
  - get_export
  - get_new-endpoint
  parameter: Authorization
  sources:
  - openapi/dashbot-export-api-openapi.yml
  type: apiKey
- description: API key supplied as a QUERY parameter on every Universal tracker ingest call — https://tracker.dimensionlabs.io/track and /trackhistorical, e.g. ?platform=universal&v=11.1.0-rest&type=incoming&apiKey=API_KEY_HERE. Each integration source has its own key. No header alternative is documented.
  in: query
  name: TrackerApiKey
  parameter: apiKey
  risk_note: A credential in the query string is written to proxy, CDN and server access logs and to browser history. Dimension Labs documents no header-based alternative for the ingest path.
  sources:
  - https://docs.dimensionlabs.io/reference/rest-api
  type: apiKey
slug: dashbot-authentication
source_filename: dashbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://docs.dimensionlabs.io/reference/generating-dashbot-api-key,\n  https://docs.dimensionlabs.io/reference/rest-api,\n  https://docs.dimensionlabs.io/reference/sending-data-to-dimension, plus\n  openapi/dashbot-export-api-openapi.yml (both operations declare the\n  Authorization header parameter).\ndocs: https://docs.dimensionlabs.io/reference/generating-dashbot-api-key\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: AuthorizationHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    API key passed in the Authorization header on the Export API\n    (GET https://api.dimensionlabs.io/export and GET\n    https://api.dimensionlabs.io/index). The OpenAPI models it as a required\n    header PARAMETER rather than a securityScheme, so no formal\n    components.securitySchemes block exists in the\
  \ published spec. No Bearer or\n    other prefix is documented — the raw key is the header value.\n  operations: [get_export, get_new-endpoint]\n  sources: [openapi/dashbot-export-api-openapi.yml]\n- name: TrackerApiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: >-\n    API key supplied as a QUERY parameter on every Universal tracker ingest call\n    — https://tracker.dimensionlabs.io/track and /trackhistorical, e.g.\n    ?platform=universal&v=11.1.0-rest&type=incoming&apiKey=API_KEY_HERE. Each\n    integration source has its own key. No header alternative is documented.\n  risk_note: >-\n    A credential in the query string is written to proxy, CDN and server access\n    logs and to browser history. Dimension Labs documents no header-based\n    alternative for the ingest path.\n  sources: [https://docs.dimensionlabs.io/reference/rest-api]\nkey_provisioning:\n  location: Dimension Labs app — Integrations > Add Source > Show Integration Instructions\n  scope: one\
  \ key per integration source\n  rotation: not documented\n  expiry: not documented\n  docs: https://docs.dimensionlabs.io/reference/generating-dashbot-api-key\nmcp_authentication:\n  endpoint: https://docs.dimensionlabs.io/mcp\n  scheme: unknown\n  note: >-\n    The MCP endpoint rejects anonymous calls with JSON-RPC error -32001\n    \"Authorization required\" but publishes no OAuth metadata\n    (/.well-known/oauth-protected-resource and\n    /.well-known/oauth-authorization-server both 404), so the authorization\n    method an agent should use is not discoverable.\nnot_supported:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  - http basic\n  - http bearer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/authentication/dashbot-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai Ml
- Conversational Analytics
- Chatbots
- Voice Assistants
- Customer Experience
- Data Enrichment
- Analytics
- Contact Center
---
