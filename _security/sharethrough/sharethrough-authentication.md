---
api_key_in: []
auth_types: []
description: 'Authentication profile for the two Sharethrough API surfaces. The Publisher Reporting API is an OAuth 2.0 bearer-token API: every request carries an Authorization: Bearer header and an anonymous request is rejected with a 401. Tokens are issued out of the company''s own Auth0 tenant, whose OpenID Provider Metadata is public. The header-bidding endpoint is unauthenticated and identified by a supply_id query parameter plus a per-publisher placement key.'
kind: authentication
layout: security
method: probed
name: Sharethrough Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sharethrough declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Sharethrough
provider_slug: sharethrough
scheme_count: 2
schemes:
- api: Sharethrough Publisher Reporting API
  evidence:
  - POST https://publisher-api.sharethrough.com/v2/programmatic with no Authorization header returns HTTP 401 {"message":"Unauthorized","statusCode":401}
  - POST with an invalid bearer token returns the identical 401 body — no distinct invalid_token/expired_token signal is exposed to the caller
  - libs/auth.py in Sharethrough's own publisher-api-examples repo implements a requests.auth.AuthBase that sets r.headers["authorization"] = "Bearer " + token
  - setup.py in the same repo defines AUTH_TOKEN as the single credential the client needs
  format: 'Authorization: Bearer <AUTH_TOKEN>'
  header: Authorization
  id: publisher_api_bearer
  in: header
  required: true
  rotation: unknown
  scheme: bearer
  scopes: none documented
  token_acquisition: Not publicly documented. The token is issued to a publisher account; the support article that described how to obtain it (360044449471) now returns 404 to anonymous callers.
  type: http
- api: Sharethrough Header Bidding (Prebid) API
  evidence:
  - STR_ENDPOINT in modules/sharethroughBidAdapter.js (Prebid.js, adapter VERSION 4.3.0) is https://btlr.sharethrough.com/universal/v1?supply_id=WYu2BXv1
  - An anonymous POST of a malformed OpenRTB body to that URL returns HTTP 400 with an empty body — the endpoint accepts unauthenticated requests and validates the payload
  format: https://btlr.sharethrough.com/universal/v1?supply_id=<supply_id>
  id: bidding_supply_id
  in: query
  note: This is bid-request identification, not authentication. Per-publisher authorization is carried by the required params.pkey placement key inside the bid request, which Sharethrough issues after the Integrations team approves the publisher.
  parameter: supply_id
  required: true
  type: none
  value_observed: WYu2BXv1
slug: sharethrough-authentication
source_filename: sharethrough-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Sharethrough Authentication\ndescription: >-\n  Authentication profile for the two Sharethrough API surfaces. The Publisher Reporting API\n  is an OAuth 2.0 bearer-token API: every request carries an Authorization: Bearer header and\n  an anonymous request is rejected with a 401. Tokens are issued out of the company's own\n  Auth0 tenant, whose OpenID Provider Metadata is public. The header-bidding endpoint is\n  unauthenticated and identified by a supply_id query parameter plus a per-publisher\n  placement key.\ngenerated: '2026-08-12'\nmethod: probed\nsource: >-\n  live probes of https://publisher-api.sharethrough.com/v2/programmatic and\n  https://sharethrough-users.auth0.com/.well-known/openid-configuration, plus Sharethrough's\n  own first-party example client at https://github.com/strchives/publisher-api-examples\ndocs: https://support.sharethrough.com/hc/en-us/sections/360009157451-Publisher-API-for-Reporting\ndocs_status: >-\n  401 anonymously — the Publisher\
  \ API for Reporting section of the support site now requires\n  a signed-in Zendesk user, so the written auth reference is not publicly readable.\nschemes:\n  - id: publisher_api_bearer\n    api: Sharethrough Publisher Reporting API\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <AUTH_TOKEN>'\n    required: true\n    evidence:\n      - >-\n        POST https://publisher-api.sharethrough.com/v2/programmatic with no Authorization\n        header returns HTTP 401 {\"message\":\"Unauthorized\",\"statusCode\":401}\n      - >-\n        POST with an invalid bearer token returns the identical 401 body — no distinct\n        invalid_token/expired_token signal is exposed to the caller\n      - >-\n        libs/auth.py in Sharethrough's own publisher-api-examples repo implements a\n        requests.auth.AuthBase that sets r.headers[\"authorization\"] = \"Bearer \" + token\n      - >-\n        setup.py in the same repo defines AUTH_TOKEN\
  \ as the single credential the client needs\n    token_acquisition: >-\n      Not publicly documented. The token is issued to a publisher account; the support article\n      that described how to obtain it (360044449471) now returns 404 to anonymous callers.\n    rotation: unknown\n    scopes: none documented\n  - id: bidding_supply_id\n    api: Sharethrough Header Bidding (Prebid) API\n    type: none\n    in: query\n    parameter: supply_id\n    required: true\n    value_observed: WYu2BXv1\n    format: 'https://btlr.sharethrough.com/universal/v1?supply_id=<supply_id>'\n    evidence:\n      - >-\n        STR_ENDPOINT in modules/sharethroughBidAdapter.js (Prebid.js, adapter VERSION 4.3.0)\n        is https://btlr.sharethrough.com/universal/v1?supply_id=WYu2BXv1\n      - >-\n        An anonymous POST of a malformed OpenRTB body to that URL returns HTTP 400 with an\n        empty body — the endpoint accepts unauthenticated requests and validates the payload\n    note: >-\n      This is bid-request\
  \ identification, not authentication. Per-publisher authorization is\n      carried by the required params.pkey placement key inside the bid request, which\n      Sharethrough issues after the Integrations team approves the publisher.\nidentity_provider:\n  vendor: Auth0\n  tenant: sharethrough-users.auth0.com\n  issuer: https://sharethrough-users.auth0.com/\n  discovery: well-known/sharethrough-openid-configuration.json\n  discovered_via: 'http://nag.sharethrough.com 302 -> https://sharethrough-users.auth0.com/u/login'\n  authorization_endpoint: https://sharethrough-users.auth0.com/authorize\n  token_endpoint: https://sharethrough-users.auth0.com/oauth/token\n  revocation_endpoint: https://sharethrough-users.auth0.com/oauth/revoke\n  jwks_uri: https://sharethrough-users.auth0.com/.well-known/jwks.json\n  device_authorization_endpoint: https://sharethrough-users.auth0.com/oauth/device/code\n  id_token_signing: RS256\n  pkce: 'S256 and plain both advertised'\n  grant_types_supported:\n\
  \    - client_credentials\n    - authorization_code\n    - refresh_token\n    - password\n    - implicit\n    - 'urn:ietf:params:oauth:grant-type:device_code'\n    - 'urn:ietf:params:oauth:grant-type:token-exchange'\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    - private_key_jwt\n    - none\n  scopes_supported:\n    - openid\n    - profile\n    - offline_access\n    - name\n    - given_name\n    - family_name\n    - nickname\n    - email\n    - email_verified\n    - picture\n    - created_at\n    - identities\n    - phone\n    - address\n  scopes_note: >-\n    These are the stock OpenID Connect / Auth0 profile scopes the tenant advertises. They are\n    NOT an authorization model for the Publisher Reporting API — Sharethrough documents no\n    API scopes or permissions anywhere public, which is why no scopes/ artifact and no\n    OAuthScopes pointer are emitted for this provider.\n\
  \  caveats:\n    - >-\n      The tenant advertises the legacy implicit and resource-owner-password grants alongside\n      authorization_code + PKCE. Both are discouraged by OAuth 2.1 / BCP 240.\ntransport:\n  tls_required: true\n  observed_tls: TLSv1.3\n  hsts_on_bidding_host: 'max-age=16000000; includeSubDomains; preload'\n  hsts_on_reporting_host: not sent on the /v2 JSON responses observed\n  cors: 'access-control-allow-origin: * on every publisher-api.sharethrough.com response observed'\nmtls: none\napi_keys: none\nbasic_auth: none\nnotes:\n  - >-\n    There is no published OpenAPI for either surface, so this profile is built from live\n    probes and from Sharethrough's own example client rather than derived from securitySchemes.\n  - >-\n    A caller cannot distinguish \"no token\", \"bad token\" and \"expired token\": all three\n    produce the same opaque 401 body with no WWW-Authenticate header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharethrough/refs/heads/main/authentication/sharethrough-authentication.yml
summary_line: 2 schemes
tags:
- Native Advertising
- Programmatic Advertising
- SSP
- DSP
- OpenRTB
- Ad Exchange
- Header Bidding
- CTV
- Sustainability
---
