---
api_key_in: []
api_specs:
- filename: das-technology-daswebapi-v1-openapi.yml
  format: yaml
  label: DAS Web API
  slug: das-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/das-technology/refs/heads/main/openapi/das-technology-daswebapi-v1-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Das Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: DAS Technology declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DAS Technology
provider_slug: das-technology
scheme_count: 1
schemes:
- declared_in_spec: false
  evidence:
    body: <Error><Message>Authorization has been denied for this request.</Message></Error>
    http_status: 401
    response_header: 'WWW-Authenticate: Bearer'
    url: https://api.digitalairstrike.com/v1/account/00000000-0000-0000-0000-000000000000
  in: header
  method: probed
  name: bearer
  parameter: Authorization
  scheme: bearer
  token_endpoint: null
  token_endpoint_note: POST https://api.digitalairstrike.com/token returns 404 and POST /oauth/token returns 404; no anonymous token or OIDC/OAuth discovery document was found on any host (see well-known/das-technology-well-known.yml).
  type: http
slug: das-technology-authentication
source_filename: das-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://api.digitalairstrike.com/v1/account/{accountGuid} (live unauthenticated GET, HTTP 401)\n  plus openapi/_original/das-technology-daswebapi-v1-swagger.json and\n  openapi/_original/das-technology-daswebapi-v2-swagger.json\napi: DAS Web API (DASWebAPI v1 + v2)\nnote: >-\n  Neither published Swagger 2.0 document declares a securityDefinitions block, so the\n  authentication profile could not be derived from the spec — it was PROBED from the live API.\n  An unauthenticated request to any v1 or v2 resource returns HTTP 401 with the header\n  `WWW-Authenticate: Bearer` and an XML error body, which establishes bearer-token\n  authentication as the deployed scheme. DAS Technology publishes no developer portal, no\n  authentication guide and no token endpoint that answers anonymously (both /token and\n  /oauth/token return 404), so how a bearer token is ISSUED is not publicly documented;\n  credentials appear to be provisioned\
  \ through the partner/dealer relationship. This is a\n  documentation gap on the provider's side, recorded here rather than guessed at.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  method: probed\n  evidence:\n    url: https://api.digitalairstrike.com/v1/account/00000000-0000-0000-0000-000000000000\n    http_status: 401\n    response_header: 'WWW-Authenticate: Bearer'\n    body: '<Error><Message>Authorization has been denied for this request.</Message></Error>'\n  declared_in_spec: false\n  token_endpoint: null\n  token_endpoint_note: >-\n    POST https://api.digitalairstrike.com/token returns 404 and POST /oauth/token returns 404;\n    no anonymous token or OIDC/OAuth discovery document was found on any host (see\n    well-known/das-technology-well-known.yml).\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key: false\nanonymous_operations: 0\ngaps:\n- id: security-not-declared\n  detail: >-\n    All 136 operations\
  \ across v1 and v2 are served behind bearer auth but neither Swagger\n    document carries a securityDefinitions block or an operation-level security requirement, so a\n    generated client will emit unauthenticated calls that 401.\n  remediation: >-\n    Add a securityDefinitions entry (type apiKey, name Authorization, in header — or migrate to\n    OpenAPI 3.x and declare an http/bearer scheme) and a top-level security requirement.\n- id: no-published-token-flow\n  detail: How a caller obtains a bearer token is not documented on any public DAS Technology surface.\n  remediation: Publish an authentication page describing the token grant, lifetime and refresh behavior.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/das-technology/refs/heads/main/authentication/das-technology-authentication.yml
summary_line: 1 scheme
tags:
- Company
- MarTech
- Automotive
- Automotive Retail
- Marketing
- Customer Data Platform
- Advertising
- Reputation Management
- Reviews
- Surveys
- Customer Experience
- Dealership
---
