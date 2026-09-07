---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Wavebl Authentication
name_suffix: Authentication
oauth_flows: []
overview: WaveBL declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: WaveBL
provider_slug: wavebl
scheme_count: 0
schemes: []
slug: wavebl-authentication
source_filename: wavebl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  WaveBL's own production login bundle\n  (https://ib.prod.wavebl.com/static/js/main.92f24860.chunk.js), the OpenID Connect discovery\n  document served at https://wsupport.wavebl.com/.well-known/openid-configuration, and anonymous\n  probes of the WaveBL API Gateway hosts on 2026-09-04.\nsummary: >-\n  WaveBL documents no API authentication anywhere. There is no OpenAPI to derive securitySchemes\n  from and no auth page on any public property. What can be established anonymously is the identity\n  machinery behind WaveBL's own web properties, recorded below as observed fact rather than as a\n  documented API contract.\napi_authentication:\n  documented: false\n  schemes: []\n  note: >-\n    No API key, token, OAuth flow, mTLS profile or signing scheme is published for any WaveBL API.\n    The one reachable API surface, https://coa.wavebl.com/coadocuments/*, rejects anonymous GET and\n    OPTIONS with HTTP 403 {\"message\"\
  :\"Missing Authentication Token\"} — the AWS API Gateway response\n    for an undefined method, which carries no WWW-Authenticate challenge, so even the scheme cannot\n    be inferred from the outside. Partner integrations against the DCSA eBL Issuance and Surrender\n    Response APIs are provisioned through WaveBL sales and support; no credential-issuance\n    documentation is public.\nobserved_identity_surfaces:\n- surface: WaveBL platform login (ib.prod.wavebl.com)\n  type: oauth2\n  flow: authorization_code\n  provider: Amazon Cognito user pools via the AWS Amplify Identity Broker\n  region: eu-west-1\n  hosted_ui_domain: wave-identity-broker-prod.auth.eu-west-1.amazoncognito.com\n  scopes:\n  - phone\n  - email\n  - openid\n  - profile\n  - aws.cognito.signin.user.admin\n  username_attribute: email\n  mfa: optional\n  mfa_types:\n  - SMS\n  - TOTP\n  password_min_length: 8\n  evidence:\n  - url: https://ib.prod.wavebl.com/\n    status: 200\n    note: >-\n      Page title \"WaveBL\
  \ Login\". Its production bundle carries the Amplify configuration block\n      naming the Cognito region, the identity-broker API endpoint, the hosted-UI domain, the OAuth\n      scope set, responseType \"code\" and the MFA/password policy quoted above. Client and pool\n      identifiers are deliberately NOT recorded here.\n  - url: https://wave-identity-broker-prod.auth.eu-west-1.amazoncognito.com/oauth2/authorize\n    status: 400\n    note: >-\n      Live Cognito hosted UI — a bare authorize request without client_id returns the Cognito error\n      page, confirming the authorization server exists.\n  - url: https://wave-identity-broker-prod.auth.eu-west-1.amazoncognito.com/.well-known/openid-configuration\n    status: 404\n    note: >-\n      Cognito hosted-UI domains do not publish discovery; the pool's OIDC metadata is served by AWS\n      at cognito-idp.eu-west-1.amazonaws.com (HTTP 200), not by WaveBL.\n- surface: WaveBL support community (wsupport.wavebl.com)\n  type: openIdConnect\n\
  \  provider: Salesforce Experience Cloud\n  discovery: https://wsupport.wavebl.com/.well-known/openid-configuration\n  issuer: https://wsupport.wavebl.com\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  id_token_signing_alg: RS256\n  dynamic_registration: true\n  evidence:\n  - url: https://wsupport.wavebl.com/.well-known/openid-configuration\n    status: 200\n    note: >-\n      Full OIDC discovery document saved verbatim to\n      well-known/wavebl-wsupport-openid-configuration.json. This is the support portal's identity\n      surface, not an API authorization server for the eBL platform.\n- surface: WaveBL API Gateway hosts\n  type: unknown\n  evidence:\n  - url: https://coa.wavebl.com/coadocuments/search\n    status: 403\n  - url: https://prod-registration.api.wavebl.com/\n    status: 403\n  - url: https://prod-logingate.api.wavebl.com/\n    status: 403\n  - url: https://prod-coa.api.wavebl.com/\n    status: 403\n  - url: https://wave-ai-staging.rnd.wavebl.com/openapi.json\n\
  \    status: 403\n  note: >-\n    Every one answers {\"message\":\"Missing Authentication Token\"} with no WWW-Authenticate header.\n    AWS API Gateway returns this identically for an unauthenticated request and for a method that\n    does not exist, so it establishes only that the hosts are live API Gateways.\nscopes:\n  documented: false\n  note: >-\n    No OAuth scope reference is published for any WaveBL API. The Cognito scope set recorded above\n    is the sign-in scope set for the platform's own web client, not an API permission model, so no\n    scopes/ artifact is written and no OAuthScopes pointer is emitted.\npointer_policy: >-\n  An Authentication pointer IS emitted against this file, because it records a real, evidenced\n  authentication posture measured from WaveBL's own production surface. It should not be read as\n  WaveBL having documented API authentication — it has not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wavebl/refs/heads/main/authentication/wavebl-authentication.yml
summary_line: 0 schemes
tags:
- Electronic Bill of Lading
- Digital Trade
- Trade Documents
- Trade Finance
- Ocean Freight
- Shipping
- Logistics
- Supply Chain
- Maritime
- Customs
- Blockchain
- Freight Forwarding
- Banking
- Document Exchange
---
