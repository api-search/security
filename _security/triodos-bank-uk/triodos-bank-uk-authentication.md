---
api_key_in: []
api_specs:
- filename: triodos-bank-uk-xs2a-openapi.json
  format: json
  label: Triodos Account Information Service (AIS) API
  slug: triodos-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-xs2a-openapi.json
- filename: triodos-bank-uk-xs2a-openapi.json
  format: json
  label: Triodos Payment Initiation Service (PIS) API
  slug: triodos-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-xs2a-openapi.json
- filename: triodos-bank-uk-xs2a-openapi.json
  format: json
  label: Triodos Confirmation of Funds Service (CoF) API
  slug: triodos-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-xs2a-openapi.json
- filename: triodos-bank-uk-auth-openapi.json
  format: json
  label: Triodos XS2A Authorization (OAuth2/OIDC) API
  slug: triodos-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-auth-openapi.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
- httpMessageSignature
- http-basic
description: ''
kind: authentication
layout: security
method: searched
name: Triodos Bank Uk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Triodos Bank UK secures its APIs with oauth2, openIdConnect, mutualTLS, httpMessageSignature, and http-basic across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Triodos Bank UK
provider_slug: triodos-bank-uk
scheme_count: 4
schemes:
- description: Production data endpoints (https://api-ma.triodos.com) require a mutual-TLS connection presenting a valid eIDAS QWAC (Qualified Website Authentication Certificate). Not required in the sandbox (https://xs2a-sandbox.triodos.com). Client-initiated browser authorisations use the non-mTLS host https://api.triodos.com to avoid prompting the PSU for a client certificate.
  layer: transport
  name: eidas-qwac-mtls
  type: mutualTLS
- algorithms:
  - rsa-sha256
  - rsa-sha512
  description: All XS2A endpoints mandate a digital signature per the NextGenPSD2 Framework v1.3 (Errata), referencing draft-cavage-http-signatures-10. The TPP signs the request with its eIDAS QSEALC (Qualified Electronic Seal Certificate).
  digest: SHA-256=
  headers:
  - Digest
  - Signature
  - TPP-Signature-Certificate
  - X-Request-ID
  keyid_format: SN=<hex-serial>,<CA-DistinguishedName in RFC1779>
  layer: message
  name: tpp-http-message-signature
  signed_headers:
  - digest
  - x-request-id
  type: httpMessageSignature
- description: OpenID Connect Authorization Code Flow implements the OAuth2 SCA approach. Per-tenant discovery documents (nl / uk / be) are exposed as an API operation.
  layer: application
  name: openid-connect
  openIdConnectUrl: https://api.triodos.com/auth/{tenant}/.well-known/openid-configuration
  sandbox_openIdConnectUrl: https://xs2a-sandbox.triodos.com/auth/{tenant}/.well-known/openid-configuration
  type: openIdConnect
- access_token_ttl_seconds: 600
  authorizationUrl: https://api.triodos.com/auth/{tenant}/v1/auth
  dynamic_client_registration: OAuth 2.0 Dynamic Client Registration gated by an Initial Access Token, which is obtained by presenting the TPP eIDAS X.509 certificate to GET /{tenant}/onboarding/v1 (initialAccessToken).
  flow: authorizationCode
  layer: application
  name: oauth2-authorization-code
  pkce: required (RFC 7636, S256 code_challenge_method)
  refresh: offline_access scope issues a refresh token (grant_type=refresh_token)
  registrationUrl: https://api.triodos.com/auth/{tenant}/v1/registration
  revocationUrl: https://api.triodos.com/auth/{tenant}/v1/token/revoke
  tokenUrl: https://api.triodos.com/auth/{tenant}/v1/token
  token_endpoint_auth: HTTP Basic (client_id:client_secret, RFC 2617)
  type: oauth2
  userinfoUrl: https://api.triodos.com/auth/{tenant}/v1/userinfo
slug: triodos-bank-uk-authentication
source_filename: triodos-bank-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.triodos.com/docs/authorisation\ndocs:\n- https://developer.triodos.com/docs/authorisation\n- https://developer.triodos.com/docs/signatures\n- https://developer.triodos.com/docs/registration\nnotes: >-\n  The harvested OpenAPI documents do not declare components.securitySchemes (the\n  Berlin Group NextGenPSD2 template externalises auth), so this profile is\n  captured from the Triodos developer documentation rather than derived from the\n  spec. Auth is a multi-layer PSD2 stack: transport-layer eIDAS mutual-TLS,\n  message-layer HTTP signatures, and application-layer OAuth2/OpenID Connect with\n  PSD2 Strong Customer Authentication.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS, httpMessageSignature, http-basic]\n  oauth2_flows: [authorizationCode, refreshToken]\n  sca: required\n  standard: Berlin Group NextGenPSD2 XS2A v1.3.6 (OAuth2 SCA Approach, Implicit Start)\nschemes:\n- name: eidas-qwac-mtls\n\
  \  layer: transport\n  type: mutualTLS\n  description: >-\n    Production data endpoints (https://api-ma.triodos.com) require a mutual-TLS\n    connection presenting a valid eIDAS QWAC (Qualified Website Authentication\n    Certificate). Not required in the sandbox (https://xs2a-sandbox.triodos.com).\n    Client-initiated browser authorisations use the non-mTLS host\n    https://api.triodos.com to avoid prompting the PSU for a client certificate.\n- name: tpp-http-message-signature\n  layer: message\n  type: httpMessageSignature\n  description: >-\n    All XS2A endpoints mandate a digital signature per the NextGenPSD2 Framework\n    v1.3 (Errata), referencing draft-cavage-http-signatures-10. The TPP signs the\n    request with its eIDAS QSEALC (Qualified Electronic Seal Certificate).\n  headers: [Digest, Signature, TPP-Signature-Certificate, X-Request-ID]\n  algorithms: [rsa-sha256, rsa-sha512]\n  digest: SHA-256=\n  signed_headers: [digest, x-request-id]\n  keyid_format: 'SN=<hex-serial>,<CA-DistinguishedName\
  \ in RFC1779>'\n- name: openid-connect\n  layer: application\n  type: openIdConnect\n  openIdConnectUrl: https://api.triodos.com/auth/{tenant}/.well-known/openid-configuration\n  sandbox_openIdConnectUrl: https://xs2a-sandbox.triodos.com/auth/{tenant}/.well-known/openid-configuration\n  description: >-\n    OpenID Connect Authorization Code Flow implements the OAuth2 SCA approach.\n    Per-tenant discovery documents (nl / uk / be) are exposed as an API operation.\n- name: oauth2-authorization-code\n  layer: application\n  type: oauth2\n  flow: authorizationCode\n  pkce: required (RFC 7636, S256 code_challenge_method)\n  authorizationUrl: https://api.triodos.com/auth/{tenant}/v1/auth\n  tokenUrl: https://api.triodos.com/auth/{tenant}/v1/token\n  revocationUrl: https://api.triodos.com/auth/{tenant}/v1/token/revoke\n  userinfoUrl: https://api.triodos.com/auth/{tenant}/v1/userinfo\n  registrationUrl: https://api.triodos.com/auth/{tenant}/v1/registration\n  token_endpoint_auth: HTTP Basic (client_id:client_secret,\
  \ RFC 2617)\n  access_token_ttl_seconds: 600\n  refresh: offline_access scope issues a refresh token (grant_type=refresh_token)\n  dynamic_client_registration: >-\n    OAuth 2.0 Dynamic Client Registration gated by an Initial Access Token, which\n    is obtained by presenting the TPP eIDAS X.509 certificate to\n    GET /{tenant}/onboarding/v1 (initialAccessToken).\nscopes_ref: scopes/triodos-bank-uk-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/authentication/triodos-bank-uk-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS/httpMessageSignature/http-basic · 4 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- XS2A
- Berlin Group
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Ethical Banking
- Sustainable Finance
- Specialist Lender
---
