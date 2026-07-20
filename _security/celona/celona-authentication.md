---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Celona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celona secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Celona
provider_slug: celona
scheme_count: 1
schemes:
- description: All Celona Orchestrator API operations require a valid API key sent in the X-API-Key request header. Keys are generated per user in the Orchestrator (user icon > API Keys > GENERATE KEY). The key value is shown once and is not recoverable afterward. Requests without a valid key are rejected (HTTP 403).
  in: header
  name: ApiKeyAuth
  parameter_name: X-API-Key
  sources:
  - docs
  type: apiKey
slug: celona-authentication
source_filename: celona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: http://docs.celona.io/en/articles/5471140-introduction-to-celona-apis\ndocs: http://docs.celona.io/en/articles/5467418-celona-network-monitoring-api-how-to\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: >-\n    All Celona Orchestrator API operations require a valid API key sent in the\n    X-API-Key request header. Keys are generated per user in the Orchestrator\n    (user icon > API Keys > GENERATE KEY). The key value is shown once and is not\n    recoverable afterward. Requests without a valid key are rejected (HTTP 403).\n  sources:\n  - docs\nnotes:\n- API keys are generated in the Celona Orchestrator UI; there is no OAuth client-credentials or token-exchange flow documented for the public API.\n- API access can be restricted to specific Device Groups (see docs article 8096652).\n- The Orchestrator\
  \ web application (cso.celona.io) additionally supports SSO/SAML (Okta, Azure) and MFA for interactive user login; that is separate from the X-API-Key used for REST API calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celona/refs/heads/main/authentication/celona-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Networking
- Private Cellular
- 5G
- LTE
- CBRS
- Wireless
- Network Monitoring
- Telecommunications
- IoT
---
