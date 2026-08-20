---
api_key_in: []
api_specs:
- filename: cj-affiliate.postman_collection.json
  format: json
  label: CJ Commission Detail API
  slug: cj-affiliate-commission-detail-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/collections/cj-affiliate.postman_collection.json
- filename: cj-affiliate-ads-asyncapi.yml
  format: yaml
  label: CJ Product Search API
  slug: cj-affiliate-product-search-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/asyncapi/cj-affiliate-ads-asyncapi.yml
- filename: cj-affiliate-advertiser-lookup-api-openapi.yml
  format: yaml
  label: CJ Affiliate Advertiser Lookup API
  slug: cj-affiliate-advertiser-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-advertiser-lookup-api-openapi.yml
- filename: cj-affiliate-link-search-api-openapi.yml
  format: yaml
  label: CJ Affiliate Link Search API
  slug: cj-affiliate-link-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-link-search-api-openapi.yml
- filename: cj-affiliate-publisher-lookup-api-openapi.yml
  format: yaml
  label: CJ Affiliate Publisher Lookup API
  slug: cj-affiliate-publisher-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-publisher-lookup-api-openapi.yml
- filename: cj-affiliate-click-events-api-openapi.yml
  format: yaml
  label: CJ Affiliate Click Events API
  slug: cj-affiliate-click-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-click-events-api-openapi.yml
- filename: cj-affiliate-publisher-tracking-api-openapi.yml
  format: yaml
  label: CJ Affiliate Publisher Tracking API
  slug: cj-affiliate-publisher-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-publisher-tracking-api-openapi.yml
- filename: cj-affiliate-commission-detail-legacy-api-openapi.yml
  format: yaml
  label: CJ Affiliate Commission Detail API (Legacy)
  slug: cj-affiliate-commission-detail-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-commission-detail-legacy-api-openapi.yml
auth_types:
- http
description: 'One credential covers CJ''s entire platform: a long-lived Personal Access Token sent as an HTTP Bearer credential. The same token authenticates all three GraphQL endpoints, all the classic REST APIs and both click-tracking APIs. There is no OAuth 2.0, no OpenID Connect, no scopes, no refresh and no token endpoint a client may call — /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404 on every CJ host including iam.cj.com, the internal PAT service the developer portal itself calls.'
kind: authentication
layout: security
method: searched
name: Cj Affiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: CJ Affiliate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CJ Affiliate
provider_slug: cj-affiliate
scheme_count: 1
schemes:
- description: 'A Personal Access Token created by a signed-in user in the CJ developer portal. CJ''s REST APIs also still accept the older Developer Key in the same Authorization header, and the documented 401 messages reference it by name ("You must specify a developer key.", "Not Authenticated: <key>").'
  expiry: not published
  format: Bearer <personal-access-token>
  header: Authorization
  issuance: manual
  issuance_url: https://developers.cj.com/account/personal-access-tokens
  name: personalAccessToken
  refresh: false
  scheme: bearer
  scopes: []
  sources:
  - https://production-docs-assets.p.cjpowered.com/REST%20APIs/Overview.md
  - openapi/_original/cj-affiliate-openapi.yml
  - graphql/cj-affiliate-graphql.md
  type: http
slug: cj-affiliate-authentication
source_filename: cj-affiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://production-docs-assets.p.cjpowered.com/REST%20APIs/Overview.md and the\n  per-API pages it indexes, plus live 401 probes of every CJ API host and the\n  developer-portal bundle at https://developers.cj.com/static/js/main.*.chunk.js\ndocs:\n- https://developers.cj.com/authentication/overview\n- https://developers.cj.com/account/personal-access-tokens\nprovider: CJ Affiliate\nproviderId: cj-affiliate\nsummary:\n  types:\n  - http\n  oauth2: false\n  oidc: false\n  mtls: false\n  scopes: false\ndescription: >-\n  One credential covers CJ's entire platform: a long-lived Personal Access Token\n  sent as an HTTP Bearer credential. The same token authenticates all three\n  GraphQL endpoints, all the classic REST APIs and both click-tracking APIs.\n  There is no OAuth 2.0, no OpenID Connect, no scopes, no refresh and no token\n  endpoint a client may call — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server\
  \ return 404 on every CJ host including\n  iam.cj.com, the internal PAT service the developer portal itself calls.\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <personal-access-token>'\n  issuance: manual\n  issuance_url: https://developers.cj.com/account/personal-access-tokens\n  expiry: not published\n  refresh: false\n  scopes: []\n  description: >-\n    A Personal Access Token created by a signed-in user in the CJ developer\n    portal. CJ's REST APIs also still accept the older Developer Key in the same\n    Authorization header, and the documented 401 messages reference it by name\n    (\"You must specify a developer key.\", \"Not Authenticated: <key>\").\n  sources:\n  - https://production-docs-assets.p.cjpowered.com/REST%20APIs/Overview.md\n  - openapi/_original/cj-affiliate-openapi.yml\n  - graphql/cj-affiliate-graphql.md\nauthorization_model:\n  mechanism: account membership + explicit account parameter\n \
  \ description: >-\n    Authentication and authorization are separated. The token establishes WHO\n    the caller is; a company identifier on every request establishes WHICH\n    account the call is against, and CJ authorizes it only if the token's user is\n    a member of that company.\n  parameters:\n  - name: requestor-cid\n    surface: classic REST (Advertiser Lookup, Publisher Lookup, Commission Detail Legacy)\n    required: true\n  - name: companyId\n    surface: GraphQL ads API\n    required: true\n  - name: publisherCompanyId\n    surface: Publisher Tracking API\n    required: true\n  - name: enterpriseId\n    surface: GraphQL Tracking API mutations\n    required: true\n    note: 'Returns \"Unauthorized\" when the enterprise id is not associated with the token.'\n  - name: forPublishers / forAdvertisers\n    surface: GraphQL Commission Detail\n  side_restrictions: >-\n    CJ additionally gates APIs by which side of the network you are on. Link\n    Search, Advertiser Lookup and\
  \ the Automated Offer Feed are publishers-only;\n    Publisher Lookup and the Tracking API are advertisers-only. Using a\n    publisher key against Publisher Lookup returns HTTP 400 \"Not Authorized\" —\n    not 401 and not 403.\n  actor_requirements: >-\n    The Click Events API requires a token generated by a user registered to the\n    PARTNER's CJ account; the Publisher Tracking API requires one from a user\n    registered to the PUBLISHER account. A token from the wrong account fails\n    even when it is valid.\nobserved_challenges:\n- host: link-search.api.cj.com\n  probe: 'GET /v2/link-search with no Authorization header'\n  status: 401\n  body: '<cj-api><error-message>You must provide an Authorization header.</error-message></cj-api>'\n  www_authenticate: absent\n- host: commission-detail.api.cj.com\n  probe: 'GET /v3/commissions with no Authorization header'\n  status: 401\n  body: '<cj-api><error-message>You must provide an Authorization header.</error-message></cj-api>'\n  www_authenticate:\
  \ absent\n- host: clicks.api.cj.com\n  probe: 'POST /partner/event with an empty JSON body and no Authorization header'\n  status: 401\n  body: '{\"destinationUrl\":\"\",\"errorMessages\":[\"Authentication failed\"]}'\n- host: publishertracking.api.cj.com\n  probe: 'POST /clickdestination with an empty JSON body and no Authorization header'\n  status: 401\n  body: '{\"destinationUrl\":\"\",\"errorMessages\":[\"Authentication failed\"]}'\n- host: commissions.api.cj.com\n  probe: 'POST /query with an introspection query and no Authorization header'\n  status: 200\n  note: >-\n    GraphQL INTROSPECTION is open without credentials on all three GraphQL\n    endpoints. Only the data is gated.\ngaps:\n- No WWW-Authenticate challenge header on any 401, so a client cannot discover the scheme from a response.\n- No published token lifetime, rotation guidance or revocation API.\n- No programmatic issuance. Every credential requires a human in the CJ portal, which is the practical blocker on unattended\
  \ agent onboarding.\n- No scopes, so a token cannot be least-privileged. One token that can read commissions can also write orders if the account is entitled to.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/authentication/cj-affiliate-authentication.yml
summary_line: http · 1 scheme
tags:
- Affiliate Marketing
- Affiliate Network
- Commission
- Product Search
- Publishers
- Advertiser
- GraphQL
- E-Commerce
- Product Feeds
- Conversion Tracking
- Attribution
- Performance Marketing
- Retail
- Coupons
---
