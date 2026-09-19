---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'The Buzz API authenticates machine callers with OAuth 2.0 client credentials carrying a JWT client assertion (RFC 6749 + RFC 7523): the integration signs a short-lived assertion with an RSA private key whose public key is registered against an "Application Identity" user account, POSTs it to the token endpoint, and receives a one-hour Bearer access token it presents on every command. A legacy username/password flow (Login3) still works and is still supported, but the provider documents it as not recommended for new integrations. Authorization is not scope-based: every command names the Rights it requires against an entity (for example DeleteCourse@courseid), and those rights are granted to the Application Identity account exactly as they would be to a person. There is no OpenAPI document to derive securitySchemes from — this profile is read from the provider''s own published authentication reference.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agilix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agilix declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agilix
provider_slug: agilix
scheme_count: 3
schemes:
- access_token:
    expires_in: 3600
    header: 'Authorization: Bearer <token>'
    refresh_guidance: Re-authenticate every half hour for long-running processes.
    response_cache_control: no-store
    type: Bearer
  browser_use: Explicitly prohibited by the provider — the private key cannot be protected in a browser; this flow is server-side only.
  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
  client_id: The userid of the Application Identity account created with CreateUsers2 (type applicationidentity)
  flow: clientCredentials
  grant_type: client_credentials
  id: oauth2_jwt_client_credentials
  key_registration:
    body: SubjectPublicKeyInfo (SPKI) PEM public key
    content_type: application/x-pem-file
    method: PUT
    note: kid is caller-chosen (ASCII letters, digits, '-', '_', '.'; max 128 chars) and must match the kid header of the JWT assertion. PUTting an existing kid replaces the key in place and immediately breaks any running application still using the old one, so rotation is done by adding a second kid, cutting traffic over, then deleting the first.
    path: '{server}/api/users/{userid}/keys/{kid}'
    rights_required: Update User on the Application Identity account
    success_status: 204
  key_size: 2048-bit RSA or larger
  preferred: true
  scopes: []
  scopes_note: The provider documents no OAuth scope surface. Authorization is carried by the Buzz Rights model (per-command rights on a domain, course, user or enrollment entity), so there is no scopes/ artifact for this provider.
  signing_algorithm: RS256
  token_endpoint: '{server}/api/oauth/token'
  token_endpoint_example: https://backgroundapi.agilixbuzz.com/api/oauth/token
  type: oauth2
- commands:
  - Login3
  - Login2
  deprecated: true
  id: legacy_password_login
  note: Interactive username/password sign-in that mints a session token. Login2 is listed under Obsolete Commands and its own page says API users should now authenticate with OAuth 2.0 Application Identity instead. Login3 remains the like-for-like successor for interactive sign-in only. Enforces password policy, account lockout and multi-factor; returns SecondFactorRequired / SecondFactorConfigurationNowRequired when a second factor is owed.
  scheme: session-token
  type: http
- alternates:
  - location: request body
    name: _token
    note: For XML/JSON POST bodies where a header cannot be sent.
  - discouraged: true
    location: query
    name: _token
    note: The provider tells callers to use the query-string form only for contexts like browser-embedded resource URLs, because URLs are recorded in logs.
  cookies: Cookie-based authentication tokens are deprecated by the provider for cross-site scripting reasons.
  id: token_transport
  in: header
  name: Authorization
  type: apiKey
slug: agilix-authentication
source_filename: agilix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://api.agilixbuzz.com/docs/entry/Concept/OAuth.md\ndocs:\n- https://api.agilixbuzz.com/docs/entry/Concept/OAuth.md\n- https://api.agilixbuzz.com/docs/entry/Concept/CommandUsage.md\n- https://api.agilixbuzz.com/docs/entry/Concept/Rights.md\nname: Agilix Buzz (DLAP / xLi) API authentication\ndescription: >-\n  The Buzz API authenticates machine callers with OAuth 2.0 client credentials carrying a\n  JWT client assertion (RFC 6749 + RFC 7523): the integration signs a short-lived assertion\n  with an RSA private key whose public key is registered against an \"Application Identity\"\n  user account, POSTs it to the token endpoint, and receives a one-hour Bearer access token\n  it presents on every command. A legacy username/password flow (Login3) still works and is\n  still supported, but the provider documents it as not recommended for new integrations.\n  Authorization is not scope-based: every command names the Rights it\
  \ requires against an\n  entity (for example DeleteCourse@courseid), and those rights are granted to the\n  Application Identity account exactly as they would be to a person.\n  There is no OpenAPI document to derive securitySchemes from — this profile is read from\n  the provider's own published authentication reference.\nprimary_scheme: oauth2\nschemes:\n- id: oauth2_jwt_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  preferred: true\n  token_endpoint: '{server}/api/oauth/token'\n  token_endpoint_example: https://backgroundapi.agilixbuzz.com/api/oauth/token\n  grant_type: client_credentials\n  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n  client_id: The userid of the Application Identity account created with CreateUsers2 (type applicationidentity)\n  signing_algorithm: RS256\n  key_size: 2048-bit RSA or larger\n  key_registration:\n    method: PUT\n    path: '{server}/api/users/{userid}/keys/{kid}'\n    content_type: application/x-pem-file\n\
  \    body: SubjectPublicKeyInfo (SPKI) PEM public key\n    success_status: 204\n    rights_required: Update User on the Application Identity account\n    note: >-\n      kid is caller-chosen (ASCII letters, digits, '-', '_', '.'; max 128 chars) and must\n      match the kid header of the JWT assertion. PUTting an existing kid replaces the key\n      in place and immediately breaks any running application still using the old one, so\n      rotation is done by adding a second kid, cutting traffic over, then deleting the first.\n  access_token:\n    type: Bearer\n    header: 'Authorization: Bearer <token>'\n    expires_in: 3600\n    response_cache_control: no-store\n    refresh_guidance: Re-authenticate every half hour for long-running processes.\n  scopes: []\n  scopes_note: >-\n    The provider documents no OAuth scope surface. Authorization is carried by the Buzz\n    Rights model (per-command rights on a domain, course, user or enrollment entity), so\n    there is no scopes/ artifact\
  \ for this provider.\n  browser_use: >-\n    Explicitly prohibited by the provider — the private key cannot be protected in a\n    browser; this flow is server-side only.\n- id: legacy_password_login\n  type: http\n  scheme: session-token\n  deprecated: true\n  commands:\n  - Login3\n  - Login2\n  note: >-\n    Interactive username/password sign-in that mints a session token. Login2 is listed under\n    Obsolete Commands and its own page says API users should now authenticate with OAuth 2.0\n    Application Identity instead. Login3 remains the like-for-like successor for interactive\n    sign-in only. Enforces password policy, account lockout and multi-factor; returns\n    SecondFactorRequired / SecondFactorConfigurationNowRequired when a second factor is owed.\n- id: token_transport\n  type: apiKey\n  in: header\n  name: Authorization\n  alternates:\n  - location: request body\n    name: _token\n    note: For XML/JSON POST bodies where a header cannot be sent.\n  - location: query\n \
  \   name: _token\n    discouraged: true\n    note: >-\n      The provider tells callers to use the query-string form only for contexts like\n      browser-embedded resource URLs, because URLs are recorded in logs.\n  cookies: >-\n    Cookie-based authentication tokens are deprecated by the provider for cross-site\n    scripting reasons.\nfederation:\n- protocol: SAML 2.0\n  role: service provider / single sign-on for Buzz end users\n  evidence: https://www.agilix.com/security\n  note: Buzz supports SSO via SAML 2.0 and Google authentication; SAML single logout is documented in the API release notes.\n- protocol: LTI 1.3 / OpenID Connect\n  role: platform (Buzz is the LTI platform; tools launch into it)\n  jwks_uri: https://api.agilixbuzz.com/lti/platform/jwks\n  authentication_endpoint: https://api.agilixbuzz.com/lti/authentication\n  token_endpoint: '{server}/lti/accesstoken/{entityid}'\n  evidence: https://api.agilixbuzz.com/docs/entry/Concept/LTIIntegration.md\nmulti_factor:\n  supported:\
  \ true\n  commands:\n  - SecondFactorAuthenticate\n  - CreateSecondFactorAuthenticationSecret\n  - SetupSecondFactorAuthentication\n  - ClearSecondFactorAuthentication\n  note: >-\n    TOTP-style second factor with a remembermfa token; policy-driven via the domain password\n    policy's mfaenforcement attribute. A documented reason to prefer OAuth for integrations\n    is that JWT assertion auth works in domains where MFA is required for administrative\n    accounts.\npassword_policy:\n  documented: true\n  url: https://api.agilixbuzz.com/docs/entry/Schema/PasswordPolicy.md\n  commands:\n  - GetEffectivePasswordPolicy\n  - CheckPasswordQuality\n  note: >-\n    Per-domain policy covering minimum length, character classes, entropy, breached-password\n    (pwned) checking, expiry, lockout and MFA. Each requirement is inert until its matching\n    enforcement attribute is set — the provider documents this explicitly.\nstandards:\n- RFC 6749 (OAuth 2.0)\n- RFC 7523 (JWT Profile for OAuth 2.0\
  \ Client Authentication)\n- RFC 7519 (JSON Web Token)\n- RFC 7517 (JSON Web Key)\n- SAML 2.0\n- OpenID Connect (as used by LTI 1.3 launch)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilix/refs/heads/main/authentication/agilix-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Education
- EdTech
- Learning Management System
- K-12
- Online Learning
- Tutoring
- Assessment
- LTI
- SCORM
- Artificial Intelligence
- Event
---
