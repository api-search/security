---
api_key_in: []
api_specs:
- filename: argus-enterprise-authentication-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Authentication API
  slug: argus-enterprise-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-authentication-api-openapi.yml
- filename: argus-enterprise-cash-flows-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Cash Flows API
  slug: argus-enterprise-cash-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-cash-flows-api-openapi.yml
- filename: argus-enterprise-events-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Events API
  slug: argus-enterprise-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-events-api-openapi.yml
- filename: argus-enterprise-health-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Health API
  slug: argus-enterprise-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-health-api-openapi.yml
- filename: argus-enterprise-leases-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Leases API
  slug: argus-enterprise-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-leases-api-openapi.yml
- filename: argus-enterprise-portfolios-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Portfolios API
  slug: argus-enterprise-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-portfolios-api-openapi.yml
- filename: argus-enterprise-properties-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Properties API
  slug: argus-enterprise-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-properties-api-openapi.yml
- filename: argus-enterprise-reports-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Reports API
  slug: argus-enterprise-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-reports-api-openapi.yml
- filename: argus-enterprise-subscriptions-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Subscriptions API
  slug: argus-enterprise-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-subscriptions-api-openapi.yml
- filename: argus-enterprise-tenants-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Tenants API
  slug: argus-enterprise-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-tenants-api-openapi.yml
- filename: argus-enterprise-users-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Users API
  slug: argus-enterprise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-users-api-openapi.yml
- filename: argus-enterprise-valuations-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Valuations API
  slug: argus-enterprise-valuations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-valuations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Argus Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARGUS Enterprise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from the /auth/token endpoint using client credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/argus-enterprise-core-openapi.yml
  - openapi/argus-enterprise-webhooks-openapi.yml
  type: http
slug: argus-enterprise-authentication
source_filename: argus-enterprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argus-enterprise-core-openapi.yml, openapi/argus-enterprise-webhooks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from the /auth/token endpoint using client credentials.\n  sources:\n  - openapi/argus-enterprise-core-openapi.yml\n  - openapi/argus-enterprise-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/authentication/argus-enterprise-authentication.yml
summary_line: http · 1 scheme
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio-Management
- Valuation
---
