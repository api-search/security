---
anonymous_access: false
api_key_in: []
api_specs:
- filename: greenbrier-cos-catalog-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Catalog API
  slug: greenbrier-cos-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-catalog-api-openapi.yml
- filename: greenbrier-cos-discovery-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Discovery API
  slug: greenbrier-cos-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-discovery-api-openapi.yml
- filename: greenbrier-cos-export-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Export API
  slug: greenbrier-cos-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-export-api-openapi.yml
- filename: greenbrier-cos-gauge-tables-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Gauge Tables API
  slug: greenbrier-cos-gauge-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-gauge-tables-api-openapi.yml
- filename: greenbrier-cos-pages-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Pages API
  slug: greenbrier-cos-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-pages-api-openapi.yml
- filename: greenbrier-cos-posts-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Posts API
  slug: greenbrier-cos-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-posts-api-openapi.yml
- filename: greenbrier-cos-products-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Products API
  slug: greenbrier-cos-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-products-api-openapi.yml
- filename: greenbrier-cos-railcars-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Railcars API
  slug: greenbrier-cos-railcars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-railcars-api-openapi.yml
- filename: greenbrier-cos-reporting-marks-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Reporting Marks API
  slug: greenbrier-cos-reporting-marks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-reporting-marks-api-openapi.yml
- filename: greenbrier-cos-search-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Search API
  slug: greenbrier-cos-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-search-api-openapi.yml
- filename: greenbrier-cos-taxonomies-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Taxonomies API
  slug: greenbrier-cos-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-taxonomies-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Greenbrier Cos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greenbrier Companies declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Greenbrier Companies
provider_slug: greenbrier-cos
scheme_count: 0
schemes: []
slug: greenbrier-cos-authentication
source_filename: greenbrier-cos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  Live anonymous HTTPS requests against every Greenbrier API surface on 2026-09-12, plus the OIDC\n  discovery document at https://shop.gbrx.com/.well-known/openid-configuration\nnote: >-\n  Greenbrier publishes no API authentication documentation because it publishes no developer\n  program. This profile was established by probing: every catalogued API answered a full, correct\n  response to an unauthenticated request, and every gated Greenbrier surface answered 401 or a login\n  form. Nothing here is inferred from prose.\nsummary:\n  public_apis_require_credentials: false\n  api_keys_issued: false\n  oauth_for_apis: false\n  signup_required: false\n  rate_limit_on_anonymous_access: not_observed\napis:\n  - api: Greenbrier Tank Car Gauge Table API\n    host: tankcar.gbrx.com\n    schemes: []\n    model: none\n    evidence: >-\n      GET https://tankcar.gbrx.com/api/car/marks returned 200 application/json with 144 records\
  \ and\n      no Authorization header, no cookie and no key. Same for the gauge-table, gauge-tables,\n      valid-car-number-list and /export/ routes.\n    write_surface: none\n  - api: Greenbrier Railcar Catalog API\n    host: www.gbrx.com\n    schemes:\n      - type: none\n        applies_to: read (GET)\n      - type: http\n        scheme: basic\n        applies_to: write (POST/PUT/PATCH/DELETE)\n        note: >-\n          WordPress application passwords. Not part of the public surface, not documented by\n          Greenbrier, and not exercised by this profile.\n    model: anonymous-read\n    evidence: >-\n      GET https://www.gbrx.com/wp-json/wp/v2/railcars?per_page=1 returned 200 with X-WP-Total 85 and\n      no credentials. The route index lists POST/PUT/PATCH/DELETE on the same routes; those require\n      WordPress authentication.\n    write_surface: credentialed-only\n  - api: Greenbrier Aftermarket Parts Store API\n    host: www.gbrx.com\n    schemes:\n      - type: none\n  \
  \      applies_to: product/category/attribute reads\n      - type: cookie\n        name: Nonce / cart token\n        applies_to: cart and checkout routes\n        note: >-\n          The /wc/store/v1/cart and /wc/store/v1/checkout routes are session-scoped and require a\n          WooCommerce Store API nonce. Those routes are deliberately excluded from the catalogued\n          contract.\n    model: anonymous-read\n    evidence: >-\n      GET https://www.gbrx.com/wp-json/wc/store/v1/products?per_page=1 returned 200 with X-WP-Total\n      207 and no credentials.\n    write_surface: session-scoped\n  - api: Greenbrier Press Room API\n    host: www.gbrx.com\n    schemes:\n      - type: none\n        applies_to: read (GET)\n    model: anonymous-read\n    evidence: GET /wp-json/wp/v2/posts?per_page=1 returned 200 with X-WP-Total 245 and no credentials.\n    write_surface: credentialed-only\n  - api: Greenbrier Site Content and Discovery API\n    host: www.gbrx.com\n    schemes:\n      - type:\
  \ none\n        applies_to: read (GET)\n    model: anonymous-read\n    evidence: GET /wp-json/wp/v2/pages?per_page=1 returned 200 with X-WP-Total 51 and no credentials.\n    write_surface: credentialed-only\ngated_surfaces:\n  - host: shop.gbrx.com\n    product: Greenbrier Aftermarket Parts store (Salesforce Experience Cloud)\n    model: oauth2 / openid-connect\n    discovery: https://shop.gbrx.com/.well-known/openid-configuration\n    issuer: https://shop.gbrx.com\n    authorization_endpoint: https://shop.gbrx.com/services/oauth2/authorize\n    token_endpoint: https://shop.gbrx.com/services/oauth2/token\n    jwks_uri: https://shop.gbrx.com/id/keys\n    grant_types: [authorization_code, refresh_token]\n    pkce: S256\n    evidence: >-\n      The discovery document is served anonymously (200). Every data route under it answered 401\n      INVALID_SESSION_ID. The scopes advertised are Salesforce's standard platform scope list, not a\n      Greenbrier-authored scope vocabulary, so no scopes/\
  \ artifact is emitted.\n    note: >-\n      Salesforce Experience Cloud running on a Greenbrier-controlled host. Greenbrier does not\n      document or issue API credentials against it; it backs a human parts-ordering storefront.\n  - host: enspire.gbrx.com\n    product: GMS Partners / Enspire railcar management software\n    model: form-login\n    evidence: >-\n      https://enspire.gbrx.com/ serves an ASP.NET MVC login form. Every /.well-known/* path answers\n      200 with the same login shell. No API surface is reachable anonymously.\n  - host: grsecomm.gbrx.com\n    product: GRS Wheelsets ordering portal\n    model: form-login\n    evidence: https://grsecomm.gbrx.com/ serves an ASP.NET login form; /.well-known/* paths 404.\n  - host: proveedores.gbrx.com\n    product: Greenbrier GIMSA supplier application (Monclova, Mexico)\n    model: form-login\n    evidence: https://proveedores.gbrx.com/ serves a login form; /.well-known/* paths 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/authentication/greenbrier-cos-authentication.yml
summary_line: 0 schemes
tags:
- Rail
- Railcars
- Freight
- Transportation
- Manufacturing
- Leasing
- Logistics
- Tank Cars
- Gauge Tables
- Aftermarket Parts
- Content
- Commerce
---
