---
api_key_in: []
auth_types:
- mutualTLS
- oauth2
- openIdConnect
- http
description: 'Lloyd''s market APIs are dual-credentialed. Every call carries TWO independent identifying security tokens: a client X.509 certificate presented on the mutual-TLS handshake to the London Market API Gateway (which identifies the calling APPLICATION via the certificate Subject CN), and an Authorization: Bearer JWT issued by the LIMOSS Common Services Azure Active Directory tenant (which identifies the PRINCIPAL). The bearer token must be an on-behalf-of token carrying an "scp" claim of user_impersonation - a plain OAuth 2.0 login token is explicitly not sufficient. There is no API-key path and no self-serve credential issuance: certificates are registered per environment through LIMOSS onboarding.'
kind: authentication
layout: security
method: searched
name: Lloyds Of London Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- on-behalf-of
- client_credentials
overview: Lloyd's of London secures its APIs with mutualTLS, oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, on-behalf-of, and client_credentials flow(s).
provider_name: Lloyd's of London
provider_slug: lloyds-of-london
scheme_count: 4
schemes:
- description: The API Consumer must initiate the HTTPS connection to the API Gateway with a client X.509 certificate. The CN of the Subject field identifies the calling application. The certificate must be signed by a CA in the Microsoft Trusted Root Certificate Program and should be an Extended Validation certificate. A DIFFERENT certificate must be registered per environment (Sandbox, PreProd, Production).
  evidence: 'Live probe 2026-07-25 - GET https://api.londonmarketgroup.co.uk/Lloyds/CatastropheCodes/v1/CatastropheCodes returns 401 {"Code":401,"Message":"Client certificate is missing. Ref: ..."}'
  name: ClientCertificate
  registration: LIMOSS API Gateway onboarding, per environment
  required: true
  sources:
  - Lloyd's Base API Standard section 5.12.1
  type: mutualTLS
- bearerFormat: JWT
  description: 'Authorization: Bearer <JWT>. The JWT must be signed by a Security Token Service known to the API Gateway (the Common Services Azure AD tenant) and must be an on-behalf-of token issued to the calling application, carrying scp=user_impersonation. Tokens returned directly from an OAuth 2.0 login are normally NOT on-behalf-of tokens; the application backend must exchange them with Azure AD. Where an API validates the audience claim, the gateway may itself obtain a further on-behalf-of token with the correct aud.'
  flows:
  - authority: https://login.microsoftonline.com/{tenantId}
    callback_path: /signin-oidc
    flow: authorizationCode
    note: tenantId is the SAND, PreProd or Prod Common Services tenant, supplied during onboarding.
    response_type: code id_token
  - flow: on-behalf-of
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    note: RFC 7523 JWT bearer assertion exchange, required to mint the token actually sent to the gateway.
  - flow: client_credentials
    note: Service-account (headless server-to-server) tokens for API consumers with no browser leg.
  name: AzureADBearer
  required: true
  scheme: bearer
  scopes:
  - user_impersonation
  sources:
  - Lloyd's Base API Standard section 5.12.1
  - Lloyd's Authentication Information page
  type: oauth2
- audience: API Providers (internal leg)
  description: After enforcing the client certificate and inbound JWT, the API Gateway acts as a Policy Enforcement Point and mints a NEW signed JWT for the API Provider, embedding the original consumer token in an "lmg_pkt" claim. Providers verify that JWT against the gateway's published OIDC discovery document and JWKS.
  jwks_uri: https://api.londonmarketgroup.co.uk/discovery/keys
  live_status: 200 (probed 2026-07-25)
  name: GatewaySignedJWT
  openIdConnectUrl: https://api.londonmarketgroup.co.uk/discovery/.well-known/openid-configuration
  required: false
  sources:
  - Lloyd's Base API Standard section 5.12.2
  - well-known/lloyds-of-london-well-known.yml
  type: openIdConnect
- description: 'Degraded alternative shown in the Lloyd''s sample application: where the client is configured with RequireOnBehalfOfToken=false, the Authorization header carries "X-Assert <user email>" instead of a bearer token. Not part of the Base API Standard''s mandatory rules; present in the published PlacingHttpClientFactory sample.'
  name: XAssert
  required: false
  scheme: X-Assert
  sources:
  - Lloyd's Authentication Information page
  type: http
slug: lloyds-of-london-authentication
source_filename: lloyds-of-london-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://web.archive.org/web/20200930095802/https://developer.lloyds.com/Get-Started/Base-API-Standard\n  (section 5.12 Security) and\n  https://web.archive.org/web/20200930085423/https://developer.lloyds.com/Get-Started/Authentication-Information\ndocs:\n- https://web.archive.org/web/20200930085423/https://developer.lloyds.com/Get-Started/Authentication-Information\n- https://web.archive.org/web/20200930095802/https://developer.lloyds.com/Get-Started/Base-API-Standard\n- https://web.archive.org/web/20200930075931/https://developer.lloyds.com/Get-Started/Registration-Onboarding\ndescription: >-\n  Lloyd's market APIs are dual-credentialed. Every call carries TWO independent identifying\n  security tokens: a client X.509 certificate presented on the mutual-TLS handshake to the\n  London Market API Gateway (which identifies the calling APPLICATION via the certificate\n  Subject CN), and an Authorization: Bearer JWT issued\
  \ by the LIMOSS Common Services Azure\n  Active Directory tenant (which identifies the PRINCIPAL). The bearer token must be an\n  on-behalf-of token carrying an \"scp\" claim of user_impersonation - a plain OAuth 2.0 login\n  token is explicitly not sufficient. There is no API-key path and no self-serve credential\n  issuance: certificates are registered per environment through LIMOSS onboarding.\nsummary:\n  types: [mutualTLS, oauth2, openIdConnect, http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oauth2_flows: [authorizationCode, on-behalf-of, client_credentials]\n  api_key_in: []\n  self_serve_credentials: false\n  mfa_signalled: true\nschemes:\n- name: ClientCertificate\n  type: mutualTLS\n  required: true\n  description: >-\n    The API Consumer must initiate the HTTPS connection to the API Gateway with a client X.509\n    certificate. The CN of the Subject field identifies the calling application. The certificate\n    must be signed by a CA in the Microsoft Trusted Root Certificate\
  \ Program and should be an\n    Extended Validation certificate. A DIFFERENT certificate must be registered per environment\n    (Sandbox, PreProd, Production).\n  evidence: >-\n    Live probe 2026-07-25 - GET https://api.londonmarketgroup.co.uk/Lloyds/CatastropheCodes/v1/CatastropheCodes\n    returns 401 {\"Code\":401,\"Message\":\"Client certificate is missing. Ref: ...\"}\n  registration: LIMOSS API Gateway onboarding, per environment\n  sources: [Lloyd's Base API Standard section 5.12.1]\n- name: AzureADBearer\n  type: oauth2\n  required: true\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Authorization: Bearer <JWT>. The JWT must be signed by a Security Token Service known to the\n    API Gateway (the Common Services Azure AD tenant) and must be an on-behalf-of token issued to\n    the calling application, carrying scp=user_impersonation. Tokens returned directly from an\n    OAuth 2.0 login are normally NOT on-behalf-of tokens; the application backend must exchange\n\
  \    them with Azure AD. Where an API validates the audience claim, the gateway may itself obtain\n    a further on-behalf-of token with the correct aud.\n  flows:\n  - flow: authorizationCode\n    authority: https://login.microsoftonline.com/{tenantId}\n    callback_path: /signin-oidc\n    response_type: code id_token\n    note: >-\n      tenantId is the SAND, PreProd or Prod Common Services tenant, supplied during onboarding.\n  - flow: on-behalf-of\n    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n    note: RFC 7523 JWT bearer assertion exchange, required to mint the token actually sent to the gateway.\n  - flow: client_credentials\n    note: Service-account (headless server-to-server) tokens for API consumers with no browser leg.\n  scopes: [user_impersonation]\n  sources: [Lloyd's Base API Standard section 5.12.1, Lloyd's Authentication Information page]\n- name: GatewaySignedJWT\n  type: openIdConnect\n  required: false\n  audience: API Providers (internal leg)\n  description:\
  \ >-\n    After enforcing the client certificate and inbound JWT, the API Gateway acts as a Policy\n    Enforcement Point and mints a NEW signed JWT for the API Provider, embedding the original\n    consumer token in an \"lmg_pkt\" claim. Providers verify that JWT against the gateway's\n    published OIDC discovery document and JWKS.\n  openIdConnectUrl: https://api.londonmarketgroup.co.uk/discovery/.well-known/openid-configuration\n  jwks_uri: https://api.londonmarketgroup.co.uk/discovery/keys\n  live_status: 200 (probed 2026-07-25)\n  sources: [Lloyd's Base API Standard section 5.12.2, well-known/lloyds-of-london-well-known.yml]\n- name: XAssert\n  type: http\n  required: false\n  scheme: X-Assert\n  description: >-\n    Degraded alternative shown in the Lloyd's sample application: where the client is configured\n    with RequireOnBehalfOfToken=false, the Authorization header carries \"X-Assert <user email>\"\n    instead of a bearer token. Not part of the Base API Standard's mandatory\
  \ rules; present in\n    the published PlacingHttpClientFactory sample.\n  sources: [Lloyd's Authentication Information page]\njwt_claims:\n  mandatory:\n  - {claim: scp, value: user_impersonation, note: must be present on the consumer token}\n  understood:\n  - {claim: sub, meaning: 'Immutable identifier of the principal; safe for authorisation checks.'}\n  - {claim: upn, meaning: 'Principal identity as an email address; may change over the lifetime of the individual.'}\n  - {claim: amr, meaning: 'Authentication methods used; presence of \"mfa\" means multi-factor authentication took place.'}\n  - {claim: aud, meaning: 'Audience; must match the endpoint URI up to but not including the version.'}\n  - {claim: iss, meaning: 'Issuer; must match the gateway URI for the environment, e.g. https://sand-api.londonmarketgroup.co.uk/ in Sandbox.'}\n  additional: [appid, given_name, idp, iat, family_name, unique_name, oid, nbf, exp, lmg_mpo, lmg_cert_dn, lmg_pkt]\n  ttl_rule: >-\n    Any token issued\
  \ by the API Gateway must not have a TTL longer than the token that called it;\n    nbf is set to now and exp to the expiry of the original token.\nauthorization:\n  model: >-\n    The API Gateway may perform high-level authorisation but should not perform low-level\n    role-based authorisation; API Providers may use any JWT claim for authorisation. Failure at\n    either enforcement step returns 401 with a message indicating which PEP step failed.\n  errors: [ResourceAccessDenied, AccessToReferencedResourceNotAllowed, NotDocumentOwner]\nonboarding:\n  self_serve: false\n  steps:\n  - Onboard the organisation to LIMOSS Common Services / the LIMOSS API Gateway (\"Subscribe to PPL API\").\n  - Guest the account identity into each Common Services environment separately (Sandbox, PreProd, Production).\n  - Register the application in the Common Services Azure Active Directory (CS Developers On-Boarding Guide v1.1).\n  - Register an X.509 certificate in each API Gateway environment (a different\
  \ certificate per environment).\n  - For Sandbox/PreProd test data, request test-harness setup from the Lloyd's API Factory.\n  contacts:\n  - {purpose: API Factory - licences, test harnesses, API standards, design issues, email: developer@lloyds.com}\n  - {purpose: Placing API adoption on the PPL platform, email: PPLEnquiries@lloyds.com}\n  - {purpose: LIMOSS onboarding and SLA, url: 'https://limoss.london/'}\ntransport_security:\n  https_only: true\n  mutual_tls: true\n  gateway_certificate: Extended Validation certificate signed by a Microsoft Trusted Root CA\n  observed_tls: TLSv1.2 (api.londonmarketgroup.co.uk, probed 2026-07-25)\nrelated:\n- scopes/lloyds-of-london-scopes.yml\n- well-known/lloyds-of-london-well-known.yml\n- conventions/lloyds-of-london-conventions.yml\n- sandbox/lloyds-of-london-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lloyds-of-london/refs/heads/main/authentication/lloyds-of-london-authentication.yml
summary_line: mutualTLS/oauth2/openIdConnect/http · 4 schemes
tags:
- Insurance
- United Kingdom
- Reinsurance
- Specialty Insurance
- London Market
- Underwriting
- Claims
- Delegated Authority
- Broker
- Market Infrastructure
- Standards
- ACORD
---
