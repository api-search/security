---
api_key_in: []
auth_types: []
description: 'Logiwa authenticates the Integration API with an OAuth 2.0 Resource Owner Password Credentials grant against a per-tenant token host, returning a bearer access token that is then sent on every Integration API call. Credentials are not self-service: the docs state an API user must be provisioned by Logiwa under a sales contract before any token can be issued.'
kind: authentication
layout: security
method: searched
name: Logiwa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Logiwa declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Logiwa
provider_slug: logiwa
scheme_count: 2
schemes:
- applied_to: All /en/api/IntegrationApi/* operations
  description: Bearer access token obtained from the tenant token endpoint. All Integration API requests must carry it.
  in: header
  key: logiwaBearer
  scheme: bearer
  type: http
- description: Documented OAuth 2.0 password grant. The docs' sample response shows token_type "bearer" and a .issued/.expires pair two weeks apart; the Getting Started page states access tokens "generally" last two weeks and that clients must refresh before expiry.
  flow: password
  key: logiwaPasswordGrant
  request_content_type: application/x-www-form-urlencoded
  request_parameters:
  - name: grant_type
    required: true
    value: password
  - description: Logiwa API user name provisioned by Logiwa
    name: username
    required: true
  - description: Logiwa API user password
    name: password
    required: true
  response_fields:
  - access_token
  - token_type
  - username
  - expires_in
  - .issued
  - .expires
  token_url_examples:
  - https://appapi.logiwa.com/token
  - https://wmsapi.logiwa.com/token
  token_url_pattern: https://{environment}api.logiwa.com/token
  type: oauth2
slug: logiwa-authentication
source_filename: logiwa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://developer.logiwa.com/?id=5df0da39e6466c2eec992f3f\ndocs: https://developer.logiwa.com/?id=5df0da39e6466c2eec992f3f\nname: Logiwa Integration API authentication\ndescription: >-\n  Logiwa authenticates the Integration API with an OAuth 2.0 Resource Owner Password Credentials\n  grant against a per-tenant token host, returning a bearer access token that is then sent on\n  every Integration API call. Credentials are not self-service: the docs state an API user must\n  be provisioned by Logiwa under a sales contract before any token can be issued.\nschemes:\n- key: logiwaBearer\n  type: http\n  scheme: bearer\n  in: header\n  description: >-\n    Bearer access token obtained from the tenant token endpoint. All Integration API requests\n    must carry it.\n  applied_to: All /en/api/IntegrationApi/* operations\n- key: logiwaPasswordGrant\n  type: oauth2\n  flow: password\n  token_url_pattern: https://{environment}api.logiwa.com/token\n\
  \  token_url_examples:\n  - https://appapi.logiwa.com/token\n  - https://wmsapi.logiwa.com/token\n  request_content_type: application/x-www-form-urlencoded\n  request_parameters:\n  - name: grant_type\n    value: password\n    required: true\n  - name: username\n    description: Logiwa API user name provisioned by Logiwa\n    required: true\n  - name: password\n    description: Logiwa API user password\n    required: true\n  response_fields:\n  - access_token\n  - token_type\n  - username\n  - expires_in\n  - .issued\n  - .expires\n  description: >-\n    Documented OAuth 2.0 password grant. The docs' sample response shows token_type \"bearer\" and\n    a .issued/.expires pair two weeks apart; the Getting Started page states access tokens\n    \"generally\" last two weeks and that clients must refresh before expiry.\ntoken_host_pattern: >-\n  The token host mirrors the tenant application host: [yourenvironment].logiwa.com pairs with\n  [yourenvironment]api.logiwa.com/token. Documented examples:\
  \ wms.logiwa.com -> wmsapi.logiwa.com/token,\n  app.logiwa.com -> appapi.logiwa.com/token.\noidc_discovery:\n  served: true\n  urls:\n  - https://appapi.logiwa.com/.well-known/openid-configuration\n  - https://wmsapi.logiwa.com/.well-known/openid-configuration\n  issuer: Ocelot\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, implicit, 'urn:ietf:params:oauth:grant-type:device_code']\n  scopes_supported: [admin, openid, offline_access]\n  code_challenge_methods_supported: [plain, S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  note: >-\n    The gateway also publishes a full OIDC discovery document advertising authorization_code,\n    client_credentials, refresh_token, implicit and device_code grants at /connect/*. None of\n    those flows are described anywhere in the public developer documentation, which documents\n    only the password grant against /token. Recorded as observed gateway capability, not as a\n\
  \    documented integration path.\nfindings:\n- id: oidc-endpoints-advertise-http\n  severity: high\n  detail: >-\n    Every endpoint in the served OIDC discovery document uses the http:// scheme\n    (http://appapi.logiwa.com/connect/token, .../authorize, .../introspect, .../userinfo), not\n    https://. A client that follows discovery literally would negotiate tokens in cleartext.\n  evidence: well-known/logiwa-appapi-openid-configuration.json\n- id: oidc-issuer-not-a-url\n  severity: medium\n  detail: >-\n    issuer is the literal string \"Ocelot\" (the .NET API gateway product name) rather than an\n    https URL, which fails the OpenID Connect Discovery 1.0 requirement that issuer be a\n    URL using the https scheme. Issuer validation in a conformant OIDC client will reject it.\n  evidence: well-known/logiwa-appapi-openid-configuration.json\n- id: password-grant-only\n  severity: medium\n  detail: >-\n    The only documented flow is the OAuth 2.0 password grant, which OAuth 2.1 deprecates.\
  \ It\n    requires the integrator to store a Logiwa user's username and password. There is no\n    documented API-key, client-credentials or per-integration credential path.\n  evidence: https://developer.logiwa.com/?id=5df0da39e6466c2eec992f3f\n- id: no-self-service-credentials\n  severity: medium\n  detail: >-\n    Getting Started states an integrator must contact a sales representative or customer success\n    manager, add API users to a sales contract, and wait for customer support to provision them.\n    No sign-up, sandbox key or trial credential is published.\n  evidence: https://developer.logiwa.com/?id=5df0d8bfe6466c2eec992f31\nauthorization_model: >-\n  \"The data this API user can access is based on the permissions given to them in Logiwa, such as\n  the Roles, Warehouses, and Clients they're affiliated with.\" Authorization is therefore carried\n  entirely by the provisioned user's role/warehouse/depositor affiliations, not by token scopes.\nerrors:\n- condition: bad username\
  \ or password\n  body: '{\"error\": \"invalid_grant\", \"error_description\": \"The user name or password is incorrect.\"}'\n- condition: missing username\n  body: '{\"expires_in\":0,\".error\":\"invalid_grant\",\".error_description\":\"Username cannot be empty.\"}'\n  observed: 'POST https://appapi.logiwa.com/token 2026-08-25, HTTP 200'\n- condition: expired or invalid bearer token\n  body: '{\"Message\": \"Authorization has been denied for this request.\"}'\n  observed: 'POST https://app.logiwa.com/en/api/IntegrationApi/LookUp 2026-08-25, HTTP 401'\nx-evidence:\n  fetched: '2026-08-25'\n  probes:\n  - url: https://appapi.logiwa.com/token\n    method: POST\n    http_status: 200\n    note: Live; returned the documented invalid_grant envelope for an empty username.\n  - url: https://app.logiwa.com/en/api/IntegrationApi/LookUp\n    method: POST\n    http_status: 401\n    note: Live; returned the documented \"Authorization has been denied for this request.\" envelope.\n  - url: https://appapi.logiwa.com/.well-known/openid-configuration\n\
  \    method: GET\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiwa/refs/heads/main/authentication/logiwa-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Warehouse Management
- Fulfillment
- Logistics
- Supply Chain
- Inventory Management
- Order Management
- Third Party Logistics
- E-Commerce
- Shipping
- Webhook
- Software-as-a-Service
---
