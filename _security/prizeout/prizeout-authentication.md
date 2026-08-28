---
api_key_in: []
auth_types: []
description: 'Prizeout has no public OpenAPI, so no securityScheme could be derived. The authentication model is reconstructed from the two first-party SDK integration wikis Prizeout publishes on GitHub and from a partner platform (LiveLike) that documents the four credentials Prizeout issues. The model is shared-secret / API-key, not OAuth: there is no authorization server, no scope surface, and no /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any Prizeout host (both probed 404 on 2026-08-26).'
kind: authentication
layout: security
method: searched
name: Prizeout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prizeout declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Prizeout
provider_slug: prizeout
scheme_count: 3
schemes:
- description: Partner API key passed to the SDK at initialisation alongside partnerId. Issued from the Prizeout Partners Dashboard under Account Settings. Prizeout issues two sets - sandbox credentials for initial testing and production credentials once integration and testing are complete.
  evidence: setCredentials(sessionId:partnerId:partnerName:apiKey:userId:email:balance:environment:) in the Swift SDK wiki
  id: partner_api_key
  in: sdk-credential
  name: apiKey
  type: apiKey
- description: Server-side secret, distinct from the API key. Documented by LiveLike as one of the four values a partner enters to connect Prizeout. Not passed to the client SDK.
  evidence: https://docs.livelike.com/docs/prizeout-integration - "Partner ID, API Key, API Secret Key, and HTTP Security Token"
  id: partner_api_secret
  in: server-side
  name: API Secret Key
  type: apiKey
- description: Shared token Prizeout presents when it calls the partner-hosted callback endpoints (balance check, session, cash-out success, cash-out failure), so the partner can authenticate the inbound request. This is the reverse direction from the API key - it authenticates PRIZEOUT to the PARTNER. The exact header name is not published publicly.
  evidence: https://docs.livelike.com/docs/prizeout-integration
  gap: Header name and signature algorithm are not documented on any public Prizeout surface.
  id: http_security_token
  in: header
  name: HTTP Security Token
  type: apiKey
slug: prizeout-authentication
source_filename: prizeout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: 'https://github.com/prizeout/swift-builds/wiki/How-To-Integrate ; https://github.com/prizeout/android-sdk-builds/wiki/How-To-Integrate ; https://docs.livelike.com/docs/prizeout-integration'\ndocs: https://github.com/prizeout/swift-builds/wiki/How-To-Integrate\nname: Prizeout Authentication\ndescription: >-\n  Prizeout has no public OpenAPI, so no securityScheme could be derived. The authentication model is\n  reconstructed from the two first-party SDK integration wikis Prizeout publishes on GitHub and from\n  a partner platform (LiveLike) that documents the four credentials Prizeout issues. The model is\n  shared-secret / API-key, not OAuth: there is no authorization server, no scope surface, and no\n  /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any Prizeout host\n  (both probed 404 on 2026-08-26).\nschemes:\n- id: partner_api_key\n  type: apiKey\n  in: sdk-credential\n  name: apiKey\n  description:\
  \ >-\n    Partner API key passed to the SDK at initialisation alongside partnerId. Issued from the\n    Prizeout Partners Dashboard under Account Settings. Prizeout issues two sets - sandbox\n    credentials for initial testing and production credentials once integration and testing are\n    complete.\n  evidence: 'setCredentials(sessionId:partnerId:partnerName:apiKey:userId:email:balance:environment:) in the Swift SDK wiki'\n- id: partner_api_secret\n  type: apiKey\n  in: server-side\n  name: API Secret Key\n  description: >-\n    Server-side secret, distinct from the API key. Documented by LiveLike as one of the four values\n    a partner enters to connect Prizeout. Not passed to the client SDK.\n  evidence: 'https://docs.livelike.com/docs/prizeout-integration - \"Partner ID, API Key, API Secret Key, and HTTP Security Token\"'\n- id: http_security_token\n  type: apiKey\n  in: header\n  name: HTTP Security Token\n  description: >-\n    Shared token Prizeout presents when it calls the\
  \ partner-hosted callback endpoints (balance\n    check, session, cash-out success, cash-out failure), so the partner can authenticate the inbound\n    request. This is the reverse direction from the API key - it authenticates PRIZEOUT to the\n    PARTNER. The exact header name is not published publicly.\n  evidence: 'https://docs.livelike.com/docs/prizeout-integration'\n  gap: 'Header name and signature algorithm are not documented on any public Prizeout surface.'\nidentity_fields:\n- name: partnerId\n  description: 'Partner/publisher identifier (a UUID in the JavaScript SDK - settings.publisher.id or settings.partner_id).'\n- name: partnerName\n  description: 'Human-readable partner name (iOS SDK only).'\n- name: sessionId\n  description: 'Per-user session identifier the partner mints and Prizeout validates back against the partner session callback.'\n- name: userId\n  description: 'Partner-scoped user identifier.'\n- name: email\n  description: 'End-user email; the gift card is delivered\
  \ to it.'\n- name: balance\n  description: >-\n    Cash-out balance in minor units, or a balanceMin/balanceMax range, or one of the pre-set\n    BalanceBin enums (11 bins in iOS, 10 in Android, from min000_max10000 to min5000000_maxUnlimited).\n    A bin lets a partner disclose a range instead of an exact balance.\noauth2: false\nopenid_connect: false\nmtls: false\nscopes: none\nnotes:\n- 'scopes/ was deliberately not authored: Prizeout has no OAuth surface, so an OAuthScopes artifact\n  would be an empty shape. derive-oauth-scopes.py confirmed 0 oauth2 schemes.'\n- 'The backend hosts named in the widget bootstrap (py-merchant-portal-api.prizeout.com and the\n  brand API on Cloud Run) return HTTP 403 to anonymous requests on every path probed, including\n  /openapi.json, /docs, /redoc and /graphql. They are real Prizeout services but are not a public\n  API surface.'\ngaps:\n- 'No public authentication reference page. The only published auth documentation is inside two\n  GitHub wikis\
  \ for SDKs described as being in private testing.'\n- 'Credential rotation, expiry and revocation are undocumented.'\n- 'No signature scheme is published for the partner callbacks, so a partner has only a shared bearer\n  token to distinguish a genuine Prizeout cash-out callback from a forged one.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prizeout/refs/heads/main/authentication/prizeout-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Advertising
- Rewards
- Gift Cards
- Payouts
- Financial Services
- Credit Unions
- Banking
- Loyalty
- Embedded Finance
- AdTech
- FinTech
---
