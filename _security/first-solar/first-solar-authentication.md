---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: First Solar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: First Solar secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: First Solar
provider_slug: first-solar
scheme_count: 2
schemes:
- claims_supported:
  - active
  - address
  - email
  - email_verified
  - family_name
  - given_name
  - is_app_installed
  - language
  - locale
  - name
  - nickname
  - organization_id
  - phone_number
  - phone_number_verified
  - photos
  - picture
  - preferred_username
  - profile
  - sub
  - updated_at
  - urls
  - user_id
  - user_type
  - zoneinfo
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://portal.firstsolar.com/developer
  jwks_uri: https://portal.firstsolar.com/developer/id/keys
  name: OpenIDConnect
  openIdConnectUrl: https://portal.firstsolar.com/.well-known/openid-configuration
  sources:
  - well-known/first-solar-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
- end_session_endpoint: https://portal.firstsolar.com/developer/services/auth/idp/oidc/logout
  flows:
  - authorizationUrl: https://portal.firstsolar.com/developer/services/oauth2/authorize
    flow: authorizationCode
    refreshUrl: https://portal.firstsolar.com/developer/services/oauth2/token
    scope_count: 36
    tokenUrl: https://portal.firstsolar.com/developer/services/oauth2/token
  introspection_endpoint: https://portal.firstsolar.com/developer/services/oauth2/introspect
  name: OAuth2
  registration_endpoint: https://portal.firstsolar.com/developer/services/oauth2/register
  response_types_supported:
  - code
  - token
  - token id_token
  revocation_endpoint: https://portal.firstsolar.com/developer/services/oauth2/revoke
  sources:
  - well-known/first-solar-openid-configuration.json
  type: oauth2
  userinfo_endpoint: https://portal.firstsolar.com/developer/services/oauth2/userinfo
slug: first-solar-authentication
source_filename: first-solar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: https://portal.firstsolar.com/.well-known/openid-configuration\ndocs: https://portal.firstsolar.com/developer/PortalCustomLogin\nnote: 'Served by the Salesforce Experience Cloud tenant that runs the First Solar Developer Portal (portal.firstsolar.com)\n  — First Solar''s own host and its own OIDC issuer. The endpoints and the scope vocabulary are Salesforce\n  platform-standard, not a First Solar-authored API contract: First Solar publishes no API product of\n  its own. Recorded because it is a real, unauthenticated, machine-readable document the provider serves.'\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  pkce:\n  - S256\n  dpop:\n  - RS256\n  - RS384\n  - RS512\n  - ES256\n  - ES384\n  -\
  \ ES512\n  - EdDSA\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://portal.firstsolar.com/.well-known/openid-configuration\n  issuer: https://portal.firstsolar.com/developer\n  jwks_uri: https://portal.firstsolar.com/developer/id/keys\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - active\n  - address\n  - email\n  - email_verified\n  - family_name\n  - given_name\n  - is_app_installed\n  - language\n  - locale\n  - name\n  - nickname\n  - organization_id\n  - phone_number\n  - phone_number_verified\n  - photos\n  - picture\n  - preferred_username\n  - profile\n  - sub\n  - updated_at\n  - urls\n  - user_id\n  - user_type\n  - zoneinfo\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.firstsolar.com/developer/services/oauth2/authorize\n    tokenUrl: https://portal.firstsolar.com/developer/services/oauth2/token\n\
  \    refreshUrl: https://portal.firstsolar.com/developer/services/oauth2/token\n    scope_count: 36\n  introspection_endpoint: https://portal.firstsolar.com/developer/services/oauth2/introspect\n  revocation_endpoint: https://portal.firstsolar.com/developer/services/oauth2/revoke\n  registration_endpoint: https://portal.firstsolar.com/developer/services/oauth2/register\n  end_session_endpoint: https://portal.firstsolar.com/developer/services/auth/idp/oidc/logout\n  userinfo_endpoint: https://portal.firstsolar.com/developer/services/oauth2/userinfo\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  sources:\n  - well-known/first-solar-openid-configuration.json\nx-evidence:\n- url: https://portal.firstsolar.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-09-10'\n- url: https://portal.firstsolar.com/developer/id/keys\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-09-10'\n  note: JWKS\
  \ returns real RSA signing keys\n- url: https://portal.firstsolar.com/developer/services/oauth2/token\n  http_status: 400\n  fetched: '2026-09-10'\n  note: unauthenticated POST returns RFC 6749 {\"error\":\"unsupported_grant_type\"} — endpoint is live\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-solar/refs/heads/main/authentication/first-solar-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Solar
- Energy
- Renewable Energy
- Manufacturing
- Fortune 1000
- Photovoltaic
- Thin Film
- Utility-Scale Solar
- Clean Energy
---
