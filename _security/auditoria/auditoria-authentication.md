---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: Auditoria Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- tokenExchange
- jwtBearer
- implicit
- password
overview: Auditoria.AI secures its APIs with openIdConnect, oauth2, and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, tokenExchange, jwtBearer, implicit, and password flow(s).
provider_name: Auditoria.AI
provider_slug: auditoria
scheme_count: 3
schemes:
- backchannel_logout: true
  dpop:
    algs:
    - ES256
    supported: true
  endpoints:
    authorization: https://auth.auditoria.ai/authorize
    backchannel_authentication: https://auth.auditoria.ai/bc-authorize
    device_authorization: https://auth.auditoria.ai/oauth/device/code
    jwks: https://auth.auditoria.ai/.well-known/jwks.json
    mfa_challenge: https://auth.auditoria.ai/mfa/challenge
    registration: https://auth.auditoria.ai/oidc/register
    revocation: https://auth.auditoria.ai/oauth/revoke
    token: https://auth.auditoria.ai/oauth/token
    userinfo: https://auth.auditoria.ai/userinfo
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.auditoria.ai/
  mfa: true
  name: Auth0OIDC
  openIdConnectUrl: https://auth.auditoria.ai/.well-known/openid-configuration
  pkce:
    methods:
    - S256
    - plain
    supported: true
  provider: Auth0
  purpose: End-user and machine sign-in to the Auditoria tenant application (app.auditoria.ai)
  sources:
  - well-known/auditoria-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- docs:
  - https://docs.auditoria.ai/hc/en-us/articles/52583635034905-Single-Sign-On-SSO-Integration-Generic-SAML-Guide
  - https://docs.auditoria.ai/hc/en-us/articles/29666250326169-SSO-Integration-Microsoft-Entra-ID-Azure-SSO
  - https://docs.auditoria.ai/hc/en-us/articles/7949613654681-Okta-SSO-for-an-Auditoria-Tenant
  identity_providers_documented:
  - Okta
  - Microsoft Entra ID (Azure AD)
  - generic SAML 2.0
  name: SAML2SSO
  purpose: Customer-tenant single sign-on into Auditoria
  sources:
  - docs.auditoria.ai
  type: saml2
- docs:
  - https://docs.auditoria.ai/hc/en-us/articles/54689809797657-Auditoria-AI-Mailbox-Integration-OAuth-Overview
  - https://docs.auditoria.ai/hc/en-us/articles/4445097262361-Authenticate-Auditoria-in-Google-Workspace
  - https://docs.auditoria.ai/hc/en-us/articles/4414146361753-Configure-your-Auditoria-mailbox-for-Okta-SSO-support
  name: MailboxOAuth
  purpose: Delegated OAuth 2.0 grant so Auditoria's SmartBots can read and send from the customer's shared AP/AR mailbox (Microsoft 365 / Google Workspace) rather than storing a password.
  sources:
  - docs.auditoria.ai
  type: oauth2
slug: auditoria-authentication
source_filename: auditoria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.auditoria.ai/.well-known/openid-configuration\ndocs: https://docs.auditoria.ai/hc/en-us/categories/360003645754-Auditoria-AI-Integrations\nscope: >-\n  This profile describes how humans and connected systems authenticate TO Auditoria and how\n  Auditoria authenticates OUT to a customer's ERP and mailbox. Auditoria publishes no public\n  API, so there is no OpenAPI securityScheme to derive from - every scheme below was probed\n  live or read from the published integration documentation.\nsummary:\n  types: [openIdConnect, oauth2, saml2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken, tokenExchange, jwtBearer, implicit, password]\n  public_api_auth: none\nschemes:\n  - name: Auth0OIDC\n    type: openIdConnect\n    openIdConnectUrl: https://auth.auditoria.ai/.well-known/openid-configuration\n    issuer: https://auth.auditoria.ai/\n    provider: Auth0\n    purpose:\
  \ End-user and machine sign-in to the Auditoria tenant application (app.auditoria.ai)\n    endpoints:\n      authorization: https://auth.auditoria.ai/authorize\n      token: https://auth.auditoria.ai/oauth/token\n      userinfo: https://auth.auditoria.ai/userinfo\n      jwks: https://auth.auditoria.ai/.well-known/jwks.json\n      registration: https://auth.auditoria.ai/oidc/register\n      revocation: https://auth.auditoria.ai/oauth/revoke\n      device_authorization: https://auth.auditoria.ai/oauth/device/code\n      backchannel_authentication: https://auth.auditoria.ai/bc-authorize\n      mfa_challenge: https://auth.auditoria.ai/mfa/challenge\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n    id_token_signing_algs: [HS256, RS256, PS256]\n    pkce: {supported: true, methods: [S256, plain]}\n    dpop: {supported: true, algs: [ES256]}\n    mfa: true\n    backchannel_logout: true\n    sources: [well-known/auditoria-openid-configuration.json]\n\
  \  - name: SAML2SSO\n    type: saml2\n    purpose: Customer-tenant single sign-on into Auditoria\n    identity_providers_documented: [Okta, Microsoft Entra ID (Azure AD), generic SAML 2.0]\n    docs:\n      - https://docs.auditoria.ai/hc/en-us/articles/52583635034905-Single-Sign-On-SSO-Integration-Generic-SAML-Guide\n      - https://docs.auditoria.ai/hc/en-us/articles/29666250326169-SSO-Integration-Microsoft-Entra-ID-Azure-SSO\n      - https://docs.auditoria.ai/hc/en-us/articles/7949613654681-Okta-SSO-for-an-Auditoria-Tenant\n    sources: [docs.auditoria.ai]\n  - name: MailboxOAuth\n    type: oauth2\n    purpose: >-\n      Delegated OAuth 2.0 grant so Auditoria's SmartBots can read and send from the customer's\n      shared AP/AR mailbox (Microsoft 365 / Google Workspace) rather than storing a password.\n    docs:\n      - https://docs.auditoria.ai/hc/en-us/articles/54689809797657-Auditoria-AI-Mailbox-Integration-OAuth-Overview\n      - https://docs.auditoria.ai/hc/en-us/articles/4445097262361-Authenticate-Auditoria-in-Google-Workspace\n\
  \      - https://docs.auditoria.ai/hc/en-us/articles/4414146361753-Configure-your-Auditoria-mailbox-for-Okta-SSO-support\n    sources: [docs.auditoria.ai]\noutbound_erp_credentials:\n  note: >-\n    Auditoria is an API CONSUMER on the ERP side. The documented pattern is a dedicated\n    service account in the customer's ERP, not an Auditoria-issued credential.\n  patterns:\n    - system: Workday\n      mechanism: Integration System User (ISU) / Automated Security User (ASU) with a web-services security group\n      docs: https://docs.auditoria.ai/hc/en-us/articles/32034349717401-Setting-Up-a-Workday-ISU-for-SmartVendor-Products-AP-Invoices-and-AP-Helpdesk\n    - system: Oracle NetSuite\n      mechanism: NetSuite connection settings with a scoped business-user role\n      docs: https://docs.auditoria.ai/hc/en-us/articles/4416849866649-Oracle-NetSuite-Connection-Settings\n    - system: Sage Intacct\n      mechanism: Sage Intacct web-services connection settings with a scoped business user\n\
  \      docs: https://docs.auditoria.ai/hc/en-us/articles/4416842321305-Sage-Intacct-Connection-Settings\n    - system: Coupa\n      mechanism: Coupa connection settings\n      docs: https://docs.auditoria.ai/hc/en-us/articles/5546330161049-Coupa-Connection-Settings\n    - system: Oracle Fusion Cloud\n      mechanism: Oracle Fusion Cloud service account\n      docs: https://docs.auditoria.ai/hc/en-us/articles/60236686051481-Set-up-Oracle-Fusion-Cloud-for-Auditoria\n    - system: Universal Connector (no native ERP connector)\n      mechanism: SFTP credentials (host/port/username/password) or an AWS S3 bucket, exchanged out of band\n      docs: https://docs.auditoria.ai/hc/en-us/articles/60112878955289-Auditoria-Universal-Connector\n  tenant_token:\n    name: Auditoria source token\n    note: >-\n      A per-tenant identifier the customer copies from Administration > System Settings and\n      pastes into the ERP-side connection. It addresses an inbound Auditoria mail endpoint\n      (<sourcetoken>@invoice-inbound.auditoria.ai);\
  \ it is not an API key and grants no API access.\n    docs: https://docs.auditoria.ai/hc/en-us/articles/4584712925721-Get-your-Auditoria-Source-Token\n  byok:\n    supported: true\n    product: Auditoria Guardian\n    docs: https://docs.auditoria.ai/hc/en-us/articles/49775469453593-Auditoria-Guardian-Bring-Your-Own-Key-BYOK-Configuration\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.auditoria.ai/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auditoria/refs/heads/main/authentication/auditoria-authentication.yml
summary_line: openIdConnect/oauth2/saml2 · 3 schemes
tags:
- Company
- Artificial Intelligence
- Finance
- Accounting
- Accounts Payable
- Accounts Receivable
- Automation
- ERP
- Agents
- Software-as-a-Service
- Invoicing
- Procurement
---
