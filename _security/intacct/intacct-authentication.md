---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Intacct Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- token-exchange
overview: Sage Intacct secures its APIs with oauth2, openIdConnect, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and token-exchange flow(s).
provider_name: Sage Intacct
provider_slug: intacct
scheme_count: 2
schemes:
- authorizationUrl: https://api.intacct.com/ia/authorize
  grant_types:
  - authorization_code
  - client_credentials
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg:
  - RS256
  issuer: https://api.intacct.com
  jwks_uri: https://api.intacct.com/.well-known/jwks.json
  name: OAuth2 / OpenID Connect (REST)
  openIdConnectUrl: https://api.intacct.com/.well-known/openid-configuration
  response_types:
  - code
  - token
  - id_token
  sources:
  - well-known/intacct-openid-configuration.json
  tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: openIdConnect
- description: Sender-level credentials (senderId + senderPassword) authorize the application; a user login (companyId, userId, userPassword) returns a sessionid used on subsequent XML requests. Documented at developer.intacct.com.
  in: body
  name: XML Web Services session (legacy)
  scheme: session-credentials
  sources:
  - https://developer.intacct.com/web-services/
  type: apiKey
slug: intacct-authentication
source_filename: intacct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.intacct.com/.well-known/openid-configuration\ndocs: https://developer.sage.com/intacct/docs/1/sage-intacct-rest-api/api-essentials\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  oauth2_flows: [authorizationCode, clientCredentials, token-exchange]\n  notes: >-\n    The modern REST API authenticates with OAuth 2.0 / OpenID Connect (issuer\n    https://api.intacct.com). The legacy XML Web Services API uses session-based\n    authentication with sender credentials (senderId/senderPassword) plus user\n    login (companyId/userId/userPassword) exchanged for a session id.\nschemes:\n- name: OAuth2 / OpenID Connect (REST)\n  type: openIdConnect\n  openIdConnectUrl: https://api.intacct.com/.well-known/openid-configuration\n  issuer: https://api.intacct.com\n  authorizationUrl: https://api.intacct.com/ia/authorize\n  tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token\n  jwks_uri: https://api.intacct.com/.well-known/jwks.json\n\
  \  grant_types: [authorization_code, client_credentials, urn:ietf:params:oauth:grant-type:token-exchange]\n  response_types: [code, token, id_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt]\n  id_token_signing_alg: [RS256]\n  sources: [well-known/intacct-openid-configuration.json]\n- name: XML Web Services session (legacy)\n  type: apiKey\n  in: body\n  scheme: session-credentials\n  description: >-\n    Sender-level credentials (senderId + senderPassword) authorize the application;\n    a user login (companyId, userId, userPassword) returns a sessionid used on\n    subsequent XML requests. Documented at developer.intacct.com.\n  sources: [https://developer.intacct.com/web-services/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intacct/refs/heads/main/authentication/intacct-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 2 schemes
tags:
- Company
- Accounting
- ERP
- Financial Management
- Cloud Accounting
- Invoicing
- Payments
- SaaS
- REST API
- OAuth
---
