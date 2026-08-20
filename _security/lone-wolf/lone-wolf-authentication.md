---
api_key_in:
- header
- query
api_specs:
- filename: lone-wolf-transact-api-openapi.yml
  format: yaml
  label: Lone Wolf Transact API
  slug: lone-wolf-transact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-transact-api-openapi.yml
- filename: lone-wolf-deals-api-openapi.yml
  format: yaml
  label: Lone Wolf Deals API
  slug: lone-wolf-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-deals-api-openapi.yml
- filename: lone-wolf-back-office-online-api-openapi.yml
  format: yaml
  label: Lone Wolf Back Office API
  slug: lone-wolf-back-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-back-office-online-api-openapi.yml
- filename: lone-wolf-authentisign-api-openapi.yml
  format: yaml
  label: Lone Wolf Authentisign API
  slug: lone-wolf-authentisign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-authentisign-api-openapi.yml
- filename: lone-wolf-transactiondesk-api-openapi.yml
  format: yaml
  label: Lone Wolf TransactionDesk Partner API
  slug: lone-wolf-transactiondesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-transactiondesk-api-openapi.yml
- filename: lone-wolf-zipform-api-openapi.yml
  format: yaml
  label: Lone Wolf zipForm Partner API
  slug: lone-wolf-zipform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-zipform-api-openapi.yml
- filename: lone-wolf-wolfconnect-api-openapi.yml
  format: yaml
  label: Lone Wolf WolfConnect API
  slug: lone-wolf-wolfconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-wolfconnect-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lone Wolf Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Lone Wolf Technologies secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Lone Wolf Technologies
provider_slug: lone-wolf
scheme_count: 6
schemes:
- bearerFormat: JWT
  description: 'JSON Web Token obtained from the Authentication API (`POST /v1/login`). Pass the token as `Authorization: Bearer <token>` in every request. Tokens expire after the number of seconds specified in the `expiresIn` field of the login response.'
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/lone-wolf-deals-api-openapi.yml
  - openapi/lone-wolf-transact-api-openapi.yml
  - openapi/lone-wolf-transactiondesk-api-openapi.yml
  type: http
- description: API subscription key issued by Lone Wolf, sent on every request.
  in: header
  name: subscriptionKey
  parameter: lw-subscription-key
  sources:
  - openapi/lone-wolf-transact-api-openapi.yml
  type: apiKey
- description: 'Custom HMAC-signed authorization scheme used when calling resources that access your actual data:


    ```

    Authorization: LoneWolfToken [API Token]:[Client Code]:[Signature]:[Date]

    ```


    A `Content-MD5` header is also required on every request (base 64 encoded MD5 hash of the request body, or of an empty string for requests without a body: `1B2M2Y8AsgTpgAmY7PhCfg==`).


    The signature is the HMACSHA256 h'
  in: header
  name: LoneWolfToken
  parameter: Authorization
  sources:
  - openapi/lone-wolf-wolfconnect-api-openapi.yml
  type: apiKey
- description: Context Id obtained from an authentication endpoint. Must be used together with X-Auth-SharedKey.
  in: header
  name: contextAuth
  parameter: X-Auth-ContextId
  sources:
  - openapi/lone-wolf-zipform-api-openapi.yml
  type: apiKey
- description: Shared Key provided by zipLogix to authenticate the partner application.
  in: header
  name: sharedKey
  parameter: X-Auth-SharedKey
  sources:
  - openapi/lone-wolf-zipform-api-openapi.yml
  type: apiKey
- description: External Id for partners authorized to use the External Id authentication scheme. Must be used together with X-Auth-SharedKey.
  in: header
  name: externalIdAuth
  parameter: X-Auth-ExternalId
  sources:
  - openapi/lone-wolf-zipform-api-openapi.yml
  type: apiKey
slug: lone-wolf-authentication
source_filename: lone-wolf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/lone-wolf-deals-api-openapi.yml, openapi/lone-wolf-transact-api-openapi.yml,\n  openapi/lone-wolf-transactiondesk-api-openapi.yml, openapi/lone-wolf-wolfconnect-api-openapi.yml,\n  openapi/lone-wolf-zipform-api-openapi.yml\ndocs:\n- https://apidocs.lwolf.com/doc/transact-api.md#authentication\n- https://apidocs.lwolf.com/doc/deals-api.md#getting-started\n- https://apidocs.lwolf.com/doc/transactiondesk-api.md#authorization\n- https://apidocs.lwolf.com/doc/zipform-api.md#authentication\n- https://apidocs.lwolf.com/doc/wolfconnect-api.md#authentication\n- https://gateway.lwolf.com/.well-known/openid-configuration\noverview: >-\n  Five different authentication models across seven APIs — the clearest evidence that Lone\n  Wolf's API estate is an assembled portfolio rather than one platform. The specs declare six\n  schemes; two definitions (Back Office Online and Authentisign) declare none at all, and the\n  gateway's OAuth\
  \ 2.0 / OIDC layer is published only through the identity discovery document,\n  not through any spec.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  specs_without_security_schemes:\n  - openapi/lone-wolf-back-office-online-api-openapi.yml\n  - openapi/lone-wolf-authentisign-api-openapi.yml\ncredential_issuance:\n  self_service: false\n  process: >-\n    Credentials are issued only after the access-request form at\n    https://www.lwolf.com/api-getting-started is reviewed by the Lone Wolf integrations team.\n    Documentation is fully open; credentials are not.\noauth2:\n  issuer: https://gateway.lwolf.com/\n  platform: Auth0\n  discovery: well-known/lone-wolf-openid-configuration.json\n  token_endpoint: https://gateway.lwolf.com/oauth/token\n  documented_grant: client_credentials\n  documented_token_request:\n    grant_type: client_credentials\n    client_id: <your client id>\n\
  \    client_secret: <your client secret>\n    audience: https://api.lwolf.com\n    lwt_client_id: <your Lone Wolf client GUID>\n  scopes: scopes/lone-wolf-scopes.yml\n  note: >-\n    The Transact API requires BOTH the bearer token and the lw-subscription-key header on every\n    call. A 401 means the token is missing or expired; a 403 means the subscription key is\n    missing or invalid.\nother_endpoints:\n- api: Deals API\n  kind: bespoke login\n  endpoint: POST https://authentication.api.lwolf.com/v1/login\n  request_fields: [emailAddress, password, clientId]\n  response_fields: [token, expiresIn]\n  note: expiresIn is documented as 86400 seconds in the published example.\n- api: TransactionDesk Partner API\n  kind: oauth2\n  authorize: https://api.pre.transactiondesk.com/oauth/authorize\n  token: POST /oauth/token\n  flows: [authorizationCode, clientCredentials]\n  note: >-\n    The authorization code is one-time-use and expires in 10 minutes. The client_credentials\n    flow requires\
  \ an On-Behalf-Of header carrying the target user's GUID.\n- api: zipForm Partner API\n  kind: shared key + session context\n  note: >-\n    X-Auth-SharedKey plus either X-Auth-ContextId or X-Auth-ExternalId; all three may\n    alternatively be supplied on the query string, which is documented explicitly.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JSON Web Token obtained from the Authentication API (`POST /v1/login`). Pass\n    the token as `Authorization: Bearer <token>` in every request. Tokens expire after the number\n    of seconds specified in the `expiresIn` field of the login response.'\n  sources:\n  - openapi/lone-wolf-deals-api-openapi.yml\n  - openapi/lone-wolf-transact-api-openapi.yml\n  - openapi/lone-wolf-transactiondesk-api-openapi.yml\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: lw-subscription-key\n  description: API subscription key issued by Lone Wolf, sent on every request.\n  sources:\n\
  \  - openapi/lone-wolf-transact-api-openapi.yml\n- name: LoneWolfToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Custom HMAC-signed authorization scheme used when calling resources that access your actual data:\n\n    ```\n    Authorization: LoneWolfToken [API Token]:[Client Code]:[Signature]:[Date]\n    ```\n\n    A `Content-MD5` header is also required on every request (base 64 encoded MD5 hash of the request body, or of an empty string for requests without a body: `1B2M2Y8AsgTpgAmY7PhCfg==`).\n\n    The signature is the HMACSHA256 h\n  sources:\n  - openapi/lone-wolf-wolfconnect-api-openapi.yml\n- name: contextAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-ContextId\n  description: Context Id obtained from an authentication endpoint. Must be used together with\n    X-Auth-SharedKey.\n  sources:\n  - openapi/lone-wolf-zipform-api-openapi.yml\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-SharedKey\n  description:\
  \ Shared Key provided by zipLogix to authenticate the partner application.\n  sources:\n  - openapi/lone-wolf-zipform-api-openapi.yml\n- name: externalIdAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-ExternalId\n  description: External Id for partners authorized to use the External Id authentication scheme.\n    Must be used together with X-Auth-SharedKey.\n  sources:\n  - openapi/lone-wolf-zipform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/authentication/lone-wolf-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- Real-Estate
- United States
- PropTech
- Transaction
- Transaction Management
- Brokerage Back Office
- Real Estate Accounting
- Commissions
- Forms
- zipForm
- TransactionDesk
- E-Signature
- CMA
- Valuation
- CRM
- MLS
- Real Estate Agents
- Brokers
---
