---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Thredd Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Thredd secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Thredd
provider_slug: thredd
scheme_count: 3
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: oauth2ClientCredentials
  request_fields:
  - client_id
  - client_secret
  - grant_type
  source: docs
  token_content_type: application/x-www-form-urlencoded
  token_format: JWT
  token_type: Bearer
  token_url: https://oauthuat.globalprocessing.net/connect/token
  type: oauth2
- broker: Cloudentity
  certificate_authority: Raidiam Connect
  client_authentication: private_key_jwt
  name: privateKeyJwt
  profile: FAPI
  source: docs
  transport: mutual-tls
  type: oauth2
- bearer_format: JWT
  header: Authorization
  name: bearerAuth
  scheme: bearer
  source: docs
  type: http
slug: thredd-authentication
source_filename: thredd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://cardsapidocs.thredd.com/docs/get-an-authentication-token\ndocs: https://cardsapidocs.thredd.com/v2.0/docs/get-an-authentication-token\nsummary:\n  types: [oauth2, mutualTLS]\n  oauth2_flows: [clientCredentials]\n  bearer: true\n  notes: >-\n    Thredd Cards API (API Hub) uses FAPI-grade OAuth2 client-credentials.\n    Clients authenticate with a client_id + client_secret to a token endpoint\n    and present the returned Bearer access token on every request. Production /\n    high-assurance access adds private_key_jwt client assertions over mutual TLS,\n    brokered by Cloudentity with Raidiam Connect acting as the certificate\n    authority. Documented example uses the UAT token endpoint.\nschemes:\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    grant_type: client_credentials\n    token_url: https://oauthuat.globalprocessing.net/connect/token\n    token_content_type: application/x-www-form-urlencoded\n\
  \    request_fields: [client_id, client_secret, grant_type]\n    token_type: Bearer\n    token_format: JWT\n    source: docs\n  - name: privateKeyJwt\n    type: oauth2\n    client_authentication: private_key_jwt\n    transport: mutual-tls\n    broker: Cloudentity\n    certificate_authority: Raidiam Connect\n    profile: FAPI\n    source: docs\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    header: Authorization\n    source: docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thredd/refs/heads/main/authentication/thredd-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Payments
- United Kingdom
- Issuer Processor
- Card Issuing
- Payment Processing
- Banking-as-a-Service
- Digital Wallet
- Cross-Border
- Fraud
- Open Banking
- FAPI
---
