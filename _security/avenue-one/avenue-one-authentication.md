---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Avenue One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avenue One declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Avenue One
provider_slug: avenue-one
scheme_count: 1
schemes:
- authorization_endpoint: https://avenueone.us.auth0.com/authorize
  device_authorization_endpoint: https://avenueone.us.auth0.com/oauth/device/code
  flows:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  - device_code
  issuer: https://avenueone.us.auth0.com/
  jwks_uri: https://avenueone.us.auth0.com/.well-known/jwks.json
  mfa:
    challenge_endpoint: https://avenueone.us.auth0.com/mfa/challenge
  name: auth0-oidc
  observed_login_request:
    edge: 'AWS ALB OIDC authentication in front of CloudFront (server: awselb/2.0)'
    note: Scopes and role gate observed in the 302 Location header that partners.avenueone.com issues to the Auth0 tenant.
    redirect_uri: https://partners.avenueone.com/oauth2/idpresponse
    required_role: Partner Portal
    response_type: code
    scope: openid profile email groups
  openid_configuration: https://avenueone.us.auth0.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  protocol: OpenID Connect 1.0 / OAuth 2.0
  provider: Auth0
  registration_endpoint: https://avenueone.us.auth0.com/oidc/register
  revocation_endpoint: https://avenueone.us.auth0.com/oauth/revoke
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  token_endpoint: https://avenueone.us.auth0.com/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://avenueone.us.auth0.com/userinfo
slug: avenue-one-authentication
source_filename: avenue-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://avenueone.us.auth0.com/.well-known/openid-configuration\nnote: >-\n  Avenue One publishes no OpenAPI, so there are no securitySchemes to derive from.\n  This profile is probed from the only publicly readable authentication surface the\n  company exposes: the Auth0 tenant that fronts the Partner Portal. It describes how\n  humans sign in to AvenueOS — it is NOT a documented developer authentication model,\n  and Avenue One does not publish one.\napplies_to: >-\n  Partner Portal (partners.avenueone.com) and the AvenueOS product hosts\n  (credit.avenueone.com and its app/builder/investor portals).\nschemes:\n- name: auth0-oidc\n  type: openIdConnect\n  protocol: OpenID Connect 1.0 / OAuth 2.0\n  provider: Auth0\n  issuer: https://avenueone.us.auth0.com/\n  openid_configuration: https://avenueone.us.auth0.com/.well-known/openid-configuration\n  jwks_uri: https://avenueone.us.auth0.com/.well-known/jwks.json\n  authorization_endpoint:\
  \ https://avenueone.us.auth0.com/authorize\n  token_endpoint: https://avenueone.us.auth0.com/oauth/token\n  userinfo_endpoint: https://avenueone.us.auth0.com/userinfo\n  revocation_endpoint: https://avenueone.us.auth0.com/oauth/revoke\n  device_authorization_endpoint: https://avenueone.us.auth0.com/oauth/device/code\n  registration_endpoint: https://avenueone.us.auth0.com/oidc/register\n  flows:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n  - device_code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  mfa:\n    challenge_endpoint: https://avenueone.us.auth0.com/mfa/challenge\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n  observed_login_request:\n    note: >-\n      Scopes and role gate observed in the 302 Location header that\n      partners.avenueone.com\
  \ issues to the Auth0 tenant.\n    scope: openid profile email groups\n    required_role: Partner Portal\n    response_type: code\n    redirect_uri: https://partners.avenueone.com/oauth2/idpresponse\n    edge: 'AWS ALB OIDC authentication in front of CloudFront (server: awselb/2.0)'\ndeveloper_authentication:\n  documented: false\n  api_keys: false\n  public_docs: false\n  note: >-\n    No developer portal, API key issuance, or published authentication guide was\n    found on any Avenue One host. Access to AvenueOS requires a partner/investor\n    account provisioned by Avenue One.\nx-evidence:\n- url: https://partners.avenueone.com/\n  http_status: 302\n  checked: '2026-08-06'\n  note: 302 to the Auth0 universal login (avenueone.us.auth0.com)\n- url: https://avenueone.us.auth0.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n  checked: '2026-08-06'\n- url: https://avenueone.us.auth0.com/.well-known/jwks.json\n  http_status: 200\n\
  \  checked: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avenue-one/refs/heads/main/authentication/avenue-one-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real Estate
- Single-Family Rental
- PropTech
- Institutional Investing
- Lending
- Asset Management
- Property Data
- Marketplace
---
