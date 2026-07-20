---
api_key_in: []
api_specs:
- filename: cobee-public-api-openapi-original.json
  format: json
  label: Cobee Public API
  slug: cobee-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobee/refs/heads/main/openapi/cobee-public-api-openapi-original.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cobee Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cobee by Pluxee secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cobee by Pluxee
provider_slug: cobee
scheme_count: 2
schemes:
- flow: clientCredentials
  name: clientCredentials
  provider: Auth0
  request_fields:
  - clientId
  - clientSecret
  sources:
  - https://docs.api.cobee.io/en/api-reference/authentication
  token_url: /oauth/token
  type: oauth2
- bearer_format: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cobee-public-api-openapi-original.json
  type: http
slug: cobee-authentication
source_filename: cobee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cobee-public-api-openapi-original.json\ndocs: https://docs.api.cobee.io/en/api-reference/authentication\n# Upgraded from the derived http-bearer scheme using the provider's docs: the\n# bearer JWT is obtained via an OAuth 2.0 Client Credentials exchange (Auth0).\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer]\n  token_format: JWT (RS256, validated against Auth0 public keys)\n  token_claims: [companyId, corporationId]\nmodel: >-\n  Server-to-server. Exchange clientId + clientSecret (issued by the customer's\n  Customer Success Manager) at POST /oauth/token for a short-lived JWT, then send\n  it as `Authorization: Bearer <jwt>` on every request. Re-authenticate when the\n  JWT expires.\nschemes:\n  - name: clientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: /oauth/token\n    request_fields: [clientId, clientSecret]\n    provider: Auth0\n  \
  \  sources: [https://docs.api.cobee.io/en/api-reference/authentication]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    sources: [openapi/cobee-public-api-openapi-original.json]\nnotes: >-\n  The OpenAPI models only the resulting http bearer scheme; the OAuth2\n  client-credentials exchange is documented on the docs security/authentication\n  pages. No OAuth scopes are documented, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobee/refs/heads/main/authentication/cobee-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Employee Benefits
- Compensation
- Human Resources
- Payroll
- Fintech
- Spain
- Flexible Benefits
---
