---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Taxo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TAXO secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TAXO
provider_slug: taxo
scheme_count: 2
schemes:
- description: OAuth 2.0 with access and refresh tokens, documented for the Taxo API white-label electronic-invoicing product.
  flows:
  - flow: authorizationCode
  name: OAuth2
  sources:
  - https://taxo.co/ec/productos/taxo-api
  type: oauth2
- description: Bearer token presented as an API key on requests (documented as "Bearer token via API Key" on the Taxo API product page).
  name: bearerAuth
  scheme: bearer
  sources:
  - https://taxo.co/ec/productos/taxo-api
  type: http
slug: taxo-authentication
source_filename: taxo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.taxo.ws/getting-started\ndocs: https://docs.taxo.ws/getting-started\nnote: >-\n  No public OpenAPI specification was discoverable; the auth model below is\n  captured from the Taxo API product page (https://taxo.co/ec/productos/taxo-api)\n  and the developer documentation at docs.taxo.ws. api.taxo.co is a serverless\n  backend that returns JSON without a public spec.\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 with access and refresh tokens, documented for the Taxo API\n    white-label electronic-invoicing product.\n  flows:\n  - flow: authorizationCode\n  sources:\n  - https://taxo.co/ec/productos/taxo-api\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token presented as an API key on requests (documented as \"Bearer\n    token via API Key\" on\
  \ the Taxo API product page).\n  sources:\n  - https://taxo.co/ec/productos/taxo-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxo/refs/heads/main/authentication/taxo-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Accounting
- Tax
- Fintech
- Electronic Invoicing
- Facturación Electrónica
- CFDI
- SRI
- SAT
- Artificial Intelligence
- Ecuador
- Mexico
- API
---
