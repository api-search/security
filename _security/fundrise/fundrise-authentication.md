---
api_key_in: []
api_specs:
- filename: fundrise-acknowledgments-api-openapi.yml
  format: yaml
  label: Fundrise Acknowledgments API
  slug: fundrise-acknowledgments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-acknowledgments-api-openapi.yml
- filename: fundrise-authentication-api-openapi.yml
  format: yaml
  label: Fundrise Authentication API
  slug: fundrise-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-authentication-api-openapi.yml
- filename: fundrise-clients-api-openapi.yml
  format: yaml
  label: Fundrise Clients API
  slug: fundrise-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-clients-api-openapi.yml
- filename: fundrise-holdings-api-openapi.yml
  format: yaml
  label: Fundrise Holdings API
  slug: fundrise-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-holdings-api-openapi.yml
- filename: fundrise-investments-api-openapi.yml
  format: yaml
  label: Fundrise Investments API
  slug: fundrise-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-investments-api-openapi.yml
- filename: fundrise-liquidations-api-openapi.yml
  format: yaml
  label: Fundrise Liquidations API
  slug: fundrise-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-liquidations-api-openapi.yml
- filename: fundrise-offerings-api-openapi.yml
  format: yaml
  label: Fundrise Offerings API
  slug: fundrise-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-offerings-api-openapi.yml
- filename: fundrise-tax-forms-api-openapi.yml
  format: yaml
  label: Fundrise Tax Forms API
  slug: fundrise-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-tax-forms-api-openapi.yml
- filename: fundrise-transactions-api-openapi.yml
  format: yaml
  label: Fundrise Transactions API
  slug: fundrise-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fundrise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fundrise secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fundrise
provider_slug: fundrise
scheme_count: 2
schemes:
- credential_issuance: Fundrise support (connect@fundrise.com)
  description: '"PartnerBasicAuthentication is enforced by HTTP Basic Authentication. A Partner username and password will be provided by Fundrise support. The Partner password should be stored securely. At a minimum, it should be encrypted at-rest and access restricted to services making requests to the Fundrise API. The Partner password should not be exposed to a Client or any of their devices. If the password is compromised please contact Fundrise support."'
  name: PartnerBasicAuthentication
  operations:
  - GetAccessToken
  - GetOfferings
  - GetHistoricalNav
  - GetOfferingDocuments
  - CreateClient
  rfc: RFC 7617
  rotation_policy: not-published
  scheme: basic
  self_service: false
  sources:
  - openapi/fundrise-connect-openapi.yml
  subject: Partner
  type: http
- bearer_format: not-published
  description: '"ClientBearerAuthentication is enforced by HTTP Bearer Authentication and requires an OAuth access token. Since access tokens are scoped to specific Clients, they identify and authenticate the Client in a request. Access tokens can be obtained in Get Access Token requests by using the refresh token flow. OAuth refresh tokens are issued on Client Creation and scoped specifically to that Client. The refresh tokens will not expire and should be stored securely after Client creation. At a minimum, refresh tokens should be encrypted at-rest and access restricted to services making requests to the Fundrise API. Refresh tokens should not be exposed to a Client or any of their devices."'
  name: ClientBearerAuthentication
  operations:
  - CreateShareLiquidationRequest
  - CancelShareLiquidationRequest
  - GetLiquidationAcknowledgments
  - GetInvestmentAcknowledgments
  - GetHoldings
  - GetClient
  - UpdateClient
  - PlaceInvestment
  - CancelInvestment
  - GetTaxForms
  - GetTransaction
  - GetTransactions
  rfc: RFC 6750
  scheme: bearer
  sources:
  - openapi/fundrise-connect-openapi.yml
  subject: Client
  type: http
slug: fundrise-authentication
source_filename: fundrise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/fundrise-connect-openapi.yml\ndocs: https://connect.fundrise.com/#tag/Authentication\nnotes: >-\n  Baseline derived by 0-working/derive-authentication.py from the published OpenAPI 3.1.0,\n  then upgraded from the Authentication tag of the Fundrise Connect documentation, which\n  documents the two-subject model, the token exchange, the credential-handling\n  obligations, and the per-partner access-control layer that the securitySchemes block\n  alone does not express.\n\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  api_key_in: []\n  oauth2_flows_declared_in_spec: []\n  oauth2_in_practice:\n  - refresh_token\n  model: two-subject\n  access_request: https://fundrise.com/connect-api/contact\n  contact: connect@fundrise.com\n\nschemes:\n- name: PartnerBasicAuthentication\n  type: http\n  scheme: basic\n  subject: Partner\n  rfc: RFC 7617\n  description: >-\n    \"PartnerBasicAuthentication is\
  \ enforced by HTTP Basic Authentication. A Partner\n    username and password will be provided by Fundrise support. The Partner password\n    should be stored securely. At a minimum, it should be encrypted at-rest and access\n    restricted to services making requests to the Fundrise API. The Partner password\n    should not be exposed to a Client or any of their devices. If the password is\n    compromised please contact Fundrise support.\"\n  credential_issuance: Fundrise support (connect@fundrise.com)\n  self_service: false\n  rotation_policy: not-published\n  operations:\n  - GetAccessToken\n  - GetOfferings\n  - GetHistoricalNav\n  - GetOfferingDocuments\n  - CreateClient\n  sources:\n  - openapi/fundrise-connect-openapi.yml\n\n- name: ClientBearerAuthentication\n  type: http\n  scheme: bearer\n  subject: Client\n  rfc: RFC 6750\n  description: >-\n    \"ClientBearerAuthentication is enforced by HTTP Bearer Authentication and requires an\n    OAuth access token. Since access tokens\
  \ are scoped to specific Clients, they identify\n    and authenticate the Client in a request. Access tokens can be obtained in Get Access\n    Token requests by using the refresh token flow. OAuth refresh tokens are issued on\n    Client Creation and scoped specifically to that Client. The refresh tokens will not\n    expire and should be stored securely after Client creation. At a minimum, refresh\n    tokens should be encrypted at-rest and access restricted to services making requests\n    to the Fundrise API. Refresh tokens should not be exposed to a Client or any of their\n    devices.\"\n  bearer_format: not-published\n  operations:\n  - CreateShareLiquidationRequest\n  - CancelShareLiquidationRequest\n  - GetLiquidationAcknowledgments\n  - GetInvestmentAcknowledgments\n  - GetHoldings\n  - GetClient\n  - UpdateClient\n  - PlaceInvestment\n  - CancelInvestment\n  - GetTaxForms\n  - GetTransaction\n  - GetTransactions\n  sources:\n  - openapi/fundrise-connect-openapi.yml\n\ntoken_exchange:\n\
  \  operation: GetAccessToken\n  path: /v1/oauth/token\n  method: post\n  auth: PartnerBasicAuthentication\n  grant: refresh_token\n  request_field: refreshToken\n  response_schema: OAuth2AccessTokenResponse\n  response_fields:\n  - accessToken\n  - refreshToken\n  - scope\n  - tokenType\n  - expiresIn\n  refresh_token_source: CreateClient\n  refresh_token_expiry: none\n  access_token_expiry: returned as expiresIn; no fixed value published\n  note: >-\n    A genuine OAuth refresh-token exchange is modelled in the spec as a plain http bearer\n    securityScheme rather than an oauth2 scheme with declared flows, so generated clients\n    receive no flow metadata, no tokenUrl, and no scope list. Declaring it as oauth2 with\n    a clientCredentials or custom flow would make the contract self-describing.\n\nseparate_consumer_oauth_surface:\n  discovery: https://fundrise.com/.well-known/openid-configuration\n  http_status: 200\n  authorization_endpoint: https://fundrise.com/oauth/authorize\n \
  \ token_endpoint: https://api.fundrise.com/oauth/token\n  scopes_supported:\n  - openid\n  - offline_access\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  note: >-\n    This is Fundrise's consumer-facing OAuth/OIDC authorization server, discovered\n    anonymously and distinct from the Connect partner API's own token operation. It is\n    recorded here and in scopes/fundrise-scopes.yml because it is the only place Fundrise\n    publishes named scopes. The discovery document omits issuer, jwks_uri,\n    subject_types_supported and id_token_signing_alg_values_supported, so it is a partial\n    rather than conformant OIDC discovery document.\n\nauthorization:\n  model: scheme-per-operation plus per-partner allowlist\n  scopes: see scopes/fundrise-scopes.yml\n  documented_statement: >-\n    \"To ensure a safe, secure platform, Fundrise imposes strict access controls to all\n    APIs. As such, there may be services or capabilities documented\
  \ that are inaccessible\n    with current permissions. Contact the support team via connect@fundrise.com to gain\n    permissions for additional endpoints.\"\n  note: >-\n    Endpoint-level authorization is expressed by which of the two schemes an operation\n    requires, plus an out-of-band per-partner permission grant. A 403 on a documented\n    operation is expected behaviour under this model, not a defect.\n\ncredential_handling_requirements:\n- Partner password encrypted at rest.\n- Client refresh tokens encrypted at rest.\n- Access to both restricted to the services making API requests.\n- Neither ever exposed to a Client or a Client device.\n- Compromise reported to Fundrise support.\n\ngaps:\n- The OAuth exchange is not declared as an oauth2 securityScheme, so flows and scopes are invisible to tooling.\n- No bearerFormat is declared, so token structure (JWT or opaque) is undocumented.\n- Refresh tokens never expire and no rotation or revocation mechanism is published.\n- No mutual\
  \ TLS, no request signing, and no key rotation policy documented for Partner Basic credentials.\n- The OIDC discovery document is incomplete against OpenID Connect Discovery 1.0.\n\nx-evidence:\n- fetched: '2026-08-04'\n  url: https://connect.fundrise.com/\n  http_status: 200\n  note: OpenAPI 3.1.0 and the Authentication tag narrative.\n- fetched: '2026-08-04'\n  url: https://fundrise.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/authentication/fundrise-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Financial-Services
- Investing
- Real-Estate
- Private Credit
- Venture Capital
- Alternative Assets
- Wealth Management
- Fintech
- Embedded Investing
---
