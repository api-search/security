---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Savvymoney Authentication
name_suffix: Authentication
oauth_flows: []
overview: SavvyMoney declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: SavvyMoney
provider_slug: savvymoney
scheme_count: 3
schemes:
- applies_to: SavvyMoney SSO REST API + External Credit API
  binding:
    audience_restriction: '"Access tokens are restricted to access the set of partners from the set of audience domains described in the SSO client credentials."'
    browser_fingerprint: Optional. The partner may obtain a browser "Fingerprint" from the SSO server and pass it on sign-on to restrict use of the access token to that same browser.
  credentials:
  - description: Client identifier issued by SavvyMoney.
    name: authId
  - description: Authentication key in JWT format.
    name: authKey
  - description: The SavvyMoney domains or partner credit-score subdomains an API user is scoped to.
    name: Audience Domains
  - description: The partner IDs an API user is authorised to perform SSO for.
    name: Partner ID List
  - description: Symmetric key used to encrypt member attributes in transit inside the request body.
    name: AES/CBC Encryption Key
  description: Partner-scoped JWT flow. SavvyMoney issues each partner application an Authentication ID (Auth ID, the client identifier) and an Authentication Key (Auth Key, in JWT format). The partner server POSTs those credentials plus the member attributes to the SSO Authentication API and receives a short-lived authorization code in JWT format. The code is exchanged at the sign-on endpoint for an access token, which is then sent to the Credit API in an HTTP Authorization header.
  family: jwt-bearer
  header: Authorization
  id: savvymoney-sso-jwt
  in: header
  token:
    format: JWT
    lifetime_note: '"the access token will automatically expire in 10 minutes"'
    lifetime_seconds: 600
    renew_operation: SSO Prolong API
    renewable: true
    revocable: true
    revoke_operation: SSO Log Off API
  type: custom
- applies_to: Partner online/mobile banking SSO (alternative to the REST flow)
  description: SavvyMoney documents SAML 2.0 as an alternative to the REST API for establishing single sign-on from a partner's online or mobile banking platform.
  id: savvymoney-saml2
  source: https://hub.savvymoney.com/sphub/cms/delivery/media/MCS7KWMTKCWNE7VNGJI5TFUISKCY
  type: saml2
- applies_to: SavvyMoney Partner Hub (hub.savvymoney.com) — NOT the credit API
  authorization_endpoint: https://hub.savvymoney.com/services/oauth2/authorize
  dpop_supported: true
  id: savvymoney-hub-oidc
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://hub.savvymoney.com/services/oauth2/introspect
  issuer: https://hub.savvymoney.com
  jwks_uri: https://hub.savvymoney.com/id/keys
  note: Served under SavvyMoney's own issuer but emitted by the Salesforce Experience Cloud platform hosting the Partner Hub — the advertised scopes are Salesforce-native. This governs partner hub sign-in, not the credit/SSO REST API.
  openid_configuration: https://hub.savvymoney.com/.well-known/openid-configuration
  registration_endpoint: https://hub.savvymoney.com/services/oauth2/register
  revocation_endpoint: https://hub.savvymoney.com/services/oauth2/revoke
  token_endpoint: https://hub.savvymoney.com/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://hub.savvymoney.com/services/oauth2/userinfo
slug: savvymoney-authentication
source_filename: savvymoney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://hub.savvymoney.com/sphub/cms/delivery/media/MCTB4AZJKJRJBWFAXB4W2WLUCAPQ\ndocs: https://hub.savvymoney.com/sphub/cms/delivery/media/MCTB4AZJKJRJBWFAXB4W2WLUCAPQ\nnote: >-\n  Derived from SavvyMoney's own publicly downloadable \"SSO Integration Using SavvyMoney REST API\"\n  guide (v2.1, 8 Aug 2022) and the \"Mobile Integration Guide\" (v1.8, 17 Sep 2019), both served\n  from hub.savvymoney.com without authentication. No OpenAPI securitySchemes block exists —\n  SavvyMoney publishes no machine-readable contract — so every field below is quoted from those\n  documents or observed on a live unauthenticated probe.\nschemes:\n- id: savvymoney-sso-jwt\n  applies_to: SavvyMoney SSO REST API + External Credit API\n  type: custom\n  family: jwt-bearer\n  in: header\n  header: Authorization\n  description: >-\n    Partner-scoped JWT flow. SavvyMoney issues each partner application an Authentication ID\n    (Auth ID, the client\
  \ identifier) and an Authentication Key (Auth Key, in JWT format). The\n    partner server POSTs those credentials plus the member attributes to the SSO Authentication\n    API and receives a short-lived authorization code in JWT format. The code is exchanged at the\n    sign-on endpoint for an access token, which is then sent to the Credit API in an HTTP\n    Authorization header.\n  credentials:\n  - name: authId\n    description: Client identifier issued by SavvyMoney.\n  - name: authKey\n    description: Authentication key in JWT format.\n  - name: Audience Domains\n    description: The SavvyMoney domains or partner credit-score subdomains an API user is scoped to.\n  - name: Partner ID List\n    description: The partner IDs an API user is authorised to perform SSO for.\n  - name: AES/CBC Encryption Key\n    description: Symmetric key used to encrypt member attributes in transit inside the request body.\n  token:\n    format: JWT\n    lifetime_seconds: 600\n    lifetime_note: '\"the\
  \ access token will automatically expire in 10 minutes\"'\n    renewable: true\n    renew_operation: SSO Prolong API\n    revocable: true\n    revoke_operation: SSO Log Off API\n  binding:\n    browser_fingerprint: >-\n      Optional. The partner may obtain a browser \"Fingerprint\" from the SSO server and pass it on\n      sign-on to restrict use of the access token to that same browser.\n    audience_restriction: >-\n      \"Access tokens are restricted to access the set of partners from the set of audience domains\n      described in the SSO client credentials.\"\n- id: savvymoney-saml2\n  applies_to: Partner online/mobile banking SSO (alternative to the REST flow)\n  type: saml2\n  description: >-\n    SavvyMoney documents SAML 2.0 as an alternative to the REST API for establishing single\n    sign-on from a partner's online or mobile banking platform.\n  source: https://hub.savvymoney.com/sphub/cms/delivery/media/MCS7KWMTKCWNE7VNGJI5TFUISKCY\n- id: savvymoney-hub-oidc\n  applies_to:\
  \ SavvyMoney Partner Hub (hub.savvymoney.com) — NOT the credit API\n  type: openIdConnect\n  openid_configuration: https://hub.savvymoney.com/.well-known/openid-configuration\n  issuer: https://hub.savvymoney.com\n  authorization_endpoint: https://hub.savvymoney.com/services/oauth2/authorize\n  token_endpoint: https://hub.savvymoney.com/services/oauth2/token\n  userinfo_endpoint: https://hub.savvymoney.com/services/oauth2/userinfo\n  revocation_endpoint: https://hub.savvymoney.com/services/oauth2/revoke\n  introspection_endpoint: https://hub.savvymoney.com/services/oauth2/introspect\n  registration_endpoint: https://hub.savvymoney.com/services/oauth2/register\n  jwks_uri: https://hub.savvymoney.com/id/keys\n  id_token_signing_alg_values_supported: [RS256]\n  dpop_supported: true\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  note: >-\n    Served under SavvyMoney's own issuer but emitted by the Salesforce Experience Cloud\
  \ platform\n    hosting the Partner Hub — the advertised scopes are Salesforce-native. This governs partner\n    hub sign-in, not the credit/SSO REST API.\nendpoints_documented:\n- operation: SSO Authentication API\n  method: POST\n  path_note: >-\n    Path not stated in the public guide; only the request/response JSON models are shown. Recorded\n    as documented-but-unnamed rather than guessed.\n- operation: SSO Fingerprint API\n  method: GET\n  path_note: Optional, called from the browser. Path not stated in the public guide.\n- operation: SSO Sign On API\n  method: POST\n  path: /sso/api/rest/signon\n  example: 'curl -X POST \"https://creditscoretest.savvymoney.com/sso/api/rest/signon\"'\n- operation: SSO Prolong API\n  method: POST\n  path: /sso/api/rest/prolong\n  example: 'curl -X POST \"https://creditscoretest.savvymoney.com/sso/api/rest/prolong\"'\n- operation: SSO Log Off API\n  method: POST\n  path: /sso/api/rest/logoff\n  example: 'curl -X POST \"https://creditscoretest.savvymoney.com/sso/api/rest/logoff\"\
  '\n- operation: SSO Relay Form POST (iFrame)\n  method: POST\n  path: /sso/api/RelayPost\n  note: HTML form POST carrying AuthCode + AuthAppUrl, targeted at an iFrame.\n- operation: SSO Redirect API\n  method: POST\n  path_note: Path not stated; request model is {authCode, appUrl} and the response carries redirectUrl.\ntransport_security:\n  tls_minimum: TLSv1.2\n  tls_note: '\"SavvyMoney supports only TLS 1.2 SSL.\" Observed live negotiation on creditscore.savvymoney.com is TLSv1.3.'\n  disabled_ciphers:\n  - TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 (0xc030)\n  - TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 (0xc02f)\n  - TLS_DHE_RSA_WITH_AES_256_GCM_SHA384 (0x9f)\n  - TLS_DHE_RSA_WITH_AES_128_GCM_SHA256 (0x9e)\n  ip_allowlisting:\n    required_of_partner: true\n    note: >-\n      Partners must allowlist SavvyMoney's static egress IPs. Production 3.227.227.11 and\n      3.222.59.58; beta 18.210.174.44 and 75.101.165.109. SavvyMoney states it does not require\n      the partner's servers to be allowlisted\
  \ in return.\nattribute_encryption:\n  algorithm: AES/CBC\n  applies_to: SSO member attributes (partnerMemberId, firstName, lastName, email, address, city, state, zip, dob, ssn, supplemental1-3)\n  flag: 'Each attribute carries an \"encrypted\": true|false boolean in the request body.'\n  guide: Attribute Encryption Guide (referenced by the SSO guide; not published publicly)\ngaps:\n- No OpenAPI/Swagger document is published, so no securitySchemes block can be harvested.\n- The full endpoint reference (\"SavvyMoney API Document\") is partner-gated; three of the six documented SSO operations have no public path.\n- No rotation, expiry or revocation policy is published for the long-lived Auth ID / Auth Key credential pair.\nevidence:\n- url: https://hub.savvymoney.com/sphub/cms/delivery/media/MCTB4AZJKJRJBWFAXB4W2WLUCAPQ\n  status: 200\n  content_type: application/pdf\n- url: https://hub.savvymoney.com/.well-known/openid-configuration\n  status: 200\n  content_type: application/json\n- url:\
  \ https://creditscore.savvymoney.com/sso/api/rest/signon\n  status: 200\n  note: 'Unauthenticated POST {} returned {\"errorMessage\":\"Missing authCode.\",\"hasErrors\":true} — endpoint confirmed live.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savvymoney/refs/heads/main/authentication/savvymoney-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Financial Services
- Credit Scores
- Credit Monitoring
- Financial Wellness
- Banking
- Credit Unions
- Fintech
- Single Sign On
- Embedded Finance
- Lending
- Account Opening
---
