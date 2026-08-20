---
api_key_in: []
api_specs:
- filename: realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Web API
  slug: realtor-ca-ddf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-ddf-web-api-openapi.json
- filename: realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Lead API
  slug: realtor-ca-ddf-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-ddf-web-api-openapi.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Realtor Ca Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: REALTOR.ca secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: REALTOR.ca
provider_slug: realtor-ca
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes:
      DDFApi_Read: Read access to the DDF Web API resources entitled to the Destination feed.
    tokenUrl: https://identity.crea.ca/connect/token
  name: DDFApiOAuth2
  note: 'CREA states the token is not sliding — a new token must be requested every hour regardless of activity. CREA also recommends server-to-server token use only: "Client-to-server API token requests create a security risk and could allow unauthorized access to your data feeds."'
  request:
    content_type: application/x-www-form-urlencoded
    fields:
      client_id: The username of your DDF Destination (data feed).
      client_secret: The password of your DDF Destination (data feed).
      grant_type: client_credentials
      scope: DDFApi_Read
    method: POST
  response:
    access_token: The bearer token value.
    expires_in: 3600
    scope: DDFApi_Read
    token_type: Bearer
  sliding: false
  source: https://ddfapi-docs.realtor.ca/#section/Authorization
  token_lifetime_seconds: 3600
  type: oauth2
- applies_to:
  - https://ddfapi.realtor.ca/odata/v1
  - https://ddfapi.realtor.ca/v1
  name: BearerAuth
  note: 'Every DDF Web API and Lead API request carries `Authorization: Bearer {access_token}`. Anonymous requests — including to the OData $metadata document — return HTTP 401 with `WWW-Authenticate: Bearer`.'
  scheme: bearer
  source: https://ddfapi-docs.realtor.ca/#section/Authorization
  type: http
slug: realtor-ca-authentication
source_filename: realtor-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://identity.crea.ca/.well-known/openid-configuration (HTTP 200, harvested verbatim) and the\n  \"Authorization\" / \"API Access Tokens\" sections of the DDF Web API documentation at\n  https://ddfapi-docs.realtor.ca/\ndocs: https://ddfapi-docs.realtor.ca/#section/Authorization\nnote: >-\n  DERIVATION FAILED BY DESIGN: neither harvested OpenAPI declares a `components.securitySchemes`\n  block and neither declares `security` on any operation, even though every endpoint returns HTTP\n  401 without a Bearer token. The auth model below is SEARCHED from CREA's own documentation and\n  from the anonymously-readable OpenID Connect discovery document, not derived from the spec. This\n  gap is captured as an enhancement in overlays/.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer]\n  spec_declares_security: false\nschemes:\n- name: DDFApiOAuth2\n  type: oauth2\n\
  \  source: https://ddfapi-docs.realtor.ca/#section/Authorization\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.crea.ca/connect/token\n    scopes:\n      DDFApi_Read: Read access to the DDF Web API resources entitled to the Destination feed.\n  request:\n    method: POST\n    content_type: application/x-www-form-urlencoded\n    fields:\n      client_id: The username of your DDF Destination (data feed).\n      client_secret: The password of your DDF Destination (data feed).\n      grant_type: client_credentials\n      scope: DDFApi_Read\n  response:\n    access_token: The bearer token value.\n    expires_in: 3600\n    token_type: Bearer\n    scope: DDFApi_Read\n  token_lifetime_seconds: 3600\n  sliding: false\n  note: >-\n    CREA states the token is not sliding — a new token must be requested every hour regardless of\n    activity. CREA also recommends server-to-server token use only: \"Client-to-server API token\n    requests create a security risk and could allow\
  \ unauthorized access to your data feeds.\"\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  source: https://ddfapi-docs.realtor.ca/#section/Authorization\n  applies_to:\n  - https://ddfapi.realtor.ca/odata/v1\n  - https://ddfapi.realtor.ca/v1\n  note: >-\n    Every DDF Web API and Lead API request carries `Authorization: Bearer {access_token}`.\n    Anonymous requests — including to the OData $metadata document — return HTTP 401 with\n    `WWW-Authenticate: Bearer`.\nauthorization_servers:\n- issuer: https://identity.crea.ca\n  role: The developer/API gate. Issues every DDF Web API access token.\n  vendor: Duende/IdentityServer\n  discovery: https://identity.crea.ca/.well-known/openid-configuration\n  harvested: authentication/realtor-ca-crea-identity-openid-configuration.json\n  authorization_endpoint: https://identity.crea.ca/connect/authorize\n  token_endpoint: https://identity.crea.ca/connect/token\n  introspection_endpoint: https://identity.crea.ca/connect/introspect\n  revocation_endpoint:\
  \ https://identity.crea.ca/connect/revocation\n  userinfo_endpoint: https://identity.crea.ca/connect/userinfo\n  jwks_uri: https://identity.crea.ca/.well-known/openid-configuration/jwks\n  pushed_authorization_request_endpoint: https://identity.crea.ca/connect/par\n  require_pushed_authorization_requests: false\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:openid:params:grant-type:ciba'\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  code_challenge_methods: [plain, S256]\n  dpop_supported: true\n  dpop_signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512]\n  claims_supported: [sub, destinationid]\n  note: >-\n    The `destinationid` claim is the entitlement carrier — a token is scoped to the member-\n    registered Destination feed whose credentials minted it, not to a developer account.\n\
  - issuer: https://auth.realtor.ca/\n  role: >-\n    Human sign-in for REALTOR.ca / ddf.realtor.ca members and consumers. NOT a developer API gate —\n    no DDF Web API token can be obtained here.\n  vendor: Auth0\n  discovery: https://auth.realtor.ca/.well-known/openid-configuration\n  harvested: authentication/realtor-ca-auth0-openid-configuration.json\n  token_endpoint: https://auth.realtor.ca/oauth/token\n  jwks_uri: https://auth.realtor.ca/.well-known/jwks.json\n  rfc8414_metadata: https://auth.realtor.ca/.well-known/oauth-authorization-server\n  mfa_challenge_endpoint: https://auth.realtor.ca/mfa/challenge\n  dpop_supported: true\n  dpop_signing_algs: [ES256]\ncredential_issuance:\n  self_serve: false\n  sandbox: false\n  gate: >-\n    A licensed REALTOR or broker owner must create a DDF Destination (data feed) in the member\n    portal at https://member.realtor.ca/Distribution/Default.aspx and link it to the integrator.\n    The credential you receive is the FEED's username/password,\
  \ not a developer key. A Technology\n    Provider enumerates the feeds linked to it by querying GET /odata/v1/Destination.\ntransport_security:\n  min_tls: '1.2'\n  https_only: true\n  source: >-\n    DDF Web API release notes, January 31st 2023 — \"Update to support minimum TLS version 1.2\n    enforcing all incoming requests to be HTTPS.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/authentication/realtor-ca-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- RESO
- IDX
- Listing Syndication
- PropTech
- OData
- Rentals
---
