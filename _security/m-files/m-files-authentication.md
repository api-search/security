---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: M Files Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: M-Files secures its APIs with oauth2, apiKey, and http across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: M-Files
provider_slug: m-files
scheme_count: 6
schemes:
- description: Recommended method. POST username, password, and vault GUID (in braces) to /REST/server/authenticationtokens; the JSON response returns a token value passed on every subsequent request via the X-Authentication header. Optional Expiration (ISO 8601) and SessionID. A 403 indicates an expired token.
  header: X-Authentication
  in: header
  name: AuthenticationToken
  obtain: POST /REST/server/authenticationtokens
  type: apiKey
- description: 'OAuth 2.0 access token passed as Authorization: Bearer <access-token>. Used when the vault / M-Files Server is configured with an OAuth identity provider (e.g. Azure AD / Microsoft Entra ID).'
  name: OAuth2Bearer
  scheme: bearer
  type: oauth2
- description: Not recommended. Credentials passed directly as X-Username, X-Password, and X-Vault headers on each request.
  header: X-Username
  in: header
  name: HttpHeaderCredentials
  type: apiKey
- description: ASP.NET session cookie returned after authentication, typically used for single sign-on scenarios; preserve cookies for Multi-Server Mode stickiness.
  name: CookieSession
  scheme: cookie
  type: http
- description: Single Sign-On (SSO) against the configured identity provider; see https://developer.m-files.com/APIs/REST-API/Authentication/Single-Sign-On/
  name: SingleSignOn
  type: oauth2
- description: Pre-shared key authentication; see https://developer.m-files.com/APIs/REST-API/Authentication/Pre-Shared-Keys/
  in: header
  name: PreSharedKeys
  type: apiKey
slug: m-files-authentication
source_filename: m-files-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.m-files.com/APIs/REST-API/Authentication/\ndocs: https://developer.m-files.com/APIs/REST-API/Authentication/\nnotes: >-\n  The M-Files Web Service (MFWS) REST API is hosted per M-Files Server (on-prem or\n  M-Files Cloud vault), so endpoints are relative to the customer's Web Access root\n  (e.g. /REST/...). Authentication is session/token based rather than a fixed public\n  OAuth server; OAuth bearer is supported where the vault is configured for it.\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  api_key_header: X-Authentication\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: AuthenticationToken\n    type: apiKey\n    in: header\n    header: X-Authentication\n    obtain: POST /REST/server/authenticationtokens\n    description: >-\n      Recommended method. POST username, password, and vault GUID (in braces) to\n      /REST/server/authenticationtokens; the JSON response returns\
  \ a token value\n      passed on every subsequent request via the X-Authentication header. Optional\n      Expiration (ISO 8601) and SessionID. A 403 indicates an expired token.\n  - name: OAuth2Bearer\n    type: oauth2\n    scheme: bearer\n    description: >-\n      OAuth 2.0 access token passed as Authorization: Bearer <access-token>. Used\n      when the vault / M-Files Server is configured with an OAuth identity provider\n      (e.g. Azure AD / Microsoft Entra ID).\n  - name: HttpHeaderCredentials\n    type: apiKey\n    in: header\n    header: X-Username\n    description: >-\n      Not recommended. Credentials passed directly as X-Username, X-Password, and\n      X-Vault headers on each request.\n  - name: CookieSession\n    type: http\n    scheme: cookie\n    description: >-\n      ASP.NET session cookie returned after authentication, typically used for\n      single sign-on scenarios; preserve cookies for Multi-Server Mode stickiness.\n  - name: SingleSignOn\n    type: oauth2\n \
  \   description: >-\n      Single Sign-On (SSO) against the configured identity provider; see\n      https://developer.m-files.com/APIs/REST-API/Authentication/Single-Sign-On/\n  - name: PreSharedKeys\n    type: apiKey\n    in: header\n    description: >-\n      Pre-shared key authentication; see\n      https://developer.m-files.com/APIs/REST-API/Authentication/Pre-Shared-Keys/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m-files/refs/heads/main/authentication/m-files-authentication.yml
summary_line: oauth2/apiKey/http · 6 schemes
tags:
- Company
- Infrastructure Saas
- Document Management
- Information Management
- Content Services
- Workflow Automation
- Compliance
- Enterprise Content Management
---
