---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Netbeez Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netbeez declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Netbeez
provider_slug: netbeez
scheme_count: 1
schemes:
- description: Dashboard-generated API key sent in the Authorization request header. Administrators generate keys in the NetBeez Dashboard under Settings > API Keys ("Generate API Key"). Applies to both the JSON v2 API (https://api.netbeez.net) and the deprecated read-only v1 Swagger API served per-instance at https://<dashboard_url>/swagger/index.html (which also prompts for the API key and a version, defaulting to v1).
  id: api_key
  in: header
  name: Authorization
  type: apiKey
slug: netbeez-authentication
source_filename: netbeez-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://help.netbeez.net/en/articles/10406758-netbeez-api (NetBeez API) + https://help.netbeez.net/en/articles/10406760-netbeez-api-swagger-endpoints\napi: NetBeez API\nsummary: >-\n  The NetBeez API authenticates with a dashboard-issued API key. The key is\n  passed in an \"Authorization\" HTTP header on every request. API keys are\n  generated and managed by dashboard administrators under Settings > API Keys.\nschemes:\n- id: api_key\n  type: apiKey\n  in: header\n  name: Authorization\n  description: >-\n    Dashboard-generated API key sent in the Authorization request header.\n    Administrators generate keys in the NetBeez Dashboard under\n    Settings > API Keys (\"Generate API Key\"). Applies to both the JSON\n    v2 API (https://api.netbeez.net) and the deprecated read-only v1\n    Swagger API served per-instance at https://<dashboard_url>/swagger/index.html\n    (which also prompts for the API key and a version, defaulting\
  \ to v1).\nkey_management:\n  location: NetBeez Dashboard > Settings > API Keys\n  action: Generate API Key\n  docs: https://help.netbeez.net/en/collections/11391846-integrations-and-api\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: >-\n  No OAuth2/OIDC or scope model is documented; access is a single bearer-style\n  API key. The v1 Swagger surface is read-only; the v2 JSON API supports read\n  and write (e.g. create targets, run ad-hoc tests).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbeez/refs/heads/main/authentication/netbeez-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Infrastructure Saas
- Network Monitoring
- Network Performance Monitoring
- Observability
- Wi-Fi Monitoring
- Digital Experience Monitoring
---
