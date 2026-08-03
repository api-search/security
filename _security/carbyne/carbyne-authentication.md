---
api_key_in: []
auth_types:
- oauth2
- saml2
- password
- sso
description: ''
kind: authentication
layout: security
method: searched
name: Carbyne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carbyne secures its APIs with oauth2, saml2, password, and sso across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Carbyne
provider_slug: carbyne
scheme_count: 4
schemes:
- description: SAML-based single sign-on federation with the customer agency's identity provider.
  name: SAML
  source: https://carbyne.com/cloud-advantage/cloud-security/
  type: saml2
- description: OAuth is listed among the supported authentication methods. No public authorization or token endpoint, flow, or scope reference is published; /.well-known/oauth-authorization-server returns 404 on carbyne.com.
  flows: []
  name: OAuth
  scopes_published: false
  source: https://carbyne.com/cloud-advantage/cloud-security/
  type: oauth2
- description: Username and password login, with optional two-factor authentication (2FA) at sign-in.
  name: Password
  scheme: basic
  source: https://carbyne.com/cloud-advantage/cloud-security/
  type: http
- description: Single Sign-On across Carbyne applications within a session; authentication methods can be individually enabled or disabled per account.
  name: SSO
  source: https://carbyne.com/cloud-advantage/cloud-security/
  type: sso
slug: carbyne-authentication
source_filename: carbyne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://carbyne.com/cloud-advantage/cloud-security/\ndocs: https://carbyne.com/cloud-advantage/cloud-security/\nscope: platform\nnote: Derived nothing from OpenAPI — Carbyne publishes no machine-readable API contract.\n  This profile records the authentication model Carbyne documents publicly for its\n  platform (Authentication / Universal Login section of the Cloud Security page). API\n  credentials themselves are provisioned under contract; see the published API Terms\n  of Use.\nsummary:\n  types:\n  - oauth2\n  - saml2\n  - password\n  - sso\n  mfa: true\n  authorization_model: role-based\n  per_account_toggle: true\nschemes:\n- name: SAML\n  type: saml2\n  description: SAML-based single sign-on federation with the customer agency's identity\n    provider.\n  source: https://carbyne.com/cloud-advantage/cloud-security/\n- name: OAuth\n  type: oauth2\n  description: OAuth is listed among the supported authentication methods.\
  \ No public\n    authorization or token endpoint, flow, or scope reference is published; /.well-known/oauth-authorization-server\n    returns 404 on carbyne.com.\n  flows: []\n  scopes_published: false\n  source: https://carbyne.com/cloud-advantage/cloud-security/\n- name: Password\n  type: http\n  scheme: basic\n  description: Username and password login, with optional two-factor authentication\n    (2FA) at sign-in.\n  source: https://carbyne.com/cloud-advantage/cloud-security/\n- name: SSO\n  type: sso\n  description: Single Sign-On across Carbyne applications within a session; authentication\n    methods can be individually enabled or disabled per account.\n  source: https://carbyne.com/cloud-advantage/cloud-security/\nauthorization:\n  model: role-based\n  description: Role-Based Authorization assigns access to specific individuals for\n    different types of business transactions.\nmfa:\n  supported: true\n  description: Multi-Factor Authentication restricts access to authorized\
  \ individuals;\n    2FA available for username/password users.\napi_access:\n  public_self_service: false\n  terms: https://carbyne.com/wp-content/uploads/2023/03/Carbyne-API-Terms-of-Use.final_.3.23.23.pdf\n  description: API access is granted under Carbyne's API Terms of Use to contracted\n    customers and partners. No public developer portal, key issuance flow, or authentication\n    reference for the API was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbyne/refs/heads/main/authentication/carbyne-authentication.yml
summary_line: oauth2/saml2/password/sso · 4 schemes
tags:
- Company
- Emergency Services
- Public Safety
- Communications
- Telecommunications
- NG911
- Contact Center
- Location
- Video
- Government
- Artificial Intelligence
---
