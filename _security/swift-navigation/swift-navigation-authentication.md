---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Swift Navigation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swift Navigation declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Swift Navigation
provider_slug: swift-navigation
scheme_count: 4
schemes:
- api: Skylark Precise Positioning Service
  credential_issuance:
    requires: account plus either a valid payment method or a promo code (or an unexpired 14-day trial)
    url: https://account.swiftnav.com/
    where: Skylark User Portal, Devices tab, ADD NEW DEVICE
  credential_recovery:
    detail: 'Documented explicitly by the provider, and it is the single most important operational fact on this surface: "For security reasons, passwords are not stored in a recoverable form and are no longer visible after the window is closed." A lost NTRIP password can only be replaced by generating a new one, which rotates the credential on the device.'
    recoverable: false
  description: Skylark correction streams are authenticated with an NTRIP username and password issued per DEVICE, not per account. The username is "<device-suffix>" derived from the account username chosen at sign-up (lowercase letters, digits and hyphens; must start with a letter and end with a letter or digit).
  header: Authorization
  id: skylark_ntrip_basic
  in: header
  revocation:
    detail: Credentials are disabled automatically when a subscription lapses — at the end of an unconverted free trial, shortly after a failed scheduled payment, or at the end of a billing cycle with auto-renew off. Re-enabling a payment method reactivates them.
  scheme: basic
  transport_security:
  - note: Basic credentials travel in the clear on the standard NTRIP port.
    port: 2101
    tls: false
  - port: 2102
    tls: true
  - note: mTLS; requires NTRIP v2.
    port: 2103
    tls: mutual
  type: http
- api: Skylark User Portal / account and subscription services
  code_challenge_methods_supported:
  - S256
  - plain
  description: The Skylark User Portal and its two backend services (account-service.skylark.swiftnav.com, subscription-service.skylark.swiftnav.com) authenticate against an Auth0 tenant, skylark-prod.us.auth0.com, with audience https://account.swiftnav.com. The tenant was identified from the portal's own public runtime configuration at https://account.swiftnav.com/runtime-config.js.
  endpoints:
    authorization: https://skylark-prod.us.auth0.com/authorize
    device_authorization: https://skylark-prod.us.auth0.com/oauth/device/code
    jwks: https://skylark-prod.us.auth0.com/.well-known/jwks.json
    registration: https://skylark-prod.us.auth0.com/oidc/register
    revocation: https://skylark-prod.us.auth0.com/oauth/revoke
    token: https://skylark-prod.us.auth0.com/oauth/token
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: skylark_portal_oidc
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://skylark-prod.us.auth0.com/
  openid_connect_url: https://skylark-prod.us.auth0.com/.well-known/openid-configuration
  scopes_note: These are the stock OIDC/Auth0 identity scopes. NO Skylark-specific API scopes (read:devices, write:subscriptions, or similar) are advertised in the discovery document and none are documented publicly, so an integrator cannot see what a Skylark token is allowed to do before requesting one.
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- api: Sora API (gRPC)
  description: A Sora device client calls the unauthenticated DeviceService.AuthServerInfo RPC, which returns Auth0AuthServerInfo {host, client_id, audience}, then runs an OAuth 2.0 Device Authorization Grant against that Auth0 host. The browser leg of the flow is where a human associates the device with a Sora project.
  flow: device_code
  id: sora_device_flow
  rfc: RFC 8628
  source: grpc/swift-navigation-sora-device-v1beta-service.proto (comment on AuthServerInfo)
  status: Contract-documented but not exercisable — grpc.sora.swiftnav.com presents a placeholder Kubernetes ingress certificate, so the AuthServerInfo bootstrap cannot complete.
  type: oauth2
- api: Swift Navigation web data endpoints
  description: The first-party JSON endpoints under https://www.swiftnav.com/wp-json/ that power the Skylark portal and the compatibility checker (receiver catalog, country availability, support FAQ, footer) are served with NO authentication and no key. Verified by anonymous probe, HTTP 200.
  id: web_data_anonymous
  type: none
slug: swift-navigation-authentication
source_filename: swift-navigation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://support.swiftnav.com/support/solutions/articles/44002519397-ntrip-client-configuration-for-skylark-corrections\n  ; https://support.swiftnav.com/support/solutions/articles/44002287337-skylark-portal-user-guide\n  ; https://skylark-prod.us.auth0.com/.well-known/openid-configuration (probed 200)\n  ; grpc/swift-navigation-sora-device-v1beta-service.proto\nname: Swift Navigation authentication profile\nnote: >-\n  Swift Navigation publishes no OpenAPI, so this profile is assembled from the surfaces that DO\n  document their own auth: the NTRIP client-configuration article, the Skylark Portal user guide,\n  the Skylark Auth0 tenant's OIDC discovery document, and a comment block inside the Sora protobuf\n  contract. There are three distinct schemes and they do not share credentials.\nschemes:\n  - id: skylark_ntrip_basic\n    api: Skylark Precise Positioning Service\n    type: http\n    scheme: basic\n    in: header\n\
  \    header: Authorization\n    description: >-\n      Skylark correction streams are authenticated with an NTRIP username and password issued\n      per DEVICE, not per account. The username is \"<device-suffix>\" derived from the account\n      username chosen at sign-up (lowercase letters, digits and hyphens; must start with a letter\n      and end with a letter or digit).\n    credential_issuance:\n      where: Skylark User Portal, Devices tab, ADD NEW DEVICE\n      url: https://account.swiftnav.com/\n      requires: account plus either a valid payment method or a promo code (or an unexpired 14-day trial)\n    credential_recovery:\n      recoverable: false\n      detail: >-\n        Documented explicitly by the provider, and it is the single most important operational fact\n        on this surface: \"For security reasons, passwords are not stored in a recoverable form and\n        are no longer visible after the window is closed.\" A lost NTRIP password can only be\n        replaced\
  \ by generating a new one, which rotates the credential on the device.\n    revocation:\n      detail: >-\n        Credentials are disabled automatically when a subscription lapses — at the end of an\n        unconverted free trial, shortly after a failed scheduled payment, or at the end of a\n        billing cycle with auto-renew off. Re-enabling a payment method reactivates them.\n    transport_security:\n      - {port: 2101, tls: false, note: Basic credentials travel in the clear on the standard NTRIP port.}\n      - {port: 2102, tls: true}\n      - {port: 2103, tls: mutual, note: mTLS; requires NTRIP v2.}\n  - id: skylark_portal_oidc\n    api: Skylark User Portal / account and subscription services\n    type: openIdConnect\n    openid_connect_url: https://skylark-prod.us.auth0.com/.well-known/openid-configuration\n    description: >-\n      The Skylark User Portal and its two backend services\n      (account-service.skylark.swiftnav.com, subscription-service.skylark.swiftnav.com) authenticate\n\
  \      against an Auth0 tenant, skylark-prod.us.auth0.com, with audience https://account.swiftnav.com.\n      The tenant was identified from the portal's own public runtime configuration at\n      https://account.swiftnav.com/runtime-config.js.\n    issuer: https://skylark-prod.us.auth0.com/\n    endpoints:\n      authorization: https://skylark-prod.us.auth0.com/authorize\n      token: https://skylark-prod.us.auth0.com/oauth/token\n      device_authorization: https://skylark-prod.us.auth0.com/oauth/device/code\n      jwks: https://skylark-prod.us.auth0.com/.well-known/jwks.json\n      revocation: https://skylark-prod.us.auth0.com/oauth/revoke\n      registration: https://skylark-prod.us.auth0.com/oidc/register\n    scopes_supported: [openid, profile, offline_access, name, given_name, family_name, nickname, email, email_verified, picture, created_at, identities, phone, address]\n    scopes_note: >-\n      These are the stock OIDC/Auth0 identity scopes. NO Skylark-specific API scopes\n \
  \     (read:devices, write:subscriptions, or similar) are advertised in the discovery document and\n      none are documented publicly, so an integrator cannot see what a Skylark token is allowed to do\n      before requesting one.\n    grant_types_supported: [client_credentials, authorization_code, refresh_token, password, implicit, 'urn:ietf:params:oauth:grant-type:device_code', 'urn:ietf:params:oauth:grant-type:token-exchange', 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    code_challenge_methods_supported: [S256, plain]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n    id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  - id: sora_device_flow\n    api: Sora API (gRPC)\n    type: oauth2\n    flow: device_code\n    rfc: RFC 8628\n    description: >-\n      A Sora device client calls the unauthenticated DeviceService.AuthServerInfo RPC, which returns\n      Auth0AuthServerInfo {host, client_id, audience},\
  \ then runs an OAuth 2.0 Device Authorization\n      Grant against that Auth0 host. The browser leg of the flow is where a human associates the\n      device with a Sora project.\n    source: grpc/swift-navigation-sora-device-v1beta-service.proto (comment on AuthServerInfo)\n    status: >-\n      Contract-documented but not exercisable — grpc.sora.swiftnav.com presents a placeholder\n      Kubernetes ingress certificate, so the AuthServerInfo bootstrap cannot complete.\n  - id: web_data_anonymous\n    api: Swift Navigation web data endpoints\n    type: none\n    description: >-\n      The first-party JSON endpoints under https://www.swiftnav.com/wp-json/ that power the Skylark\n      portal and the compatibility checker (receiver catalog, country availability, support FAQ,\n      footer) are served with NO authentication and no key. Verified by anonymous probe, HTTP 200.\ngaps:\n  - >-\n    No API-key mechanism, no machine-to-machine credential and no documented service account for the\n\
  \    Skylark account or subscription services. Everything an integrator can automate today is either\n    the anonymous sourcetable/web-data reads or an NTRIP stream keyed to a single device.\n  - >-\n    No published scope reference. The Auth0 discovery document advertises only identity scopes, and\n    Swift Navigation documents no authorization model for its backend services.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift-navigation/refs/heads/main/authentication/swift-navigation-authentication.yml
summary_line: 4 schemes
tags:
- Company
- GNSS
- Precise Positioning
- Location
- Corrections
- RTK
- NTRIP
- RTCM
- Automotive
- Geospatial
- IoT
- Robotics
- Protocols
---
