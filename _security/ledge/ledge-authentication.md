---
api_key_in: []
api_specs:
- filename: ledge-api-openapi.yml
  format: yaml
  label: Ledge API
  slug: ledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/openapi/ledge-api-openapi.yml
auth_types:
- oauth2
description: Ledge authenticates API callers with an OAuth 2.0 client_credentials grant issued by its Auth0 tenant, and authorizes them with a role-based fine-grained permissions model rather than with token scopes. Human access to the web application supports enterprise SAML 2.0 SSO with SCIM 2.0 provisioning.
kind: authentication
layout: security
method: searched
name: Ledge Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ledge secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ledge
provider_slug: ledge
scheme_count: 1
schemes:
- credential_source: Client ID and client secret are obtained on the Ledge Developers page at https://app.goledge.io/developers, which also shows the Organization ID (orgId) required as a path segment on every operation.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://goledge.us.auth0.com/oauth/token
  identity_provider:
    custom_domain: https://auth.goledge.io
    discovery:
    - well-known/ledge-openid-configuration.json
    - well-known/ledge-oauth-authorization-server.json
    - well-known/ledge-auth-openid-configuration.json
    tenant: https://goledge.us.auth0.com
    vendor: Auth0
  name: oauth2ClientCredentials
  presentation: 'Authorization: Bearer <access_token>'
  primary: true
  request:
    content_type: application/x-www-form-urlencoded
    method: POST
    parameters:
    - grant_type=client_credentials
    - client_id
    - client_secret
    - audience
    url: https://goledge.us.auth0.com/oauth/token
  response_fields:
  - access_token
  - token_type
  - expires_in
  sources:
  - https://docs.ledge.co/api-reference/fundamentals/authentication
  - openapi/ledge-api-openapi.yml
  token_lifetime_note: Observed in the documented example response; Ledge does not publish a guaranteed lifetime, so refresh on 401 rather than assuming this value.
  token_lifetime_seconds: 10800
  token_type: Bearer
  type: oauth2
slug: ledge-authentication
source_filename: ledge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://docs.ledge.co/api-reference/fundamentals/authentication and\n  https://docs.ledge.co/api-reference/fundamentals/fine-grained-permissions,\n  corroborated by the live Auth0 discovery documents in well-known/ and by\n  openapi/ledge-api-openapi.yml.\ndocs: https://docs.ledge.co/api-reference/fundamentals/authentication\ndescription: >-\n  Ledge authenticates API callers with an OAuth 2.0 client_credentials grant\n  issued by its Auth0 tenant, and authorizes them with a role-based fine-grained\n  permissions model rather than with token scopes. Human access to the web\n  application supports enterprise SAML 2.0 SSO with SCIM 2.0 provisioning.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  scopes_published: false\n  authorization_model: role-based fine-grained permissions\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  primary: true\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://goledge.us.auth0.com/oauth/token\n    scopes: 0\n  credential_source: >-\n    Client ID and client secret are obtained on the Ledge Developers page at\n    https://app.goledge.io/developers, which also shows the Organization ID\n    (orgId) required as a path segment on every operation.\n  request:\n    method: POST\n    url: https://goledge.us.auth0.com/oauth/token\n    content_type: application/x-www-form-urlencoded\n    parameters:\n    - grant_type=client_credentials\n    - client_id\n    - client_secret\n    - audience\n  response_fields: [access_token, token_type, expires_in]\n  token_type: Bearer\n  token_lifetime_seconds: 10800\n  token_lifetime_note: >-\n    Observed in the documented example response; Ledge does not publish a\n    guaranteed lifetime, so refresh on 401 rather than assuming this value.\n  presentation: 'Authorization: Bearer <access_token>'\n  identity_provider:\n    vendor: Auth0\n    tenant: https://goledge.us.auth0.com\n    custom_domain:\
  \ https://auth.goledge.io\n    discovery:\n    - well-known/ledge-openid-configuration.json\n    - well-known/ledge-oauth-authorization-server.json\n    - well-known/ledge-auth-openid-configuration.json\n  sources:\n  - https://docs.ledge.co/api-reference/fundamentals/authentication\n  - openapi/ledge-api-openapi.yml\nauthorization:\n  model: role-based fine-grained permissions\n  docs: https://docs.ledge.co/api-reference/fundamentals/fine-grained-permissions\n  description: >-\n    Administrators define permissions that fit their organization's needs with\n    role-based access, using either built-in or custom roles. There are no named\n    OAuth scopes on the access token; the role attached to the principal decides\n    what data is available.\n  builtin_roles:\n  - name: Administrator\n    access: Full access to all resources; user management control\n  - name: Full member\n    access: Full access to all resources\n  - name: View-only\n    access: Read-only access to all resources\n\
  \  custom_roles: >-\n    Custom roles can be used to allow, or deny, access to specific resources.\n  failure_mode: >-\n    A role that denies a resource yields HTTP 403 (\"The request was rejected for\n    security reasons\"), which is not retryable.\n  detail: scopes/ledge-scopes.yml\nenterprise_sso:\n  saml:\n    supported: true\n    version: '2.0'\n    docs: https://docs.ledge.co/authentication/how-to-guide-configure-saml-sso-with-ledge\n    acs_url: https://auth.goledge.io/login/callback?connection={your-ledge-workspace}\n    sp_entity_id: urn:auth0:goledge:{your-ledge-workspace}\n    nameid_format: urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress\n    signature_algorithm: RSA-SHA256\n    required_claims:\n    - http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress\n    - http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname\n    - http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname\n    - http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\n\
  \    idps_documented: [Okta, JumpCloud, Microsoft Entra ID, Google Workspace, OneLogin]\n    setup: >-\n      IdP metadata is sent to the customer's Ledge Customer Experience Manager to\n      complete configuration — there is no self-serve SSO setup.\n  scim:\n    supported: true\n    version: '2.0'\n    docs: https://docs.ledge.co/authentication/how-to-guide-configure-scim-provisioning-with-ledge\n    auth: Bearer token, per SCIM 2.0\n    base_url: Issued per-account by Ledge (not a published URL)\n    enablement: >-\n      SCIM is enabled per account by the customer's Ledge Customer Experience\n      Manager, who provides the SCIM Bearer Token and SCIM Base URL.\n    schemas: SCIM core and Enterprise schemas\n    limitations:\n    - Group membership is not synced — Ledge does not consume the SCIM /groups endpoint.\n    - Custom schema extensions are not consumed.\nnotes:\n- >-\n  The API host api.goledge.io serves no /.well-known/ discovery document; the\n  OAuth metadata lives on the\
  \ Auth0 tenant.\n- >-\n  Ledge publishes no API-key-only authentication path. The Getting Started page\n  and the 401 message refer to an \"API key\", but the documented mechanism is\n  the OAuth client credential pair.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/authentication/ledge-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Accounting
- Reconciliation
- Financial Close
- Payment Operations
- Transaction Matching
- Cash Application
- Journal Entries
- AI Agents
- ERP Integration
- Finance Automation
---
