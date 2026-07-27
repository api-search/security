---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Totogi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Totogi secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Totogi
provider_slug: totogi
scheme_count: 3
schemes:
- applies_to:
  - https://gql.produseast1.api.totogi.com/graphql
  - https://gql.prodapsoutheast1.api.totogi.com/graphql
  - https://api.totogi.io/graphql
  authorization_model: named-roles
  client_auth: HTTP Basic (base64 of client_key:client_secret) on the token request
  credential_management:
    note: Tenant clients are minted through the API itself — createClientCredentials, getClientCredentials, listAllClientCredentials, updateClientCredentials and deleteClientCredentials are published GraphQL operations gated on the Tenant_Admin role, and ClientCreationLimitExceeded is a typed error carrying currentClientCount/maxClientLimit.
  evidence:
  - detail: Totogi's own published demo posts grant_type=client_credentials with a Basic-encoded key:secret to https://oauth.totogi.io/oauth2/token and sends the returned access_token as the Authorization header on https://api.totogi.io/graphql.
    source: https://github.com/totogi/marketplace-api-demo
  - detail: '"Access to Totogi APIs is limited to authorized OAuth 2.0 tokens."'
    source: https://www.totogi.com/how-to-guides/build-a-charging-emulator-demo-app-using-totogi-apis/
  flow: clientCredentials
  name: OAuth 2.0 client credentials (Charging-as-a-Service GraphQL)
  probes:
  - body: UnauthorizedException — "Valid authorization header not provided." (AWS AppSync)
    status: 401
    url: https://api.totogi.io/graphql
  - status: 403
    url: https://oauth.totogi.io/.well-known/openid-configuration
  - status: 403
    url: https://oauth.totogi.io/.well-known/oauth-authorization-server
  roles_artifact: scopes/totogi-scopes.yml
  token_url: https://oauth.totogi.io/oauth2/token
  type: oauth2
- applies_to:
  - https://5g.produseast1.api.totogi.com/nchf-convergedcharging/v3/chargingData
  - https://5g.prodapsoutheast1.api.totogi.com/nchf-convergedcharging/v3/chargingData
  bearer_format: JWT id token
  evidence:
  - detail: 'Totogi''s published proxy forwards charging requests over HTTP/2 with Authorization: Bearer <idToken> and hard-allowlists the two 3GPP Nchf endpoints above.'
    source: https://github.com/totogi/totogi-charging-proxy
  name: Bearer id token (5G converged charging)
  probes:
  - status: 403
    url: https://5g.produseast1.api.totogi.com
  - status: 403
    url: https://5g.prodapsoutheast1.api.totogi.com
  scheme: bearer
  type: http
- applies_to:
  - https://api.whoosh.totogi.solutions/2010-04-01/Accounts/{AccountSid}/Messages.json
  evidence:
  - detail: The published curl quickstart authenticates with -u $TWILIO_ACCOUNT_SID:$TWILIO_AUTH_TOKEN. The Twilio credential model is reproduced exactly, down to the environment-variable names every Whoosh SDK reads.
    source: https://docs.whoosh.totogi.solutions/send_message
  issued_from: https://console.whoosh.totogi.solutions
  name: HTTP Basic — Account SID and Auth Token (Whoosh messaging)
  note: There is no self-serve signup; credentials are issued by Totogi through the operator.
  password: AuthToken
  scheme: basic
  type: http
  username: AccountSid
slug: totogi-authentication
source_filename: totogi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://docs.api.totogi.com/\ndocs: https://docs.api.totogi.com/\nnote: >-\n  Totogi has no single authentication model — it runs three separate credential systems across\n  three separate API surfaces, and none of them share an issuer. Derived mechanically where a\n  spec existed and read from Totogi's own published documentation and demo code everywhere else.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer, basic]\n  openid_connect: false\n  mutual_tls: false\n  discovery_documents: none\nschemes:\n- name: OAuth 2.0 client credentials (Charging-as-a-Service GraphQL)\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://oauth.totogi.io/oauth2/token\n  client_auth: HTTP Basic (base64 of client_key:client_secret) on the token request\n  applies_to:\n  - https://gql.produseast1.api.totogi.com/graphql\n  - https://gql.prodapsoutheast1.api.totogi.com/graphql\n\
  \  - https://api.totogi.io/graphql\n  authorization_model: named-roles\n  roles_artifact: scopes/totogi-scopes.yml\n  credential_management:\n    note: >-\n      Tenant clients are minted through the API itself — createClientCredentials,\n      getClientCredentials, listAllClientCredentials, updateClientCredentials and\n      deleteClientCredentials are published GraphQL operations gated on the Tenant_Admin role,\n      and ClientCreationLimitExceeded is a typed error carrying currentClientCount/maxClientLimit.\n  evidence:\n  - source: https://github.com/totogi/marketplace-api-demo\n    detail: >-\n      Totogi's own published demo posts grant_type=client_credentials with a Basic-encoded\n      key:secret to https://oauth.totogi.io/oauth2/token and sends the returned access_token\n      as the Authorization header on https://api.totogi.io/graphql.\n  - source: https://www.totogi.com/how-to-guides/build-a-charging-emulator-demo-app-using-totogi-apis/\n    detail: '\"Access to Totogi APIs\
  \ is limited to authorized OAuth 2.0 tokens.\"'\n  probes:\n  - {url: 'https://api.totogi.io/graphql', status: 401, body: 'UnauthorizedException — \"Valid authorization header not provided.\" (AWS AppSync)'}\n  - {url: 'https://oauth.totogi.io/.well-known/openid-configuration', status: 403}\n  - {url: 'https://oauth.totogi.io/.well-known/oauth-authorization-server', status: 403}\n- name: Bearer id token (5G converged charging)\n  type: http\n  scheme: bearer\n  bearer_format: JWT id token\n  applies_to:\n  - https://5g.produseast1.api.totogi.com/nchf-convergedcharging/v3/chargingData\n  - https://5g.prodapsoutheast1.api.totogi.com/nchf-convergedcharging/v3/chargingData\n  evidence:\n  - source: https://github.com/totogi/totogi-charging-proxy\n    detail: >-\n      Totogi's published proxy forwards charging requests over HTTP/2 with\n      Authorization: Bearer <idToken> and hard-allowlists the two 3GPP Nchf endpoints above.\n  probes:\n  - {url: 'https://5g.produseast1.api.totogi.com',\
  \ status: 403}\n  - {url: 'https://5g.prodapsoutheast1.api.totogi.com', status: 403}\n- name: HTTP Basic — Account SID and Auth Token (Whoosh messaging)\n  type: http\n  scheme: basic\n  username: AccountSid\n  password: AuthToken\n  applies_to:\n  - https://api.whoosh.totogi.solutions/2010-04-01/Accounts/{AccountSid}/Messages.json\n  issued_from: https://console.whoosh.totogi.solutions\n  evidence:\n  - source: https://docs.whoosh.totogi.solutions/send_message\n    detail: >-\n      The published curl quickstart authenticates with -u $TWILIO_ACCOUNT_SID:$TWILIO_AUTH_TOKEN.\n      The Twilio credential model is reproduced exactly, down to the environment-variable names\n      every Whoosh SDK reads.\n  note: There is no self-serve signup; credentials are issued by Totogi through the operator.\ngaps:\n- No OpenID Connect discovery document is published on any host.\n- No mutual-TLS, no API-key-in-header scheme, and no signed-request scheme is documented.\n- >-\n  The OAuth authorization-server\
  \ metadata is unreachable anonymously (403), so token lifetime,\n  supported grants and the canonical scope list cannot be verified without a tenant credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/totogi/refs/heads/main/authentication/totogi-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Telecommunications
- United States
- BSS
- OSS
- Charging
- Messaging
- SMS
- A2P
- 5G
- TM Forum
- Standards
- Network Vendor
- Vertical AI
- GraphQL
- Policy Control
---
