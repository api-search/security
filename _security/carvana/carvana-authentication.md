---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Carvana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carvana declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Carvana
provider_slug: carvana
scheme_count: 4
schemes:
- api: carvana:partner-api
  description: An account on the Carvana developer portal is the first gate. The portal states the API "requires authorization by Carvana LLC" — sign-up alone does not grant access; Carvana must approve the partner.
  evidence:
  - note: Azure API Management developer-portal sign-in page
    status: 200
    url: https://api-developer.carvana.com/signin
  - note: Azure API Management developer-portal sign-up page
    status: 200
    url: https://api-developer.carvana.com/signup
  - note: The portal's own management proxy answers anonymously with {"value":[],"nextLink":null}. Zero APIs and zero products are visible without an account, which is the concrete proof that the whole Partner API catalog is authorization-gated rather than merely undocumented.
    status: 200
    url: https://api-developer.carvana.com/developer/apis?api-version=2022-04-01-preview
  host: api-developer.carvana.com
  id: apim-portal-account
  observed: true
  type: portal-account
- api: carvana:partner-api
  basis: azure-apim-platform-default
  description: NOT OBSERVED on a live Carvana gateway response. Azure API Management issues a per-product subscription key sent as Ocp-Apim-Subscription-Key (or ?subscription-key=), and Carvana's portal is a stock Azure APIM portal, so this is the expected credential — but no anonymous request has ever been answered by a Carvana APIM gateway, so it is recorded as a platform default and not as a documented Carvana fact. Confirm at partner onboarding.
  evidence:
  - note: Page identifies itself as "Microsoft Azure API Management - developer portal" and links /products, the Azure APIM subscription surface.
    status: 200
    url: https://api-developer.carvana.com/
  id: apim-subscription-key
  in: header
  name: Ocp-Apim-Subscription-Key
  observed: false
  type: apiKey
- api: carvana:collective-api
  description: HTTP Basic authentication guards the entire Collective host, documentation included. This is a shared-credential scheme with no scopes, no token endpoint and no rotation surface exposed to the client.
  evidence:
  - header: 'WWW-Authenticate: Basic realm="Collective API Reference", charset="UTF-8"'
    note: 'Every path on this host — including invented ones — answers 401 with this header. The realm name is itself the finding: a document titled "Collective API Reference" exists behind HTTP Basic auth. The reference is published, it is simply not public.'
    status: 401
    url: https://api.collective.carvana.com/
  host: api.collective.carvana.com
  id: collective-http-basic
  observed: true
  realm: Collective API Reference
  scheme: basic
  type: http
- description: Recorded for completeness. No credential is requested and no route is reachable anonymously.
  evidence:
  - body: '{"statusCode":404,"message":"Resource not found"}'
    note: A live JSON gateway not declared in apis.yml. It answers every path with the same 404 and never challenges for a credential, so no authentication scheme can be attributed to it.
    status: 404
    url: https://api.carvana.com/v1/vehicles
  host: api.carvana.com
  id: gateway-unauthenticated-404
  observed: true
  type: none
slug: carvana-authentication
source_filename: carvana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live HTTP probes of api-developer.carvana.com, api.collective.carvana.com and api.carvana.com,\n  2026-09-05. No OpenAPI securitySchemes exist to derive from — Carvana publishes no machine-readable\n  contract — so every entry below is either an OBSERVED response header or is explicitly marked as a\n  platform default that was not observed.\nnote: >-\n  Carvana operates two authenticated API surfaces and one bare gateway. Neither surface publishes an\n  OAuth or OpenID discovery document; /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server 404 (or 401) on every host. There is no public scope\n  reference, so scopes/ is deliberately not written.\nschemes:\n  - id: apim-portal-account\n    api: carvana:partner-api\n    host: api-developer.carvana.com\n    type: portal-account\n    observed: true\n    evidence:\n      - url: https://api-developer.carvana.com/signin\n        status: 200\n      \
  \  note: Azure API Management developer-portal sign-in page\n      - url: https://api-developer.carvana.com/signup\n        status: 200\n        note: Azure API Management developer-portal sign-up page\n      - url: https://api-developer.carvana.com/developer/apis?api-version=2022-04-01-preview\n        status: 200\n        note: >-\n          The portal's own management proxy answers anonymously with {\"value\":[],\"nextLink\":null}.\n          Zero APIs and zero products are visible without an account, which is the concrete proof\n          that the whole Partner API catalog is authorization-gated rather than merely undocumented.\n    description: >-\n      An account on the Carvana developer portal is the first gate. The portal states the API\n      \"requires authorization by Carvana LLC\" — sign-up alone does not grant access; Carvana must\n      approve the partner.\n  - id: apim-subscription-key\n    api: carvana:partner-api\n    type: apiKey\n    in: header\n    name: Ocp-Apim-Subscription-Key\n\
  \    observed: false\n    basis: azure-apim-platform-default\n    evidence:\n      - url: https://api-developer.carvana.com/\n        status: 200\n        note: >-\n          Page identifies itself as \"Microsoft Azure API Management - developer portal\" and links\n          /products, the Azure APIM subscription surface.\n    description: >-\n      NOT OBSERVED on a live Carvana gateway response. Azure API Management issues a per-product\n      subscription key sent as Ocp-Apim-Subscription-Key (or ?subscription-key=), and Carvana's\n      portal is a stock Azure APIM portal, so this is the expected credential — but no anonymous\n      request has ever been answered by a Carvana APIM gateway, so it is recorded as a platform\n      default and not as a documented Carvana fact. Confirm at partner onboarding.\n  - id: collective-http-basic\n    api: carvana:collective-api\n    host: api.collective.carvana.com\n    type: http\n    scheme: basic\n    observed: true\n    realm: Collective API\
  \ Reference\n    evidence:\n      - url: https://api.collective.carvana.com/\n        status: 401\n        header: 'WWW-Authenticate: Basic realm=\"Collective API Reference\", charset=\"UTF-8\"'\n        note: >-\n          Every path on this host — including invented ones — answers 401 with this header. The realm\n          name is itself the finding: a document titled \"Collective API Reference\" exists behind HTTP\n          Basic auth. The reference is published, it is simply not public.\n    description: >-\n      HTTP Basic authentication guards the entire Collective host, documentation included. This is a\n      shared-credential scheme with no scopes, no token endpoint and no rotation surface exposed to\n      the client.\n  - id: gateway-unauthenticated-404\n    host: api.carvana.com\n    type: none\n    observed: true\n    evidence:\n      - url: https://api.carvana.com/v1/vehicles\n        status: 404\n        body: '{\"statusCode\":404,\"message\":\"Resource not found\"}'\n\
  \        note: >-\n          A live JSON gateway not declared in apis.yml. It answers every path with the same 404 and\n          never challenges for a credential, so no authentication scheme can be attributed to it.\n    description: >-\n      Recorded for completeness. No credential is requested and no route is reachable anonymously.\nabsent:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  - published_scope_reference\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carvana/refs/heads/main/authentication/carvana-authentication.yml
summary_line: 4 schemes
tags:
- Automotive
- E-Commerce
- Used Cars
- Inventory
- Partner API
- Fortune 500
---
