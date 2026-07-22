---
api_key_in: []
api_specs:
- filename: physna-openapi-original.json
  format: json
  label: Physna Public API
  slug: physna-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Physna Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Physna secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Physna
provider_slug: physna
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://physna.okta.com/oauth2/default/v1/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://physna.okta.com/oauth2/default/v1/token
  - documented_scope: tenantApp roles
    flow: clientCredentials
    tokenUrl: https://physna.okta.com/oauth2/default/v1/token
  name: okta
  sources:
  - openapi/physna-openapi-original.json
  - https://physna.github.io/public-api-guide/api-reference/authentication.html
  type: oauth2
slug: physna-authentication
source_filename: physna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/physna-openapi-original.json\ndocs: https://physna.github.io/public-api-guide/api-reference/authentication.html\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nnotes: >-\n  The OpenAPI declares a single oauth2 scheme named \"okta\" using the\n  authorizationCode flow against Physna's Okta authorization server. The public\n  API guide documents machine-to-machine access via the OAuth 2.0\n  client_credentials grant: POST to the Okta token endpoint with HTTP Basic\n  auth (CLIENT_ID:CLIENT_SECRET) and body\n  `grant_type=client_credentials&scope=tenantApp roles`. The returned Bearer\n  access_token is valid for 36000 seconds (10 hours) and is sent as\n  `Authorization: Bearer <token>`. Requests are tenant-scoped and several\n  operations additionally carry an `X-PHYSNA-TENANTID` header. Client\n  credentials are provisioned via the /client-credentials endpoints.\nschemes:\n\
  - name: okta\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://physna.okta.com/oauth2/default/v1/authorize\n    tokenUrl: https://physna.okta.com/oauth2/default/v1/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://physna.okta.com/oauth2/default/v1/token\n    documented_scope: tenantApp roles\n  sources:\n  - openapi/physna-openapi-original.json\n  - https://physna.github.io/public-api-guide/api-reference/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/authentication/physna-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai
- 3D
- Geometric Search
- Manufacturing
- Engineering
- Machine Learning
- Search
- Computer Vision
- Product Development
---
