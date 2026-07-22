---
api_key_in: []
api_specs:
- filename: sign-in-enterprise-guest-api-openapi-original.yml
  format: yaml
  label: Sign In Solutions VMS API
  slug: sign-in-solutions-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sign-in-enterprise/refs/heads/main/openapi/sign-in-enterprise-guest-api-openapi-original.yml
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sign In Enterprise Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sign In Enterprise secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sign In Enterprise
provider_slug: sign-in-enterprise
scheme_count: 1
schemes:
- authorization_endpoint: https://us.tractionguest.com/oauth/authorize
  introspection_endpoint: https://us.tractionguest.com/oauth/introspect
  issuer: https://us.tractionguest.com
  jwks_uri: https://us.tractionguest.com/oauth/discovery/keys
  name: TractionGuestAuth
  openIdConnectUrl: https://us.tractionguest.com/.well-known/openid-configuration
  revocation_endpoint: https://us.tractionguest.com/oauth/revoke
  scheme: bearer
  scopes_reference: scopes/sign-in-enterprise-scopes.yml
  sources:
  - openapi/sign-in-enterprise-guest-api-openapi-original.yml
  - well-known/sign-in-enterprise-openid-configuration.json
  token_endpoint: https://us.tractionguest.com/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://us.tractionguest.com/oauth/userinfo
slug: sign-in-enterprise-authentication
source_filename: sign-in-enterprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sign-in-enterprise-guest-api-openapi-original.yml\ndocs: https://developers.signinenterprise.com/\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: TractionGuestAuth\n  type: openIdConnect\n  scheme: bearer\n  openIdConnectUrl: https://us.tractionguest.com/.well-known/openid-configuration\n  issuer: https://us.tractionguest.com\n  authorization_endpoint: https://us.tractionguest.com/oauth/authorize\n  token_endpoint: https://us.tractionguest.com/oauth/token\n  revocation_endpoint: https://us.tractionguest.com/oauth/revoke\n  introspection_endpoint: https://us.tractionguest.com/oauth/introspect\n  userinfo_endpoint: https://us.tractionguest.com/oauth/userinfo\n  jwks_uri: https://us.tractionguest.com/oauth/discovery/keys\n  scopes_reference: scopes/sign-in-enterprise-scopes.yml\n  sources:\n  - openapi/sign-in-enterprise-guest-api-openapi-original.yml\n  - well-known/sign-in-enterprise-openid-configuration.json\n\
  notes: >\n  The Sign In Solutions VMS API authenticates every request with an OAuth 2.0 /\n  OpenID Connect bearer token. Access is limited-release; contact support to obtain\n  client credentials. Tokens carry fine-grained resource scopes (see scopes/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sign-in-enterprise/refs/heads/main/authentication/sign-in-enterprise-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Vertical Software
- Visitor Management
- Physical Security
- Workplace Experience
- Identity
- Compliance
- Access Control
---
