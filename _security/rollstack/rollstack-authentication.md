---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Rollstack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Rollstack secures its APIs with openIdConnect, oauth2, and saml across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Rollstack
provider_slug: rollstack
scheme_count: 2
schemes:
- authorization_endpoint: https://auth.rollstack.com/authorize
  issuer: https://auth.rollstack.com/
  jwks_uri: https://auth.rollstack.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://auth.rollstack.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - profile
  - offline_access
  - email
  - phone
  - address
  source: https://auth.rollstack.com/.well-known/openid-configuration
  token_endpoint: https://auth.rollstack.com/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://auth.rollstack.com/userinfo
- name: SAML SSO
  provider: BoxyHQ Jackson
  source: https://www.rollstack.com/security
  type: saml
  url: https://jackson.rollstack.com
slug: rollstack-authentication
source_filename: rollstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.rollstack.com/.well-known/openid-configuration, https://www.rollstack.com/security\ndocs: https://docs.rollstack.com/user-management\nsummary:\n  types: [openIdConnect, oauth2, saml]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken]\n  sso: true\nnotes: >-\n  Rollstack has no public developer REST API; authentication described here is\n  the platform sign-in / SSO surface. Identity is handled by an Auth0 tenant on\n  the custom domain auth.rollstack.com, which publishes a standard OpenID Connect\n  discovery document. Enterprise SAML single sign-on is brokered through BoxyHQ\n  Jackson (jackson.rollstack.com). Social/enterprise connections include Google\n  and Microsoft (Azure AD).\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.rollstack.com/.well-known/openid-configuration\n  issuer: https://auth.rollstack.com/\n  authorization_endpoint:\
  \ https://auth.rollstack.com/authorize\n  token_endpoint: https://auth.rollstack.com/oauth/token\n  userinfo_endpoint: https://auth.rollstack.com/userinfo\n  jwks_uri: https://auth.rollstack.com/.well-known/jwks.json\n  scopes_supported: [openid, profile, offline_access, email, phone, address]\n  source: https://auth.rollstack.com/.well-known/openid-configuration\n- name: SAML SSO\n  type: saml\n  provider: BoxyHQ Jackson\n  url: https://jackson.rollstack.com\n  source: https://www.rollstack.com/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollstack/refs/heads/main/authentication/rollstack-authentication.yml
summary_line: openIdConnect/oauth2/saml · 2 schemes
tags:
- Company
- Business Intelligence
- Reporting
- Presentations
- Documents
- Data Automation
- Analytics
- Productivity
---
