---
api_key_in:
- header
api_specs:
- filename: forex-com-session-api-openapi.yml
  format: yaml
  label: FOREX.com Session API
  slug: forex-com-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-session-api-openapi.yml
- filename: forex-com-account-api-openapi.yml
  format: yaml
  label: FOREX.com Account API
  slug: forex-com-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-account-api-openapi.yml
- filename: forex-com-market-api-openapi.yml
  format: yaml
  label: FOREX.com Market API
  slug: forex-com-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-market-api-openapi.yml
- filename: forex-com-pricing-api-openapi.yml
  format: yaml
  label: FOREX.com Pricing API
  slug: forex-com-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-pricing-api-openapi.yml
- filename: forex-com-account-api-openapi.yml
  format: yaml
  label: FOREX.com Account API
  slug: forex-com-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-account-api-openapi.yml
- filename: forex-com-margin-api-openapi.yml
  format: yaml
  label: FOREX.com Margin API
  slug: forex-com-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-margin-api-openapi.yml
- filename: forex-com-market-api-openapi.yml
  format: yaml
  label: FOREX.com Market API
  slug: forex-com-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-market-api-openapi.yml
- filename: forex-com-orders-api-openapi.yml
  format: yaml
  label: FOREX.com Orders API
  slug: forex-com-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-orders-api-openapi.yml
- filename: forex-com-positions-api-openapi.yml
  format: yaml
  label: FOREX.com Positions API
  slug: forex-com-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-positions-api-openapi.yml
- filename: forex-com-pricing-api-openapi.yml
  format: yaml
  label: FOREX.com Pricing API
  slug: forex-com-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-pricing-api-openapi.yml
- filename: forex-com-session-api-openapi.yml
  format: yaml
  label: FOREX.com Session API
  slug: forex-com-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/openapi/forex-com-session-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Forex Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: FOREX.com secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FOREX.com
provider_slug: forex-com
scheme_count: 2
schemes:
- description: Session ID obtained from POST /session
  in: header
  name: SessionAuth
  parameter: Session
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: FOREX.com account username
  in: header
  name: UserNameAuth
  parameter: UserName
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: forex-com-authentication
source_filename: forex-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SessionAuth\n  type: apiKey\n  in: header\n  parameter: Session\n  description: Session ID obtained from POST /session\n  sources:\n  - openapi/openapi.yml\n- name: UserNameAuth\n  type: apiKey\n  in: header\n  parameter: UserName\n  description: FOREX.com account username\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/authentication/forex-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Forex
- FX Trading
- CFD Trading
- Algorithmic Trading
- Financial-Services
- Trading APIs
- Currency Exchange
---
