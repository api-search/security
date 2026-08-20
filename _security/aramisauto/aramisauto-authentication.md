---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Aramisauto Authentication
name_suffix: Authentication
oauth_flows: []
overview: AramisAuto declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AramisAuto
provider_slug: aramisauto
scheme_count: 1
schemes:
- confidence: high
  credentials:
    note: No signup, key-issuance or partner-onboarding endpoint is published. The only route into the Aramisauto commercial surface is the marketplace partner relationship, whose configuration contracts are published at schemas.aramis.group but whose onboarding is a business conversation.
    obtained_via: not published
    self_serve: false
  evidence:
    body: <?xml version="1.0" encoding="utf-8"?><Errors><Error><Message>Missing WSSE Username.</Message></Error></Errors>
    content_type: application/xml; charset=utf-8
    fetched: '2026-08-17'
    http_status: 403
    url: https://api.aramisauto.com/
  header: X-WSSE
  id: wsse-usernametoken
  in: header
  method: probed
  note: '"Missing WSSE Username" is the canonical error emitted by WSSE UsernameToken authenticators in the PHP/Symfony ecosystem — consistent with the `x-powered-by: PHP/5.6.40` and `x-aramisauto-application: api` headers the same host returns. The exact header name and digest construction are NOT published by Aramisauto; `X-WSSE` is the conventional carrier for this profile and is recorded as the probable header, not as a documented fact.'
  scheme_name: WSSE
  standard: OASIS WS-Security 1.1 UsernameToken Profile
  transport: https
  type: custom
slug: aramisauto-authentication
source_filename: aramisauto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://api.aramisauto.com/\nnote: >-\n  Aramisauto publishes NO authentication documentation — there is no developer\n  portal, no auth guide and no securityScheme anywhere, because there is no\n  published API specification (see x-coverage in apis.yml). Everything below was\n  read off the wire: api.aramisauto.com answers every request with HTTP 403 and\n  an XML body demanding a WSSE username, which identifies the scheme as OASIS\n  WS-Security UsernameToken. This is an observation, not a provider claim, and it\n  is recorded that way. No credential-issuing route is published anywhere on the\n  Aramisauto or Aramis Group surface.\n\napi_host: https://api.aramisauto.com\ndocumented_by_provider: false\n\nschemes:\n- id: wsse-usernametoken\n  type: custom\n  standard: OASIS WS-Security 1.1 UsernameToken Profile\n  in: header\n  header: X-WSSE\n  scheme_name: WSSE\n  transport: https\n  method: probed\n  confidence: high\n  evidence:\n\
  \    url: https://api.aramisauto.com/\n    http_status: 403\n    content_type: application/xml; charset=utf-8\n    body: <?xml version=\"1.0\" encoding=\"utf-8\"?><Errors><Error><Message>Missing WSSE\n      Username.</Message></Error></Errors>\n    fetched: '2026-08-17'\n  note: >-\n    \"Missing WSSE Username\" is the canonical error emitted by WSSE UsernameToken\n    authenticators in the PHP/Symfony ecosystem — consistent with the\n    `x-powered-by: PHP/5.6.40` and `x-aramisauto-application: api` headers the\n    same host returns. The exact header name and digest construction are NOT\n    published by Aramisauto; `X-WSSE` is the conventional carrier for this\n    profile and is recorded as the probable header, not as a documented fact.\n  credentials:\n    obtained_via: not published\n    self_serve: false\n    note: >-\n      No signup, key-issuance or partner-onboarding endpoint is published. The\n      only route into the Aramisauto commercial surface is the marketplace\n     \
  \ partner relationship, whose configuration contracts are published at\n      schemas.aramis.group but whose onboarding is a business conversation.\n\noauth2: false\nopenid_connect: false\napi_keys_documented: false\nmutual_tls: false\nmtls_note: Not observed; the host completes a standard TLS 1.3 handshake without requesting\n  a client certificate.\n\nscopes:\n  published: false\n  note: >-\n    No OAuth surface, so no scope model. scopes/ is deliberately not written —\n    forcing an empty OAuthScopes artifact on a WSSE key-auth provider would be\n    fabrication.\n\nprobes:\n- url: https://api.aramisauto.com/\n  status: 403\n  result: WSSE challenge\n- url: https://api.aramisauto.com/nonsense-control-path-xyz\n  status: 403\n  result: >-\n    IDENTICAL WSSE challenge for a path that cannot exist. The gate sits in front\n    of routing, so no individual path can be confirmed or denied from anonymous\n    probing. Recorded as opaque, not as evidence of any specific endpoint.\n- url:\
  \ https://api.aramisauto.com/.well-known/oauth-authorization-server\n  status: 403\n  result: no authorization-server metadata reachable\n- url: https://www.aramisauto.com/.well-known/openid-configuration\n  status: 301\n  result: empty body, no OIDC discovery document\n\npointer_emitted: false\npointer_reason: >-\n  No `Authentication` pointer is wired into apis.yml. The scoring check it feeds\n  is `authentication_documented`, and Aramisauto documents nothing — this file is\n  OUR probe record of an undocumented gate, so pointing at it would credit the\n  provider with an auth reference it has never published. The finding is\n  preserved here and summarised in conventions/aramisauto-conventions.yml so a\n  later round can upgrade to method: searched if Aramisauto ever publishes a\n  partner auth guide.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aramisauto/refs/heads/main/authentication/aramisauto-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer
- Automotive
- E-Commerce
- Used Cars
- Vehicle Data
- Marketplace
- Retail
- Auto Finance
- France
- JSON-Schema
---
