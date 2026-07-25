---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Great West Lifeco Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Great-West Lifeco secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Great-West Lifeco
provider_slug: great-west-lifeco
scheme_count: 3
schemes:
- description: '"The API key is used to protect the Empower API from unauthorized access. When your application makes a request to the API, the API key must be supplied as a request header named x-api-key with the value of the API key delivered." The key is delivered by secure email after an access request is reviewed and approved. The OAuth 2.0 API release notes additionally state that the /token and /auth endpoints accept an optional x-api-key header.'
  entity: Empower (U.S. retirement subsidiary)
  in: header
  name: EmpowerApiKey
  parameter_name: x-api-key
  source: https://developer.empower.com/docs/get-started
  type: apiKey
- client_authentication:
  - method: client_secret_basic
    note: '"Using Type of Basic Auth, set client_credentials as grant_type, Username set to your received Client ID, and Password set to your received Client secret value. This call will return a bearer access token." Retained only for read-only APIs, on individual request and after security review.'
    status: legacy
  - method: private_key_jwt
    note: '"Starting Q4 2024 - in support of higher API security required for Financial-grade APIs (FAPI), Empower APIs will be requiring the use asymmetric (public-key based) method ... for client authentication method." Empower states OAuth2 and OpenID Connect are used to protect its APIs, and that asymmetric client authentication means the Empower Authorization Server does not need to store sensitive symmetric keys.'
    since: 2024-Q4
    status: required
  entity: Empower (U.S. retirement subsidiary)
  flows:
  - flow: clientCredentials
    note: The authorization service endpoint is not published; it is communicated privately to approved partners together with the Client ID and Client Secret by secure email. The public OAuth 2.0 API catalog entry documents /auth and /token endpoint paths but not their host.
    tokenUrl: null
  name: EmpowerOAuth2ClientCredentials
  source: https://developer.empower.com/docs/additional-security-protocols-publicprivate-key-infrastructure-pki
  token_usage: Bearer access token supplied as the value of the Authorization request header.
  type: oauth2
- endpoints:
    authorization: https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED
    jwks: https://api.canadalife.com/oauth2/v1/jwks
    revocation: https://api.canadalife.com/oauth2/v1/revoke
    token: https://api.canadalife.com/oauth2/v1/generate
    userinfo: https://api.canadalife.com/oauth2/v1/userinfo
  entity: Canada Life (Canadian operating brand)
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.canadalife.com
  name: CanadaLifeGatewayOIDC
  note: The authorization_endpoint value is published literally as "https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED", i.e. the interactive authorization-code redirect is deliberately disabled and the gateway is machine-to-machine only. scopes_supported is an empty array, so scope names are provisioned per client rather than advertised. Anonymous calls to protected paths return an Apigee error naming the "Consumer-Key", confirming an Apigee-fronted gateway. jwks_uri returns live RSA keys anonymously (HTTP 200).
  openIdConnectUrl: https://api.canadalife.com/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  scopes_supported: []
  source: well-known/great-west-lifeco-openid-configuration.json
  subject_types_supported: public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - client_secret_jwt
  type: openIdConnect
slug: great-west-lifeco-authentication
source_filename: great-west-lifeco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://developer.empower.com/docs/get-started;\n  https://developer.empower.com/docs/additional-security-protocols-publicprivate-key-infrastructure-pki;\n  https://developer.empower.com/api-catalog/oauth2-api;\n  https://www.empower.com/financial-professionals/experience/apis;\n  https://api.canadalife.com/.well-known/openid-configuration (HTTP 200)\ndocs: https://developer.empower.com/docs/get-started\nnote: >-\n  Great-West Lifeco has no group-wide auth model. Two independent, unrelated\n  authorization surfaces exist inside the group and are recorded separately:\n  Empower (U.S. retirement) documents its model in prose on a public developer\n  portal but issues credentials only after an approved access request, and\n  Canada Life (Canada) publishes no documentation at all but does serve a live\n  OpenID Connect discovery document on its production API gateway. No OpenAPI\n  securitySchemes exist anywhere in the group,\
  \ so nothing here is derived from\n  a spec; every field below was read off a public page or a live probe.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  api_key_names: [x-api-key]\n  oauth2_flows: [clientCredentials]\n  client_authentication: [client_secret_basic, private_key_jwt, client_secret_post, client_secret_jwt]\n  self_serve_credentials: false\n  fapi_alignment: claimed\nschemes:\n- name: EmpowerApiKey\n  entity: Empower (U.S. retirement subsidiary)\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  source: https://developer.empower.com/docs/get-started\n  description: >-\n    \"The API key is used to protect the Empower API from unauthorized access.\n    When your application makes a request to the API, the API key must be\n    supplied as a request header named x-api-key with the value of the API key\n    delivered.\" The key is delivered by secure email after an access request is\n    reviewed and approved. The OAuth 2.0 API release\
  \ notes additionally state\n    that the /token and /auth endpoints accept an optional x-api-key header.\n- name: EmpowerOAuth2ClientCredentials\n  entity: Empower (U.S. retirement subsidiary)\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    note: >-\n      The authorization service endpoint is not published; it is communicated\n      privately to approved partners together with the Client ID and Client\n      Secret by secure email. The public OAuth 2.0 API catalog entry documents\n      /auth and /token endpoint paths but not their host.\n  client_authentication:\n  - method: client_secret_basic\n    status: legacy\n    note: >-\n      \"Using Type of Basic Auth, set client_credentials as grant_type, Username\n      set to your received Client ID, and Password set to your received Client\n      secret value. This call will return a bearer access token.\" Retained only\n      for read-only APIs, on individual request and after security review.\n  - method:\
  \ private_key_jwt\n    status: required\n    since: '2024-Q4'\n    note: >-\n      \"Starting Q4 2024 - in support of higher API security required for\n      Financial-grade APIs (FAPI), Empower APIs will be requiring the use\n      asymmetric (public-key based) method ... for client authentication\n      method.\" Empower states OAuth2 and OpenID Connect are used to protect its\n      APIs, and that asymmetric client authentication means the Empower\n      Authorization Server does not need to store sensitive symmetric keys.\n  token_usage: >-\n    Bearer access token supplied as the value of the Authorization request\n    header.\n  source: https://developer.empower.com/docs/additional-security-protocols-publicprivate-key-infrastructure-pki\n- name: CanadaLifeGatewayOIDC\n  entity: Canada Life (Canadian operating brand)\n  type: openIdConnect\n  openIdConnectUrl: https://api.canadalife.com/.well-known/openid-configuration\n  issuer: https://api.canadalife.com\n  source: well-known/great-west-lifeco-openid-configuration.json\n\
  \  endpoints:\n    token: https://api.canadalife.com/oauth2/v1/generate\n    jwks: https://api.canadalife.com/oauth2/v1/jwks\n    revocation: https://api.canadalife.com/oauth2/v1/revoke\n    userinfo: https://api.canadalife.com/oauth2/v1/userinfo\n    authorization: https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED\n  response_types_supported: [code, token]\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - client_secret_jwt\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: public\n  scopes_supported: []\n  note: >-\n    The authorization_endpoint value is published literally as\n    \"https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED\", i.e. the\n    interactive authorization-code redirect is deliberately disabled and the\n    gateway is machine-to-machine only. scopes_supported is an empty array, so\n    scope names are provisioned per client rather than advertised. Anonymous\n    calls to\
  \ protected paths return an Apigee error naming the \"Consumer-Key\",\n    confirming an Apigee-fronted gateway. jwks_uri returns live RSA keys\n    anonymously (HTTP 200).\ngated:\n  credentials_issued_by: >-\n    Empower: portal registration, then a \"Get Access\" request per API, reviewed\n    and approved, after which API Key, Client ID, Client Secret (or PKI\n    onboarding documentation) and the authorization service endpoint arrive by\n    secure email. Canada Life: no public request path at all - the gateway\n    error envelope points to https://apimarketplace.canadalife.com, a\n    digitalML-hosted API marketplace that does not resolve publicly.\n  reference_documentation: >-\n    Every Empower API reference page states \"To see the reference\n    documentation, please login\". No endpoint list, base URL or specification\n    is retrievable anonymously anywhere in the group.\nb2c:\n  supported: contact-required\n  note: '\"Contact us to discuss a B2C scenario.\" - Empower Get\
  \ started guide.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/great-west-lifeco/refs/heads/main/authentication/great-west-lifeco-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Retirement
- Wealth Management
- Reinsurance
- Annuities
- Partner Gated
---
