---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'There is no single Safari API credential. Authentication is per-surface, and two of the three network surfaces use certificate- or key-based schemes rather than a bearer token or API key — which is why no OAuth or OpenID discovery document is served on any host in this record. Derived by reading the docs, not from an OpenAPI securitySchemes block: Apple publishes no OpenAPI for Safari.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apple Safari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apple Safari declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Apple Safari
provider_slug: apple-safari
scheme_count: 4
schemes:
- constraints:
  - JWT subject claim must be a URL or a mailto: URI.
  - JWT audience claim must be the origin of the push service the request is sent to.
  - JWT expiration must not be more than one day in the future.
  - Do not refresh the JWT more frequently than once per hour.
  description: The application server signs a VAPID JSON Web Token with its own private key and sends it, together with the matching VAPID public key, in the Authorization header. The public key must match the one passed to PushManager.subscribe for that subscription.
  docs: https://developer.apple.com/documentation/usernotifications/sending-web-push-notifications-in-web-apps-and-browsers
  failure_modes:
  - BadAuthorizationHeader
  - BadJwtToken
  - BadVapidPublicKey
  - VapidPkHashMismatch
  id: vapid-jwt
  location: Authorization header
  requires_paid_membership: false
  scheme: vapid
  surface: Apple Web Push service
  type: http
- constraints:
  - TLS 1.2 or later.
  - 'Cipher suite limited to: TLS_AES_128_GCM_SHA256, TLS_AES_256_GCM_SHA384, ECDHE-ECDSA-AES128-GCM-SHA256, ECDHE-RSA-AES128-GCM-SHA256, ECDHE-ECDSA-AES256-GCM-SHA384, ECDHE-RSA-AES256-GCM-SHA384.'
  - TLS Server Name Indication (SNI) required on all connections.
  - HTTPS over TCP port 443 to a strict allow list of Apple Pay gateway domains and IP ranges.
  - The returned session object expires after five minutes.
  description: '"Your server posts a request using mutual TLS (mTLS)" to the Apple Pay Payment Session endpoint, presenting the merchant identity certificate associated with the merchant ID. The request must come from the server, never from the client.'
  docs: https://developer.apple.com/documentation/applepayontheweb/requesting-an-apple-pay-payment-session
  id: apple-pay-mtls
  location: TLS client certificate
  membership_note: The merchant identity certificate is issued through an Apple Developer Program account.
  requires_paid_membership: true
  surface: Apple Pay merchant validation
  type: mutualTLS
- description: No credential. Access is authorised by the user turning on "Allow remote automation and external agents" in Safari's Developer settings on their own machine, and the driver is reachable only from that machine. Automation sessions run in isolated windows that cannot read browsing history, AutoFill data or other sensitive state.
  docs: https://developer.apple.com/documentation/webkit/about-webdriver-for-safari
  id: safaridriver-local
  location: local machine
  requires_paid_membership: false
  surface: safaridriver (W3C WebDriver + Safari MCP server)
  type: none
- description: ASWebAuthenticationSession is the client-side handoff an app uses to run an OAuth or WebAuthn flow in Safari and receive the callback. Safari is the user agent in the flow — it is not itself an authorization server, and it issues no tokens of its own. Passkeys/WebAuthn credentials are held by the platform and the relying party is the site, not Apple.
  docs: https://developer.apple.com/documentation/authenticationservices/aswebauthenticationsession
  id: aswebauthenticationsession
  requires_paid_membership: false
  surface: Safari Authentication Services API
  type: delegated
slug: apple-safari-authentication
source_filename: apple-safari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: >-\n  https://developer.apple.com/documentation/usernotifications/sending-web-push-notifications-in-web-apps-and-browsers,\n  https://developer.apple.com/documentation/applepayontheweb/requesting-an-apple-pay-payment-session,\n  https://developer.apple.com/documentation/applepayontheweb/setting-up-your-server,\n  https://developer.apple.com/documentation/authenticationservices/aswebauthenticationsession\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Apple Safari\nproviderId: apple-safari\ndescription: >-\n  There is no single Safari API credential. Authentication is per-surface, and two of the\n  three network surfaces use certificate- or key-based schemes rather than a bearer token\n  or API key — which is why no OAuth or OpenID discovery document is served on any host\n  in this record. Derived by reading the docs, not from an OpenAPI securitySchemes block:\n  Apple publishes no OpenAPI\
  \ for Safari.\nschemes:\n  - id: vapid-jwt\n    surface: Apple Web Push service\n    type: http\n    scheme: vapid\n    location: Authorization header\n    description: >-\n      The application server signs a VAPID JSON Web Token with its own private key and\n      sends it, together with the matching VAPID public key, in the Authorization header.\n      The public key must match the one passed to PushManager.subscribe for that\n      subscription.\n    constraints:\n      - JWT subject claim must be a URL or a mailto: URI.\n      - JWT audience claim must be the origin of the push service the request is sent to.\n      - JWT expiration must not be more than one day in the future.\n      - Do not refresh the JWT more frequently than once per hour.\n    failure_modes:\n      - BadAuthorizationHeader\n      - BadJwtToken\n      - BadVapidPublicKey\n      - VapidPkHashMismatch\n    docs: https://developer.apple.com/documentation/usernotifications/sending-web-push-notifications-in-web-apps-and-browsers\n\
  \    requires_paid_membership: false\n  - id: apple-pay-mtls\n    surface: Apple Pay merchant validation\n    type: mutualTLS\n    location: TLS client certificate\n    description: >-\n      \"Your server posts a request using mutual TLS (mTLS)\" to the Apple Pay Payment\n      Session endpoint, presenting the merchant identity certificate associated with the\n      merchant ID. The request must come from the server, never from the client.\n    constraints:\n      - TLS 1.2 or later.\n      - 'Cipher suite limited to: TLS_AES_128_GCM_SHA256, TLS_AES_256_GCM_SHA384, ECDHE-ECDSA-AES128-GCM-SHA256, ECDHE-RSA-AES128-GCM-SHA256, ECDHE-ECDSA-AES256-GCM-SHA384, ECDHE-RSA-AES256-GCM-SHA384.'\n      - TLS Server Name Indication (SNI) required on all connections.\n      - HTTPS over TCP port 443 to a strict allow list of Apple Pay gateway domains and IP ranges.\n      - The returned session object expires after five minutes.\n    docs: https://developer.apple.com/documentation/applepayontheweb/requesting-an-apple-pay-payment-session\n\
  \    requires_paid_membership: true\n    membership_note: The merchant identity certificate is issued through an Apple Developer Program account.\n  - id: safaridriver-local\n    surface: safaridriver (W3C WebDriver + Safari MCP server)\n    type: none\n    location: local machine\n    description: >-\n      No credential. Access is authorised by the user turning on \"Allow remote automation\n      and external agents\" in Safari's Developer settings on their own machine, and the\n      driver is reachable only from that machine. Automation sessions run in isolated\n      windows that cannot read browsing history, AutoFill data or other sensitive state.\n    docs: https://developer.apple.com/documentation/webkit/about-webdriver-for-safari\n    requires_paid_membership: false\n  - id: aswebauthenticationsession\n    surface: Safari Authentication Services API\n    type: delegated\n    description: >-\n      ASWebAuthenticationSession is the client-side handoff an app uses to run an OAuth\
  \ or\n      WebAuthn flow in Safari and receive the callback. Safari is the user agent in the\n      flow — it is not itself an authorization server, and it issues no tokens of its own.\n      Passkeys/WebAuthn credentials are held by the platform and the relying party is the\n      site, not Apple.\n    docs: https://developer.apple.com/documentation/authenticationservices/aswebauthenticationsession\n    requires_paid_membership: false\nno_credential_required:\n  apis:\n    - Safari Extensions API\n    - Safari App Extensions API\n    - Safari Web Content API (WebKit)\n    - Safari Services API\n    - Safari Content Blocking API\n    - Safari Developer Tools API\n  note: >-\n    In-process platform APIs. Distribution through App Store Connect requires Apple\n    Developer Program membership, but calling the API does not.\ndiscovery_documents:\n  openid_configuration: not served\n  oauth_authorization_server: not served\n  evidence: well-known/apple-safari-well-known.yml\nmaintainers:\n\
  \  - FN: Kin Lane\n    email: kin@apievangelist.com\n    url: https://apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-safari/refs/heads/main/authentication/apple-safari-authentication.yml
summary_line: 4 schemes
tags:
- Apple
- Browser
- Privacy
- Web Browser
- Webkit
---
