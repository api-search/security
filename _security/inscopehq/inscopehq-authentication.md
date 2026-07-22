---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Inscopehq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Inscope secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Inscope
provider_slug: inscopehq
scheme_count: 2
schemes:
- issuer: https://auth.inscopehq.com
  name: openIdConnect
  openIdConnectUrl: https://auth.inscopehq.com/.well-known/openid-configuration
  sources:
  - well-known/inscopehq-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.inscopehq.com/propelauth/oauth/authorize
    flow: authorizationCode
    scopes:
      email: Access to the user's email address
      openid: OpenID Connect authentication
      profile: Access to basic profile claims (first_name, last_name, picture_url)
    tokenUrl: https://auth.inscopehq.com/propelauth/oauth/token
    userinfoUrl: https://auth.inscopehq.com/propelauth/oauth/userinfo
  name: oauth2
  sources:
  - well-known/inscopehq-openid-configuration.json
  type: oauth2
slug: inscopehq-authentication
source_filename: inscopehq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.inscopehq.com/.well-known/openid-configuration\ndocs: https://www.inscopehq.com/security-privacy-and-trust\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  identity_provider: PropelAuth (hosted tenant at auth.inscopehq.com)\n  pkce: S256\n  notes: >-\n    This profile describes Inscope's application sign-in surface (OIDC), the\n    only authorization surface published publicly. Inscope exposes no public\n    product API, so there is no API-key or bearer-token developer auth to\n    document. Machine-to-machine access, if any, is not publicly documented.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.inscopehq.com/.well-known/openid-configuration\n  issuer: https://auth.inscopehq.com\n  sources: [well-known/inscopehq-openid-configuration.json]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://auth.inscopehq.com/propelauth/oauth/authorize\n    tokenUrl: https://auth.inscopehq.com/propelauth/oauth/token\n    userinfoUrl: https://auth.inscopehq.com/propelauth/oauth/userinfo\n    scopes:\n      openid: OpenID Connect authentication\n      email: Access to the user's email address\n      profile: Access to basic profile claims (first_name, last_name, picture_url)\n  sources: [well-known/inscopehq-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inscopehq/refs/heads/main/authentication/inscopehq-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Financial Reporting
- Accounting
- Audit
- Artificial Intelligence
- Fintech
- Financial Close
- GAAP
- SaaS
---
