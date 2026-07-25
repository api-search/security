---
api_key_in: []
api_specs:
- filename: b3-exchange-investor-position-openapi.json
  format: json
  label: B3 Investor Area (Área do Investidor) APIs
  slug: b3-investor-area-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-investor-position-openapi.json
- filename: b3-exchange-tesouro-direto-bonds-openapi.json
  format: json
  label: B3 Tesouro Direto APIs
  slug: b3-tesouro-direto-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-tesouro-direto-bonds-openapi.json
- filename: b3-exchange-otc-public-info-openapi.json
  format: json
  label: B3 OTC (Balcão) APIs
  slug: b3-otc-balcao-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-otc-public-info-openapi.json
- filename: b3-exchange-core-calculation-openapi.json
  format: json
  label: B3 Listed Markets (Listados) APIs
  slug: b3-listed-markets-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-core-calculation-openapi.json
- filename: b3-exchange-isin-openapi.json
  format: json
  label: B3 ISIN API
  slug: b3-isin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-isin-openapi.json
- filename: b3-exchange-banco-b3-custody-openapi.json
  format: json
  label: Banco B3 APIs
  slug: b3-banco-b3-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-banco-b3-custody-openapi.json
- filename: b3-exchange-insurance-claim-openapi.json
  format: json
  label: B3 Insurance (Seguros) APIs
  slug: b3-insurance-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-insurance-claim-openapi.json
- filename: b3-exchange-auth-client-credentials-openapi.json
  format: json
  label: B3 Authentication APIs
  slug: b3-authentication-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-auth-client-credentials-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: B3 Exchange Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: B3 (Brasil Bolsa Balcão) secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: B3 (Brasil Bolsa Balcão)
provider_slug: b3-exchange
scheme_count: 3
schemes:
- docs: https://developers.b3.com.br/apis/autenticacao
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - openapi/b3-exchange-auth-client-credentials-openapi.json
  token_endpoint_path: /aapi/oauth/token
  token_request:
    content_type: application/x-www-form-urlencoded
    method: POST
    parameters:
    - client_id
    - client_secret
    - grant_type
  type: oauth2
- docs: https://developers.b3.com.br/apis/autenticacao
  flow: password
  name: OAuth2ROPC
  sources:
  - openapi/b3-exchange-auth-ropc-openapi.json
  token_endpoint_path: /api/oauth/token
  token_request:
    content_type: application/x-www-form-urlencoded
    method: POST
    parameters:
    - client_id
    - client_secret
    - grant_type
    - username
    - password
  type: oauth2
- description: Per-API OAuth 2.0 security profile applied across the catalog - bearer access token in the Authorization header, scopes resource.READ and resource.WRITE, any-scope matching.
  header_prefix: Bearer
  name: OAuth2ResourceAccess
  scopes:
  - resource.READ
  - resource.WRITE
  sources:
  - openapi/b3-exchange-investor-position-openapi.json
  - openapi/b3-exchange-investor-transactions-openapi.json
  - openapi/b3-exchange-isin-openapi.json
  - openapi/b3-exchange-otc-public-info-openapi.json
  - openapi/b3-exchange-tesouro-direto-bonds-openapi.json
  - openapi/b3-exchange-tesouro-direto-positions-openapi.json
  - openapi/b3-exchange-tesouro-direto-orders-openapi.json
  - openapi/b3-exchange-banco-b3-custody-openapi.json
  - openapi/b3-exchange-banco-b3-settlement-openapi.json
  - openapi/b3-exchange-core-calculation-openapi.json
  - openapi/b3-exchange-securities-lending-openapi.json
  - openapi/b3-exchange-insurance-claim-openapi.json
  token_location: header
  type: oauth2
slug: b3-exchange-authentication
source_filename: b3-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/ (12 of 14 harvested Swagger 1.1 definitions declare oauth2 authorizations)\ndocs: https://developers.b3.com.br/apis/autenticacao\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, password]\n  token_location: header\n  header_prefix: Bearer\n  scopes_matching: Any\n  notes: >-\n    All B3 for Developers REST APIs authenticate with OAuth 2.0 bearer tokens.\n    The portal documents six token-issuance model APIs - Client Credentials\n    (plain, plus category_ID, key, and scope parameter variants) and Resource\n    Owner Password Credentials (plain and category_ID variants). Access is\n    B2B-only: client_id/client_secret credentials are issued to contracted\n    institutions, not self-serve. The Swagger definitions carry a placeholder\n    token endpoint (https://localhost:8089/api/oauth/token) that the portal\n    substitutes with the client's entitled gateway host at runtime.\nschemes:\n  - name: OAuth2ClientCredentials\n\
  \    type: oauth2\n    flow: clientCredentials\n    token_endpoint_path: /aapi/oauth/token\n    token_request:\n      method: POST\n      content_type: application/x-www-form-urlencoded\n      parameters: [client_id, client_secret, grant_type]\n    docs: https://developers.b3.com.br/apis/autenticacao\n    sources:\n      - openapi/b3-exchange-auth-client-credentials-openapi.json\n  - name: OAuth2ROPC\n    type: oauth2\n    flow: password\n    token_endpoint_path: /api/oauth/token\n    token_request:\n      method: POST\n      content_type: application/x-www-form-urlencoded\n      parameters: [client_id, client_secret, grant_type, username, password]\n    docs: https://developers.b3.com.br/apis/autenticacao\n    sources:\n      - openapi/b3-exchange-auth-ropc-openapi.json\n  - name: OAuth2ResourceAccess\n    type: oauth2\n    description: >-\n      Per-API OAuth 2.0 security profile applied across the catalog - bearer\n      access token in the Authorization header, scopes resource.READ\
  \ and\n      resource.WRITE, any-scope matching.\n    token_location: header\n    header_prefix: Bearer\n    scopes: [resource.READ, resource.WRITE]\n    sources:\n      - openapi/b3-exchange-investor-position-openapi.json\n      - openapi/b3-exchange-investor-transactions-openapi.json\n      - openapi/b3-exchange-isin-openapi.json\n      - openapi/b3-exchange-otc-public-info-openapi.json\n      - openapi/b3-exchange-tesouro-direto-bonds-openapi.json\n      - openapi/b3-exchange-tesouro-direto-positions-openapi.json\n      - openapi/b3-exchange-tesouro-direto-orders-openapi.json\n      - openapi/b3-exchange-banco-b3-custody-openapi.json\n      - openapi/b3-exchange-banco-b3-settlement-openapi.json\n      - openapi/b3-exchange-core-calculation-openapi.json\n      - openapi/b3-exchange-securities-lending-openapi.json\n      - openapi/b3-exchange-insurance-claim-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/authentication/b3-exchange-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Financial
- Market Data
- Stocks
- Trading
- Exchange
- Derivatives
- Fixed Income
- Real-Time
- Reference Data
- Brazil
---
