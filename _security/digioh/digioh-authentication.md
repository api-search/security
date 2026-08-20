---
api_key_in:
- path
- header
- body
auth_types:
- tenantIdentifier
- http-basic
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Digioh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digioh secures its APIs with tenantIdentifier, http-basic, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Digioh
provider_slug: digioh
scheme_count: 4
schemes:
- direction: client-side
  in: path
  name: ClientGUID
  parameter: '{CLIENT_GUID}'
  secret: false
  secret_note: This value is visible in public page source and in the CDN request path, so it identifies a tenant but authenticates nothing. It is retrievable in the Digioh UI under the profile menu and is visible to Admin users only (not subusers), per the WordPress plugin installation notes.
  sources:
  - https://wordpress.org/plugins/digioh/
  - https://github.com/digioh/digioh-ios-sdk
  type: tenantIdentifier
  where: Embedded in the loader URL https://www.lightboxcdn.com/vendor/{CLIENT_GUID}/lightbox_inline.js, passed as userGId to DigiohWeb()/Digioh() in the iOS and Android SDKs, and entered as the "Client GUID" / "Client ID" setting in the WordPress plugin.
- direction: outbound
  name: OutboundBasicAuth
  scheme: basic
  secret: true
  sources:
  - https://help.digioh.com/docs/digioh-rest-api
  type: http
  where: '"Basic Auth Username" and "Basic Auth Password" fields on the Advanced screen of an API Form POST integration. Digioh sends these to the customer''s endpoint; they may be left blank.'
- direction: outbound
  in: header
  name: OutboundHeaderCredential
  parameter: Authorization (or any header name the customer configures)
  secret: true
  sources:
  - https://help.digioh.com/docs/digioh-rest-api
  type: apiKey
  where: Free-form HTTP header key/value pairs on the same Advanced screen, described by Digioh as the usual place to put "an api key or auth token". Header fields may be left blank.
- direction: outbound
  name: DestinationPlatformCredentials
  secret: true
  sources:
  - https://help.digioh.com/docs/understanding-digioh-pipelines
  type: apiKey
  where: Digioh Pipelines and the legacy integrations store per-destination credentials for Klaviyo, Iterable, Braze, Attentive, Ometria, HubSpot, Salesforce, Yotpo, Marketo and others, entered by the customer when connecting the account. Each is the destination platform's own credential, not a Digioh-issued one.
slug: digioh-authentication
source_filename: digioh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://help.digioh.com/docs/digioh-rest-api, https://help.digioh.com/knowledgebase/security-and-compliance/,\n  https://github.com/digioh/digioh-ios-sdk, https://github.com/digioh/digioh-android-sdk,\n  https://wordpress.org/plugins/digioh/\ndocs: https://help.digioh.com/docs/digioh-rest-api\nderived_from_spec: false\nderivation_note: >-\n  0-working/derive-authentication.py was run and produced no profile - there is no OpenAPI or Swagger\n  document in this repo to derive securitySchemes from, because Digioh publishes none. This file is\n  authored from the provider's own documentation and from the shipped SDK signatures, and is marked\n  searched accordingly.\nsummary:\n  types: [tenantIdentifier, http-basic, apiKey]\n  api_key_in: [path, header, body]\n  oauth2_flows: []\n  note: >-\n    Digioh issues no API credential to a developer. There is no public inbound API, so there is no\n    inbound auth scheme. What exists\
  \ is (a) a non-secret account Client GUID that keys the widget\n    runtime and the mobile SDKs, and (b) pass-through credential fields where Digioh presents the\n    CUSTOMER's credentials to the CUSTOMER's own endpoint on an outbound form post.\nschemes:\n- name: ClientGUID\n  type: tenantIdentifier\n  direction: client-side\n  in: path\n  parameter: '{CLIENT_GUID}'\n  where: >-\n    Embedded in the loader URL https://www.lightboxcdn.com/vendor/{CLIENT_GUID}/lightbox_inline.js,\n    passed as userGId to DigiohWeb()/Digioh() in the iOS and Android SDKs, and entered as the\n    \"Client GUID\" / \"Client ID\" setting in the WordPress plugin.\n  secret: false\n  secret_note: >-\n    This value is visible in public page source and in the CDN request path, so it identifies a\n    tenant but authenticates nothing. It is retrievable in the Digioh UI under the profile menu and\n    is visible to Admin users only (not subusers), per the WordPress plugin installation notes.\n  sources: [https://wordpress.org/plugins/digioh/,\
  \ https://github.com/digioh/digioh-ios-sdk]\n- name: OutboundBasicAuth\n  type: http\n  scheme: basic\n  direction: outbound\n  where: >-\n    \"Basic Auth Username\" and \"Basic Auth Password\" fields on the Advanced screen of an API Form POST\n    integration. Digioh sends these to the customer's endpoint; they may be left blank.\n  secret: true\n  sources: [https://help.digioh.com/docs/digioh-rest-api]\n- name: OutboundHeaderCredential\n  type: apiKey\n  in: header\n  parameter: Authorization (or any header name the customer configures)\n  direction: outbound\n  where: >-\n    Free-form HTTP header key/value pairs on the same Advanced screen, described by Digioh as the\n    usual place to put \"an api key or auth token\". Header fields may be left blank.\n  secret: true\n  sources: [https://help.digioh.com/docs/digioh-rest-api]\n- name: DestinationPlatformCredentials\n  type: apiKey\n  direction: outbound\n  where: >-\n    Digioh Pipelines and the legacy integrations store per-destination\
  \ credentials for Klaviyo,\n    Iterable, Braze, Attentive, Ometria, HubSpot, Salesforce, Yotpo, Marketo and others, entered by\n    the customer when connecting the account. Each is the destination platform's own credential, not\n    a Digioh-issued one.\n  secret: true\n  sources: [https://help.digioh.com/docs/understanding-digioh-pipelines]\naccount_authentication:\n  sso:\n    supported: true\n    providers_named: [Okta, Azure AD, Google Workspace]\n    protocol: not-published\n    self_serve: false\n    note: Enablement requires Digioh Support or a Customer Success Manager; no metadata or discovery endpoint is served.\n  mfa:\n    supported: true\n    note: Offered on enterprise and team accounts, enabled via Digioh support.\n  roles:\n    supported: true\n    source: https://help.digioh.com/docs/account-management-digioh-user-roles\n    note: Role-based access with an Admin/subuser distinction; activity logging documented separately.\n  login_url: https://account.digioh.com/\n  probe_note:\
  \ >-\n    account.digioh.com answers 302 to /Box/List for every anonymous path and then 403, so no\n    unauthenticated auth metadata is observable.\noauth2: []\ngaps:\n- No developer-issued API key exists, so there is no key rotation, scoping or revocation contract to document.\n- No OAuth 2.0 or OpenID Connect surface; /.well-known/openid-configuration returns 404 on every host.\n- SSO protocol is never named in public documentation.\nevidence:\n- {url: 'https://help.digioh.com/docs/digioh-rest-api', status: 200, fetched: '2026-08-12'}\n- {url: 'https://help.digioh.com/knowledgebase/security-and-compliance/', status: 200, fetched: '2026-08-12'}\n- {url: 'https://account.digioh.com/.well-known/openid-configuration', status: 302, fetched: '2026-08-12'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digioh/refs/heads/main/authentication/digioh-authentication.yml
summary_line: tenantIdentifier/http-basic/apiKey · 4 schemes
tags:
- Company
- Marketing
- E-Commerce
- Personalization
- Zero-Party Data
- Forms
- Popups
- Quizzes
- Conversion Rate Optimization
- Identity Resolution
---
