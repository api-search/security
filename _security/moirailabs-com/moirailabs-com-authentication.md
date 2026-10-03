---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moirailabs-com-analytics-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Analytics Controller API
  slug: moirailabs-com-analytics-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-analytics-controller-api-openapi.yml
- filename: moirailabs-com-analytics-invocation-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Analytics Invocation Controller API
  slug: moirailabs-com-analytics-invocation-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-analytics-invocation-controller-api-openapi.yml
- filename: moirailabs-com-contract-info-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Contract Info Controller API
  slug: moirailabs-com-contract-info-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-contract-info-controller-api-openapi.yml
- filename: moirailabs-com-functions-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Functions Controller API
  slug: moirailabs-com-functions-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-functions-controller-api-openapi.yml
- filename: moirailabs-com-plan-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Plan Controller API
  slug: moirailabs-com-plan-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-plan-controller-api-openapi.yml
- filename: moirailabs-com-report-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Report Controller API
  slug: moirailabs-com-report-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-report-controller-api-openapi.yml
- filename: moirailabs-com-subscription-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Subscription Controller API
  slug: moirailabs-com-subscription-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-subscription-controller-api-openapi.yml
- filename: moirailabs-com-user-info-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs User Info Controller API
  slug: moirailabs-com-user-info-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-user-info-controller-api-openapi.yml
- filename: moirailabs-com-wallet-profiling-controller-api-openapi.yml
  format: yaml
  label: Moirai Labs Wallet Profiling Controller API
  slug: moirailabs-com-wallet-profiling-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-wallet-profiling-controller-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Moirailabs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moirai Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moirai Labs
provider_slug: moirailabs-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moirailabs-com-openapi.yml
  type: http
slug: moirailabs-com-authentication
source_filename: moirailabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/moirailabs-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/moirailabs-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/authentication/moirailabs-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Blockchain
- Smart Contracts
- Web3
- Analytics
- cohort-analysis
- Wallet Profiling
- Ethereum
- AI Agents
- A2A
- MCP
- Agent-Native
---
