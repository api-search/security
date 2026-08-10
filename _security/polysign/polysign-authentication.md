---
api_key_in: []
api_specs:
- filename: polysign-abc-accounts-api-openapi.yml
  format: yaml
  label: PolySign ABC Accounts API
  slug: polysign-abc-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-accounts-api-openapi.yml
- filename: polysign-abc-memorials-api-openapi.yml
  format: yaml
  label: PolySign ABC Memorials API
  slug: polysign-abc-memorials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-memorials-api-openapi.yml
- filename: polysign-abc-signing-api-openapi.yml
  format: yaml
  label: PolySign ABC Signing API
  slug: polysign-abc-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-signing-api-openapi.yml
- filename: polysign-abc-testnet-api-openapi.yml
  format: yaml
  label: PolySign ABC Testnet API
  slug: polysign-abc-testnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-testnet-api-openapi.yml
- filename: polysign-asset-api-openapi.yml
  format: yaml
  label: PolySign Asset API
  slug: polysign-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-asset-api-openapi.yml
- filename: polysign-authentication-api-openapi.yml
  format: yaml
  label: PolySign Authentication API
  slug: polysign-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-authentication-api-openapi.yml
- filename: polysign-beneficiary-authorization-api-openapi.yml
  format: yaml
  label: PolySign beneficiary authorization API
  slug: polysign-beneficiary-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-beneficiary-authorization-api-openapi.yml
- filename: polysign-book-transfer-api-openapi.yml
  format: yaml
  label: PolySign book transfer API
  slug: polysign-book-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-book-transfer-api-openapi.yml
- filename: polysign-book-transfer-confirmation-api-openapi.yml
  format: yaml
  label: PolySign book transfer confirmation API
  slug: polysign-book-transfer-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-book-transfer-confirmation-api-openapi.yml
- filename: polysign-escrow-authorization-api-openapi.yml
  format: yaml
  label: PolySign escrow authorization API
  slug: polysign-escrow-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-escrow-authorization-api-openapi.yml
- filename: polysign-investor-api-openapi.yml
  format: yaml
  label: PolySign Investor API
  slug: polysign-investor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-investor-api-openapi.yml
- filename: polysign-order-api-openapi.yml
  format: yaml
  label: PolySign Order API
  slug: polysign-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-order-api-openapi.yml
- filename: polysign-partner-api-openapi.yml
  format: yaml
  label: PolySign Partner API
  slug: polysign-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-partner-api-openapi.yml
- filename: polysign-settlement-api-openapi.yml
  format: yaml
  label: PolySign Settlement API
  slug: polysign-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-settlement-api-openapi.yml
- filename: polysign-settlement-confirmation-api-openapi.yml
  format: yaml
  label: PolySign settlement confirmation API
  slug: polysign-settlement-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-settlement-confirmation-api-openapi.yml
- filename: polysign-system-api-openapi.yml
  format: yaml
  label: PolySign System API
  slug: polysign-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-system-api-openapi.yml
- filename: polysign-utility-api-openapi.yml
  format: yaml
  label: PolySign Utility API
  slug: polysign-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-utility-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Polysign Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: PolySign secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: PolySign
provider_slug: polysign
scheme_count: 1
schemes:
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /v1/auth/token
  name: OAuth2
  sources:
  - openapi/polysign-abc-proxy-service-openapi.json
  - openapi/polysign-atomicnet-api-server-openapi.json
  - openapi/polysign-merchant-gate-openapi.json
  type: oauth2
slug: polysign-authentication
source_filename: polysign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/polysign-abc-proxy-service-openapi.json, openapi/polysign-atomicnet-api-server-openapi.json,\n  openapi/polysign-merchant-gate-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n    scopes: 1\n  description: OAuth 2.0 with the client credentials grant flow.\n  sources:\n  - openapi/polysign-abc-proxy-service-openapi.json\n  - openapi/polysign-atomicnet-api-server-openapi.json\n  - openapi/polysign-merchant-gate-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/authentication/polysign-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- digital-assets
- blockchain
- institutional-custody
- settlement
- escrow
- capital-markets
- payments
- fintech
- distributed-ledger
- atomicnet
---
