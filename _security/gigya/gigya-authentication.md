---
api_key_in:
- query
- body
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gigya Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Gigya secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Gigya
provider_slug: gigya
scheme_count: 2
schemes:
- description: Gigya's classic REST authentication. Every request carries the site `apiKey` plus a credential — an application/user key and secret used to HMAC-SHA1 sign the request (or a `userKey`+`secret` pair, or a session `oauth_token` obtained from socialize.login). Credentials are passed as request parameters (query string or POST body).
  evidence: SAP CDC REST API auth model documented on help.sap.com
  name: gigya-api-key-and-secret
  type: apiKey
- evidence: well-known/gigya-oauth-authorization-server.json
  flow: clientCredentials
  grant_types:
  - client_credentials
  - refresh_token
  introspection_endpoint: https://accounts.us1.gigya.com/introspect
  issuer: https://oauth2.gigya.com
  jwks_uri: https://accounts.us1.gigya.com/oauth2/jwks
  name: gigya-oauth2
  revocation_endpoint: https://accounts.us1.gigya.com/revocation
  token_endpoint: https://accounts.us1.gigya.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  type: oauth2
slug: gigya-authentication
source_filename: gigya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  well-known/gigya-oauth-authorization-server.json (RFC 8414 metadata, fetched\n  200 from https://accounts.us1.gigya.com/.well-known/oauth-authorization-server);\n  SAP Customer Data Cloud (Gigya) REST API documentation on help.sap.com.\ndocs: https://help.sap.com/docs/SAP_CUSTOMER_DATA_CLOUD\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [query, body]\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: gigya-api-key-and-secret\n    type: apiKey\n    description: >-\n      Gigya's classic REST authentication. Every request carries the site\n      `apiKey` plus a credential — an application/user key and secret used to\n      HMAC-SHA1 sign the request (or a `userKey`+`secret` pair, or a session\n      `oauth_token` obtained from socialize.login). Credentials are passed as\n      request parameters (query string or POST body).\n    evidence: SAP CDC REST API auth model documented on help.sap.com\n  - name: gigya-oauth2\n\
  \    type: oauth2\n    flow: clientCredentials\n    issuer: https://oauth2.gigya.com\n    token_endpoint: https://accounts.us1.gigya.com/oauth2/token\n    introspection_endpoint: https://accounts.us1.gigya.com/introspect\n    revocation_endpoint: https://accounts.us1.gigya.com/revocation\n    jwks_uri: https://accounts.us1.gigya.com/oauth2/jwks\n    grant_types: [client_credentials, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post]\n    evidence: well-known/gigya-oauth-authorization-server.json\nnotes: >-\n  Host shown is the US data center (us1); the same endpoints exist per data\n  center (eu1, eu2, au1, cn1, ...) under accounts.{dc}.gigya.com. The RFC 8414\n  metadata advertises no `scopes_supported`, so no OAuth scope reference is\n  captured (see scopes/ — skipped).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigya/refs/heads/main/authentication/gigya-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Identity
- Authentication
- CIAM
- Customer Identity
- OAuth
- Single Sign-On
- Consent Management
- SAP
---
