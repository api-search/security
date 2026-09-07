---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcbest-pickups-api-openapi.yml
  format: yaml
  label: ArcBest Pickups API
  slug: arcbest-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-pickups-api-openapi.yml
- filename: arcbest-rates-api-openapi.yml
  format: yaml
  label: ArcBest Rates API
  slug: arcbest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-rates-api-openapi.yml
- filename: arcbest-shipments-api-openapi.yml
  format: yaml
  label: ArcBest Shipments API
  slug: arcbest-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-shipments-api-openapi.yml
- filename: arcbest-tracking-api-openapi.yml
  format: yaml
  label: ArcBest Tracking API
  slug: arcbest-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-tracking-api-openapi.yml
- filename: arcbest-expedite-customer-api-openapi.yml
  format: yaml
  label: ArcBest Expedite Customer API
  slug: arcbest-expedite-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-expedite-customer-api-openapi.yml
- filename: arcbest-expedite-tms-api-openapi.yml
  format: yaml
  label: ArcBest Expedite Third Party TMS API
  slug: arcbest-expedite-tms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-expedite-tms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Arcbest Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArcBest secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ArcBest
provider_slug: arcbest
scheme_count: 2
schemes:
- api: arcbest:arcbest-expedite-customer-api
  credential_issuance: ArcBest support (api@arcb.com). Not self-serve.
  description: 'Customer API. POST {"ClientId": "<32 chars>", "ClientSecret": "<64 chars>"} to https://api.arcb.com/expedite/customer/authorize; the response is {"AccessToken": "<~1000 chars>"}. Send that token on every subsequent call as `Authorization: Bearer <accesstoken>`. ArcBest states "The API uses standard bearer authentication".'
  evidence:
  - note: GET returns Method Not Allowed - the endpoint is live and POST-only. Probed 2026-09-04.
    status: 405
    url: https://api.arcb.com/expedite/customer/authorize
  name: bearerAuth
  refresh: not published
  scheme: bearer
  scopes: none published
  sources:
  - docs/arcbest-expedite-customer-quote-book-instructions-2024-08.pdf
  - docs/arcbest-expedite-customer-api-definition.html
  test_token_endpoint: https://test.api.arcb.com/expedite/customer/authorize
  token_endpoint: https://api.arcb.com/expedite/customer/authorize
  token_lifetime: not published
  type: http
- api: arcbest:arcbest-expedite-tms-api
  credential_issuance: ArcBest Expedite team. Not self-serve.
  description: Third Party TMS API. HTTP Basic with a username and password issued by the ArcBest Expedite team. "Request basic authentication username and password from the ArcBest Expedite team."
  evidence:
  - note: Returns a WWW-Authenticate header of `Basic realm="service"`. Probed 2026-09-04.
    status: 401
    url: https://api.arcb.com/expedite/digital/
  - note: Same Basic challenge on the test host. Probed 2026-09-04.
    status: 401
    url: https://test.api.arcb.com/expedite/digital/
  name: basicAuth
  scheme: basic
  sources:
  - docs/arcbest-expedite-tms-quote-book-instructions-2024-08.pdf
  - docs/arcbest-expedite-tms-api-definition.html
  type: http
slug: arcbest-authentication
source_filename: arcbest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  ArcBest's own published Expedite instructions\n  (docs/arcbest-expedite-customer-quote-book-instructions-2024-08.pdf,\n  docs/arcbest-expedite-tms-quote-book-instructions-2024-08.pdf), the ArcBest API access support\n  article (https://support.arcb.com/en/articles/2851223-api-access), and live probes of api.arcb.com\n  on 2026-09-04.\nprovider: ArcBest\nproviderId: arcbest\nsummary:\n  types:\n    - http\n  self_serve: false\n  note: >-\n    ArcBest runs two different authentication schemes on two different Expedite products. Neither is\n    OAuth 2.0 and neither is self-serve - every credential is issued by a human at ArcBest.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    api: arcbest:arcbest-expedite-customer-api\n    description: >-\n      Customer API. POST {\"ClientId\": \"<32 chars>\", \"ClientSecret\": \"<64 chars>\"} to\n      https://api.arcb.com/expedite/customer/authorize; the response\
  \ is\n      {\"AccessToken\": \"<~1000 chars>\"}. Send that token on every subsequent call as\n      `Authorization: Bearer <accesstoken>`. ArcBest states \"The API uses standard bearer\n      authentication\".\n    token_endpoint: https://api.arcb.com/expedite/customer/authorize\n    test_token_endpoint: https://test.api.arcb.com/expedite/customer/authorize\n    credential_issuance: ArcBest support (api@arcb.com). Not self-serve.\n    token_lifetime: not published\n    refresh: not published\n    scopes: none published\n    sources:\n      - docs/arcbest-expedite-customer-quote-book-instructions-2024-08.pdf\n      - docs/arcbest-expedite-customer-api-definition.html\n    evidence:\n      - url: https://api.arcb.com/expedite/customer/authorize\n        status: 405\n        note: GET returns Method Not Allowed - the endpoint is live and POST-only. Probed 2026-09-04.\n  - name: basicAuth\n    type: http\n    scheme: basic\n    api: arcbest:arcbest-expedite-tms-api\n    description: >-\n\
  \      Third Party TMS API. HTTP Basic with a username and password issued by the ArcBest Expedite\n      team. \"Request basic authentication username and password from the ArcBest Expedite team.\"\n    credential_issuance: ArcBest Expedite team. Not self-serve.\n    sources:\n      - docs/arcbest-expedite-tms-quote-book-instructions-2024-08.pdf\n      - docs/arcbest-expedite-tms-api-definition.html\n    evidence:\n      - url: https://api.arcb.com/expedite/digital/\n        status: 401\n        note: 'Returns a WWW-Authenticate header of `Basic realm=\"service\"`. Probed 2026-09-04.'\n      - url: https://test.api.arcb.com/expedite/digital/\n        status: 401\n        note: Same Basic challenge on the test host. Probed 2026-09-04.\naccount_api_id:\n  detail: >-\n    Separately from the Expedite APIs, an existing arcb.com customer has an \"API ID\" visible after\n    signing in - Menu > Resources > APIs at https://arcb.com/api, which 302s to\n    https://arcb.com/login?m=login-required\
  \ for anonymous callers. That surface (rate quote, volume\n    quote, tracking, document retrieval, transit times, pickup request, bill of lading) is documented\n    only behind that login; its authentication scheme is not published anywhere anonymous.\n  evidence:\n    - url: https://arcb.com/api\n      status: 200\n      note: Redirects to https://arcb.com/login?m=login-required. Probed 2026-09-04.\n    - url: https://support.arcb.com/en/articles/2851223-api-access\n      status: 200\noauth:\n  supported: false\n  detail: >-\n    No OAuth 2.0 or OpenID Connect. No /.well-known/oauth-authorization-server or\n    /.well-known/openid-configuration is served on arcb.com, api.arcb.com, test.api.arcb.com or\n    www.arcbest.com - all 404, probed 2026-09-04. See well-known/arcbest-well-known.yml. No scopes\n    artifact is emitted because no scopes exist to record.\nmtls:\n  supported: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/authentication/arcbest-authentication.yml
summary_line: http · 2 schemes
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
- Expedite
- Truckload
- EDI
- Bill of Lading
- Rate Quote
- Shipment Tracking
---
