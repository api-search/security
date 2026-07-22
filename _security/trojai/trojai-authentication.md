---
api_key_in:
- header
api_specs:
- filename: eng-api
  format: yaml
  label: TrojAI Platform API
  slug: trojai-platform-api
  spec_type: OpenAPI
  url: https://docs.troj.ai/reference/eng-api
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Trojai Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrojAI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TrojAI
provider_slug: trojai
scheme_count: 2
schemes:
- applies_to: Platform API (/api/v2 endpoints)
  description: Raw API key generated in the web application (profile menu > API Keys > Generate API Key). Sent verbatim in the x-trojai-api-key header, NOT prefixed with "Bearer". Shown only once at creation. Authenticates management calls (users, datasets, models, firewall configs, firewall events, red team jobs/results, secrets).
  in: header
  name: platform-api-key
  parameter: x-trojai-api-key
  source: https://docs.troj.ai/reference/eng-api
  type: apiKey
- applies_to: Firewall Proxy API (TrojAI Defend)
  description: Client-ID header used by the Defend Firewall Proxy API to select which firewall policy applies to a proxied request. Distinct from the platform x-trojai-api-key.
  in: header
  name: firewall-proxy-client-id
  parameter: x-eag-clientid
  source: https://docs.troj.ai/trojai-defend/eng-proxy-api
  type: apiKey
slug: trojai-authentication
source_filename: trojai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.troj.ai/reference/eng-api\ndocs: https://docs.troj.ai/reference/eng-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The TrojAI platform is self-hosted / single-tenant (Cloud or Enterprise),\n    so the API host is per-deployment (https://<your_trojai_host>). The platform\n    API and the Firewall Proxy API use two distinct header-based keys. Platform\n    user identity is backed by Keycloak (upgraded to Keycloak 26 in v2.17.0);\n    rotating the identity provider invalidates existing API keys, which must be\n    regenerated.\nschemes:\n  - name: platform-api-key\n    type: apiKey\n    in: header\n    parameter: x-trojai-api-key\n    applies_to: Platform API (/api/v2 endpoints)\n    description: >-\n      Raw API key generated in the web application (profile menu > API Keys >\n      Generate API Key). Sent verbatim in the x-trojai-api-key header, NOT\n      prefixed\
  \ with \"Bearer\". Shown only once at creation. Authenticates\n      management calls (users, datasets, models, firewall configs, firewall\n      events, red team jobs/results, secrets).\n    source: https://docs.troj.ai/reference/eng-api\n  - name: firewall-proxy-client-id\n    type: apiKey\n    in: header\n    parameter: x-eag-clientid\n    applies_to: Firewall Proxy API (TrojAI Defend)\n    description: >-\n      Client-ID header used by the Defend Firewall Proxy API to select which\n      firewall policy applies to a proxied request. Distinct from the platform\n      x-trojai-api-key.\n    source: https://docs.troj.ai/trojai-defend/eng-proxy-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trojai/refs/heads/main/authentication/trojai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Security
- Machine Learning
- LLM Security
- Red Teaming
- AI Firewall
- Prompt Injection
- Model Risk
- MLOps
- Agentic AI
---
