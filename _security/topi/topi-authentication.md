---
api_key_in: []
api_specs:
- filename: topi-seller-api-openapi-original.yaml
  format: yaml
  label: topi Seller API
  slug: topi-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-seller-api-openapi-original.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Topi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Topi secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Topi
provider_slug: topi
scheme_count: 1
schemes:
- description: Read our [Integration Guide](https://developer.topi.eu/docs/get-started/introduction) for detailed instructions on how to authenticate.
  flows:
  - flow: clientCredentials
    scopes: 13
    tokenUrl: https://identity.topi.eu/oauth2/token
  name: OAuth2Seller_header_Authorization
  sources:
  - openapi/topi-seller-api-openapi-original.yaml
  type: oauth2
slug: topi-authentication
source_filename: topi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/topi-seller-api-openapi-original.yaml\ndocs: https://developer.topi.eu/docs/get-started/introduction\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2Seller_header_Authorization\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.topi.eu/oauth2/token\n    scopes: 13\n  description: Read our [Integration Guide](https://developer.topi.eu/docs/get-started/introduction)\n    for detailed instructions on how to authenticate.\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/authentication/topi-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Hardware as a Service
- Rental
- Embedded Finance
- B2B Payments
- Financing
- Checkout
- Germany
- API
---
