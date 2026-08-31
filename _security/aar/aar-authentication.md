---
api_key_in: []
auth_types:
- http-bearer
description: AAR CORP. publishes no developer authentication guide, no OpenAPI securitySchemes, and no OAuth or OIDC discovery document on any host. This profile is therefore built entirely from observed runtime behaviour of the one live, anonymously reachable API surface AAR operates — the AAR PAARTS Store commerce API at shop.aarcorp.com/rest/V1/ — plus the api.aarcorp.com gateway. No credential, key format, token endpoint or scope list is published by AAR, so none is recorded here.
kind: authentication
layout: security
method: probed
name: Aar Authentication
name_suffix: Authentication
oauth_flows: []
overview: AAR Corp secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AAR Corp
provider_slug: aar
scheme_count: 1
schemes:
- evidence:
  - body: '{"message":"The consumer isn''t authorized to access %resources.","parameters":{"resources":"Magento_Catalog::products"}}'
    probe: GET https://shop.aarcorp.com/rest/V1/products
    status: 401
  - body: '{"message":"The consumer isn''t authorized to access %resources.","parameters":{"resources":"Magento_Backend::store"}}'
    probe: GET https://shop.aarcorp.com/rest/V1/store/storeViews
    status: 401
  - note: An invalid bearer token yields the same envelope; the header is read but no token issuance path is published.
    probe: GET https://shop.aarcorp.com/rest/V1/store/storeViews with Authorization Bearer <invalid>
    status: 401
  name: magentoBearerToken
  note: The 401 envelope carries a Magento ACL resource identifier (Magento_Catalog::products, Magento_Backend::store), which is a platform-level permission name, not an AAR-published OAuth scope. No scopes/ artifact is emitted, because AAR publishes no scope reference.
  scheme: bearer
  status: observed
  surface: https://shop.aarcorp.com/rest/V1
  type: http
slug: aar-authentication
source_filename: aar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://shop.aarcorp.com/rest/V1/* and https://api.aarcorp.com/\n  on 2026-08-29. AAR CORP. publishes no developer authentication documentation; everything\n  below is what the running endpoints actually returned.\nprovider: AAR Corp\nproviderId: aar\ndescription: >-\n  AAR CORP. publishes no developer authentication guide, no OpenAPI securitySchemes, and no\n  OAuth or OIDC discovery document on any host. This profile is therefore built entirely\n  from observed runtime behaviour of the one live, anonymously reachable API surface AAR\n  operates — the AAR PAARTS Store commerce API at shop.aarcorp.com/rest/V1/ — plus the\n  api.aarcorp.com gateway. No credential, key format, token endpoint or scope list is\n  published by AAR, so none is recorded here.\nsummary:\n  types:\n    - http-bearer\n  api_key_in: []\n  oauth2_flows: []\n  documented_by_provider: false\n  discovery_documents: none\n  note:\
  \ >-\n    The bearer scheme below is inferred ONLY from the 401 challenge the live endpoint\n    returns; AAR does not document it, and no token endpoint was found. Treat as observed,\n    not as a provider contract.\nschemes:\n  - name: magentoBearerToken\n    type: http\n    scheme: bearer\n    surface: https://shop.aarcorp.com/rest/V1\n    status: observed\n    evidence:\n      - probe: GET https://shop.aarcorp.com/rest/V1/products\n        status: 401\n        body: '{\"message\":\"The consumer isn''t authorized to access %resources.\",\"parameters\":{\"resources\":\"Magento_Catalog::products\"}}'\n      - probe: GET https://shop.aarcorp.com/rest/V1/store/storeViews\n        status: 401\n        body: '{\"message\":\"The consumer isn''t authorized to access %resources.\",\"parameters\":{\"resources\":\"Magento_Backend::store\"}}'\n      - probe: GET https://shop.aarcorp.com/rest/V1/store/storeViews with Authorization Bearer <invalid>\n        status: 401\n        note: An invalid bearer\
  \ token yields the same envelope; the header is read but no token issuance path is published.\n    note: >-\n      The 401 envelope carries a Magento ACL resource identifier (Magento_Catalog::products,\n      Magento_Backend::store), which is a platform-level permission name, not an AAR-published\n      OAuth scope. No scopes/ artifact is emitted, because AAR publishes no scope reference.\nanonymous_surface:\n  note: >-\n    A small set of /rest/V1 routes answer with no credential at all. These are the only\n    AAR API operations any third party can call today.\n  endpoints:\n    - method: GET\n      path: /rest/V1/directory/currency\n      status: 200\n      content_type: application/json; charset=utf-8\n    - method: GET\n      path: /rest/V1/directory/countries\n      status: 200\n      content_type: application/json; charset=utf-8\n    - method: POST\n      path: /rest/V1/guest-carts\n      status: 200\n      note: >-\n        Anonymous WRITE. Returns a guest quote identifier as a\
  \ bare JSON string. Recorded\n        because an unauthenticated write surface is a material fact about the API, not\n        because AAR documents or endorses its use.\ngateway:\n  host: https://api.aarcorp.com\n  status: live\n  observed: >-\n    Every path probed (/, /openapi.json, /swagger.json, /api-docs, /docs, /v1, /api, /health,\n    /graphql, /mcp and all /.well-known/*) returned HTTP 404 with the JSON envelope\n    {\"statusCode\":404,\"message\":\"Resource not found\"}. The host is a real API gateway with no\n    anonymously discoverable route and no published authentication contract.\npartner_portal:\n  host: https://myconnection.aarcorp.com\n  note: >-\n    AAR's partner/customer portal. Anonymous requests complete the TLS handshake and open an\n    HTTP/2 stream, then receive no response within 15s. Not retried. Any customer-facing\n    integration credentials are issued through this portal or through a commercial contract,\n    neither of which is publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aar/refs/heads/main/authentication/aar-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Aviation
- MRO
- Aerospace
- Defense
- Parts Supply
- Maintenance
- Government
- Aviation Software
- Supply Chain
- E-Commerce
- Fortune 1000
---
