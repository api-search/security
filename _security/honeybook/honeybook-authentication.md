---
api_key_in: []
api_specs:
- filename: honeybook-clients-api-openapi.yml
  format: yaml
  label: HoneyBook Clients API
  slug: honeybook-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-clients-api-openapi.yml
- filename: honeybook-contracts-api-openapi.yml
  format: yaml
  label: HoneyBook Contracts API
  slug: honeybook-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-contracts-api-openapi.yml
- filename: honeybook-invoices-api-openapi.yml
  format: yaml
  label: HoneyBook Invoices API
  slug: honeybook-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-invoices-api-openapi.yml
- filename: honeybook-payments-api-openapi.yml
  format: yaml
  label: HoneyBook Payments API
  slug: honeybook-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-payments-api-openapi.yml
- filename: honeybook-projects-api-openapi.yml
  format: yaml
  label: HoneyBook Projects API
  slug: honeybook-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-projects-api-openapi.yml
- filename: honeybook-proposals-api-openapi.yml
  format: yaml
  label: HoneyBook Proposals API
  slug: honeybook-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-proposals-api-openapi.yml
- filename: honeybook-scheduler-api-openapi.yml
  format: yaml
  label: HoneyBook Scheduler API
  slug: honeybook-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-scheduler-api-openapi.yml
- filename: honeybook-webhooks-api-openapi.yml
  format: yaml
  label: HoneyBook Webhooks API
  slug: honeybook-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Honeybook Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HoneyBook secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HoneyBook
provider_slug: honeybook
scheme_count: 1
schemes:
- description: Third-party integration guides reference OAuth 2.0 against api.honeybook.com, but are inconsistent on the exact token endpoint and grant type and are not independently verifiable. Modeled here as an authorization-code flow with refresh tokens, the most common pattern for a user-data platform of this kind; treat as unverified.
  flows:
  - authorizationUrl: https://api.honeybook.com/oauth/authorize
    flow: authorizationCode
    scopes: 14
    tokenUrl: https://api.honeybook.com/oauth/token
  name: oauth2
  sources:
  - openapi/honeybook-openapi.yml
  type: oauth2
slug: honeybook-authentication
source_filename: honeybook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/honeybook-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.honeybook.com/oauth/authorize\n    tokenUrl: https://api.honeybook.com/oauth/token\n    scopes: 14\n  description: Third-party integration guides reference OAuth 2.0 against api.honeybook.com,\n    but are inconsistent on the exact token endpoint and grant type and are not independently\n    verifiable. Modeled here as an authorization-code flow with refresh tokens, the most common\n    pattern for a user-data platform of this kind; treat as unverified.\n  sources:\n  - openapi/honeybook-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/authentication/honeybook-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Clientflow
- Proposals
- Contracts
- Invoicing
- Payments
- Scheduling
- Creative Entrepreneurs
- Small Business
---
