---
api_key_in:
- path
api_specs:
- filename: appsamurai-campaign-spend-api-openapi.yml
  format: yaml
  label: Appsamurai Campaign Spend API
  slug: appsamurai-campaign-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-campaign-spend-api-openapi.yml
- filename: appsamurai-app-api-openapi.yml
  format: yaml
  label: Appsamurai App API
  slug: appsamurai-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-app-api-openapi.yml
- filename: appsamurai-audience-api-openapi.yml
  format: yaml
  label: Appsamurai Audience API
  slug: appsamurai-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-audience-api-openapi.yml
- filename: appsamurai-instance-api-openapi.yml
  format: yaml
  label: Appsamurai Instance API
  slug: appsamurai-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-instance-api-openapi.yml
- filename: appsamurai-segment-api-openapi.yml
  format: yaml
  label: Appsamurai Segment API
  slug: appsamurai-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-segment-api-openapi.yml
- filename: appsamurai-story-api-openapi.yml
  format: yaml
  label: Appsamurai Story API
  slug: appsamurai-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-story-api-openapi.yml
- filename: appsamurai-story-group-api-openapi.yml
  format: yaml
  label: Appsamurai Story Group API
  slug: appsamurai-story-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-story-group-api-openapi.yml
auth_types:
- http-bearer
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appsamurai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appsamurai secures its APIs with http-bearer and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Appsamurai
provider_slug: appsamurai
scheme_count: 2
schemes:
- api: Storyly External API
  applies_to: all 18 operations (declared per-operation, not as a root security requirement)
  bearer_format: JWT
  docs: https://docs.storyly.io/reference
  expiry: not documented
  gaps:
  - The spec declares no 401/403 responses, so a generated client has no failure path.
  - No token lifetime, refresh or revocation is documented.
  header: Authorization
  in: header
  issuance: Not documented publicly. No token endpoint appears in the OpenAPI, and docs.storyly.io publishes no token/credentials page - the JWT is obtained from the Storyly dashboard or an account contact.
  name: bearerAuth
  observed_behaviour:
    checked: '2026-08-13'
    method: probed
    probes:
    - body_code: TokenNotFound
      note: A missing credential returns 400, not the conventional 401.
      request: GET https://api.storyly.io/external/app with no Authorization header
      status: 400
    - body_code: InvalidToken
      request: GET https://api.storyly.io/external/app with an invalid bearer token
      status: 401
  rotation: not documented
  scheme: bearer
  sources:
  - openapi/appsamurai-storyly-external-api-openapi.json
  type: http
- api: AppSamurai Campaign Spend API
  docs: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api
  in: path
  issuance: manual (provided by an AppSamurai account manager)
  modelling_note: Represented in the OpenAPI as apiKey/in:query because OpenAPI 3.x has no in:path security scheme. The real placement is a path segment.
  name: PathApiKey
  parameter: api_key
  path_template: /api/customer-pull/spent/{api_key}
  risk:
    credential_in_url: true
    documented_over_http: true
    note: A secret in a path segment is written to every proxy log, browser history and referrer along the route, and the published base URL is http://, not https://. It also cannot be rotated by the customer. See security/appsamurai-domain-security.yml.
  rotation: not documented
  sources:
  - openapi/appsamurai-campaign-spend-api-openapi.yml
  type: apiKey
slug: appsamurai-authentication
source_filename: appsamurai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.storyly.io/reference +\n  openapi/appsamurai-storyly-external-api-openapi.json +\n  https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api\n  + live 400/401 probes of api.storyly.io (2026-08-13)\ndocs: https://docs.storyly.io/reference\nsummary:\n  types: [http-bearer, apiKey]\n  api_key_in: [path]\n  bearer_formats: [JWT]\n  oauth2_flows: []\n  openid_connect: false\n  mtls: false\n  notes: >-\n    Two APIs, two unrelated credentials, neither self-service. The Storyly\n    External API takes a bearer JWT; the AppSamurai Campaign Spend API takes an\n    account-scoped key embedded in the URL path. There is no OAuth, no OIDC, no\n    scope model and no documented token-issuance endpoint anywhere in App\n    Samurai's surface - both credentials are obtained out of band.\n    The MCP server is the outlier and the only unauthenticated surface:\n    mcp.storyly.io answered tools/list and\
  \ tools/call anonymously.\n\nschemes:\n  - name: bearerAuth\n    api: Storyly External API\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    applies_to: all 18 operations (declared per-operation, not as a root security requirement)\n    issuance: >-\n      Not documented publicly. No token endpoint appears in the OpenAPI, and\n      docs.storyly.io publishes no token/credentials page - the JWT is obtained\n      from the Storyly dashboard or an account contact.\n    rotation: not documented\n    expiry: not documented\n    sources:\n      - openapi/appsamurai-storyly-external-api-openapi.json\n    docs: https://docs.storyly.io/reference\n    observed_behaviour:\n      method: probed\n      checked: '2026-08-13'\n      probes:\n        - request: GET https://api.storyly.io/external/app with no Authorization header\n          status: 400\n          body_code: TokenNotFound\n          note: A missing credential returns 400, not the\
  \ conventional 401.\n        - request: GET https://api.storyly.io/external/app with an invalid bearer token\n          status: 401\n          body_code: InvalidToken\n    gaps:\n      - The spec declares no 401/403 responses, so a generated client has no failure path.\n      - No token lifetime, refresh or revocation is documented.\n\n  - name: PathApiKey\n    api: AppSamurai Campaign Spend API\n    type: apiKey\n    in: path\n    parameter: api_key\n    path_template: /api/customer-pull/spent/{api_key}\n    issuance: manual (provided by an AppSamurai account manager)\n    rotation: not documented\n    sources:\n      - openapi/appsamurai-campaign-spend-api-openapi.yml\n    docs: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api\n    risk:\n      credential_in_url: true\n      documented_over_http: true\n      note: >-\n        A secret in a path segment is written to every proxy log, browser history\n        and referrer along the route, and the published\
  \ base URL is http://, not\n        https://. It also cannot be rotated by the customer. See\n        security/appsamurai-domain-security.yml.\n    modelling_note: >-\n      Represented in the OpenAPI as apiKey/in:query because OpenAPI 3.x has no\n      in:path security scheme. The real placement is a path segment.\n\nunauthenticated_surfaces:\n  - name: Storyly Integration MCP server\n    url: https://mcp.storyly.io/mcp\n    auth: none\n    verified: probed\n    checked: '2026-08-13'\n    note: >-\n      tools/list and tools/call both answered anonymously. No OAuth challenge,\n      and no /.well-known/oauth-authorization-server or\n      /.well-known/oauth-protected-resource is served (both 404). It exposes\n      documentation content only, not customer data.\n  - name: Storyly External API OpenAPI\n    url: https://docs.storyly.io/openapi/68f9ff1ab2a841f03a72b06b\n    note: The specification is public; the operations it describes are not.\n\nscopes:\n  model: none\n  note: >-\n   \
  \ Neither credential carries scopes, roles or permissions. The Storyly JWT is\n    account-wide - any holder can create and delete story groups, stories and\n    segments across every app on the account. No scopes/ artifact is emitted\n    because there is nothing to enumerate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/authentication/appsamurai-authentication.yml
summary_line: http-bearer/apiKey · 2 schemes
tags:
- Company
- Mobile
- Advertising
- User Acquisition
- Marketing
- App Growth
- Attribution
- Analytics
- Mobile Marketing
- SDK
- Storyly
- Content Experience
- In-App Stories
- MCP
- Mobile Commerce
---
