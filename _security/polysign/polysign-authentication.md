---
api_key_in: []
api_specs:
- filename: polysign-atomicnet-api-server-openapi.json
  format: json
  label: AtomicNet API Server
  slug: atomicnet-api-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-atomicnet-api-server-openapi.json
- filename: polysign-merchant-gate-openapi.json
  format: json
  label: AtomicNet Merchant Gate Node
  slug: atomicnet-merchant-gate-node
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-merchant-gate-openapi.json
- filename: polysign-abc-proxy-service-openapi.json
  format: json
  label: AtomicNet ABC Proxy Service
  slug: atomicnet-abc-proxy-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-proxy-service-openapi.json
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
