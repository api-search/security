---
api_key_in:
- header
api_specs:
- filename: truebiz-async-web-presence-review-api-openapi.yml
  format: yaml
  label: TrueBiz Async Web Presence Review API
  slug: truebiz-async-web-presence-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-async-web-presence-review-api-openapi.yml
- filename: truebiz-fraud-searches-api-openapi.yml
  format: yaml
  label: TrueBiz Fraud Searches API
  slug: truebiz-fraud-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-fraud-searches-api-openapi.yml
- filename: truebiz-history-api-openapi.yml
  format: yaml
  label: TrueBiz History API
  slug: truebiz-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-history-api-openapi.yml
- filename: truebiz-industry-discovery-api-openapi.yml
  format: yaml
  label: TrueBiz Industry Discovery API
  slug: truebiz-industry-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-industry-discovery-api-openapi.yml
- filename: truebiz-industry-discovery-history-api-openapi.yml
  format: yaml
  label: TrueBiz Industry Discovery History API
  slug: truebiz-industry-discovery-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-industry-discovery-history-api-openapi.yml
- filename: truebiz-monitoring-alerts-api-openapi.yml
  format: yaml
  label: TrueBiz Monitoring Alerts API
  slug: truebiz-monitoring-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-monitoring-alerts-api-openapi.yml
- filename: truebiz-monitoring-domains-api-openapi.yml
  format: yaml
  label: TrueBiz Monitoring Domains API
  slug: truebiz-monitoring-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-monitoring-domains-api-openapi.yml
- filename: truebiz-web-presence-review-api-openapi.yml
  format: yaml
  label: TrueBiz Web Presence Review API
  slug: truebiz-web-presence-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-web-presence-review-api-openapi.yml
- filename: truebiz-web-presence-review-blocklist-api-openapi.yml
  format: yaml
  label: TrueBiz Web Presence Review Blocklist API
  slug: truebiz-web-presence-review-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-web-presence-review-blocklist-api-openapi.yml
- filename: truebiz-web-presence-review-history-api-openapi.yml
  format: yaml
  label: TrueBiz Web Presence Review History API
  slug: truebiz-web-presence-review-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-web-presence-review-history-api-openapi.yml
- filename: truebiz-website-status-api-openapi.yml
  format: yaml
  label: TrueBiz Website Status API
  slug: truebiz-website-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/openapi/truebiz-website-status-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Truebiz Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueBiz secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TrueBiz
provider_slug: truebiz
scheme_count: 4
schemes:
- description: Primary authentication. Send your TrueBiz API key in the X-API-KEY header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/truebiz-openapi-original.json
  type: apiKey
- description: Same X-API-KEY header, applied to the asynchronous (job-submission) endpoints.
  in: header
  name: AsyncApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/truebiz-openapi-original.json
  type: apiKey
- description: PropelAuth-issued bearer JWT accepted for dashboard/app-originated calls.
  name: PropelAuthBearer
  scheme: bearer
  sources:
  - openapi/truebiz-openapi-original.json
  type: http
- description: PropelAuth bearer JWT applied to the asynchronous endpoints.
  name: AsyncPropelAuthBearer
  scheme: bearer
  sources:
  - openapi/truebiz-openapi-original.json
  type: http
slug: truebiz-authentication
source_filename: truebiz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/truebiz-openapi-original.json\ndocs: https://ae.truebiz.io/api/v1/docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    All requests to TrueBiz require an API key sent in the X-API-KEY request\n    header (documented in the API reference Introduction). A PropelAuth bearer\n    JWT is accepted as an alternative for dashboard-issued sessions. There is no\n    OAuth2 authorization-code/scoped flow, so no scopes artifact applies.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Primary authentication. Send your TrueBiz API key in the X-API-KEY header.\n  sources:\n  - openapi/truebiz-openapi-original.json\n- name: AsyncApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Same X-API-KEY header, applied to the asynchronous (job-submission) endpoints.\n  sources:\n  - openapi/truebiz-openapi-original.json\n\
  - name: PropelAuthBearer\n  type: http\n  scheme: bearer\n  description: PropelAuth-issued bearer JWT accepted for dashboard/app-originated calls.\n  sources:\n  - openapi/truebiz-openapi-original.json\n- name: AsyncPropelAuthBearer\n  type: http\n  scheme: bearer\n  description: PropelAuth bearer JWT applied to the asynchronous endpoints.\n  sources:\n  - openapi/truebiz-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truebiz/refs/heads/main/authentication/truebiz-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Security
- Fraud Prevention
- Business Verification
- Merchant Risk
- KYB
- Underwriting
- Payments
- Monitoring
---
