---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Redaptive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- tokenExchange
- refreshToken
overview: Redaptive secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, tokenExchange, and refreshToken flow(s).
provider_name: Redaptive
provider_slug: redaptive
scheme_count: 2
schemes:
- client_authentication:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  endpoints:
    introspection_endpoint: https://core-api.redaptiveinc.com/oauth2/introspect
    jwks_uri: https://core-api.redaptiveinc.com/oauth2/jwks
    revocation_endpoint: https://core-api.redaptiveinc.com/oauth2/revoke
  flows:
  - authorizationUrl: https://core-api.redaptiveinc.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token
  - deviceAuthorizationUrl: https://core-api.redaptiveinc.com/oauth2/device_authorization
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
  - flow: tokenExchange
    grant_type: urn:ietf:params:oauth:grant-type:token-exchange
    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token
  implementation: Spring Authorization Server (inferred from /actuator/health + metadata shape)
  issuer: https://core-api.redaptiveinc.com
  name: RedaptiveCoreOAuth2
  response_types_supported:
  - code
  scopes_note: The metadata document declares no scopes_supported and there is no public scope or permission reference, so no scopes/ artifact is emitted rather than guess at one.
  scopes_published: false
  sender_constrained_tokens:
    spec: RFC 8705
    tls_client_certificate_bound_access_tokens: true
  source: well-known/redaptive-oauth-authorization-server.json
  type: oauth2
- in: header
  issuance: Issued by Redaptive to contracted Data Solutions customers; sharing prohibited by contract.
  name: RedaptiveDataSolutionsAPIKey
  note: The terms name the credential but not the header it travels in; the header name is not published anywhere public, so it is deliberately left unrecorded rather than invented.
  parameter_name_published: false
  source: https://redaptive.com/data-solutions-terms-and-conditions/
  type: apiKey
slug: redaptive-authentication
source_filename: redaptive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://core.api.prod.redaptivegroup.com/.well-known/oauth-authorization-server\ndocs: https://redaptive.com/data-solutions-terms-and-conditions/\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, tokenExchange, refreshToken]\n  public_reference: false\n  note: >-\n    Redaptive publishes no public API reference. The OAuth model below is read verbatim from\n    the RFC 8414 Authorization Server Metadata document the Redaptive ONE Core API gateway\n    serves anonymously. The API-key model is read from the published Data Solutions Terms and\n    Conditions, which define an \"API Key\" as \"a digital credential issued by Redaptive that\n    enables access to and use of the API\" — keys are issued by Redaptive to contracted\n    customers and may not be shared with third parties.\nschemes:\n- name: RedaptiveCoreOAuth2\n  type: oauth2\n  issuer: https://core-api.redaptiveinc.com\n\
  \  source: well-known/redaptive-oauth-authorization-server.json\n  implementation: Spring Authorization Server (inferred from /actuator/health + metadata shape)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://core-api.redaptiveinc.com/oauth2/authorize\n    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token\n    pkce: [S256]\n  - flow: clientCredentials\n    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token\n  - flow: deviceCode\n    grant_type: urn:ietf:params:oauth:grant-type:device_code\n    deviceAuthorizationUrl: https://core-api.redaptiveinc.com/oauth2/device_authorization\n  - flow: tokenExchange\n    grant_type: urn:ietf:params:oauth:grant-type:token-exchange\n    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://core-api.redaptiveinc.com/oauth2/token\n  endpoints:\n    jwks_uri: https://core-api.redaptiveinc.com/oauth2/jwks\n    revocation_endpoint: https://core-api.redaptiveinc.com/oauth2/revoke\n\
  \    introspection_endpoint: https://core-api.redaptiveinc.com/oauth2/introspect\n  client_authentication:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\n  sender_constrained_tokens:\n    tls_client_certificate_bound_access_tokens: true\n    spec: RFC 8705\n  response_types_supported: [code]\n  scopes_published: false\n  scopes_note: >-\n    The metadata document declares no scopes_supported and there is no public scope or\n    permission reference, so no scopes/ artifact is emitted rather than guess at one.\n- name: RedaptiveDataSolutionsAPIKey\n  type: apiKey\n  in: header\n  source: https://redaptive.com/data-solutions-terms-and-conditions/\n  issuance: Issued by Redaptive to contracted Data Solutions customers; sharing prohibited by contract.\n  parameter_name_published: false\n  note: >-\n    The terms name the credential but not the header it travels in; the header name is not\n \
  \   published anywhere public, so it is deliberately left unrecorded rather than invented.\ngaps:\n- No public authentication guide, token walkthrough, or API reference.\n- The declared issuer host core-api.redaptiveinc.com resolves but serves a TLS certificate\n  that does not match the hostname, so the metadata document's own issuer, jwks_uri, token,\n  introspection and revocation endpoints are not fetchable by an anonymous client.\nx-evidence:\n- url: https://core.api.prod.redaptivegroup.com/.well-known/oauth-authorization-server\n  status: 200\n  content_type: application/json\n  fetched: '2026-08-05'\n- url: https://core-api.redaptiveinc.com/oauth2/jwks\n  status: 0\n  error: TLS certificate subject name mismatch\n  fetched: '2026-08-05'\n- url: https://redaptive.com/data-solutions-terms-and-conditions/\n  status: 200\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redaptive/refs/heads/main/authentication/redaptive-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Energy
- Energy Efficiency
- Energy as a Service
- Sustainability
- ESG Reporting
- Metering
- Buildings
- Real-Estate
- Industrial
- Climate Tech
---
