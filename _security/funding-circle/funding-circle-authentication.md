---
api_key_in: []
api_specs:
- filename: funding-circle-introducer-openapi.yml
  format: yaml
  label: Funding Circle Introducer API
  slug: funding-circle-introducer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/funding-circle/refs/heads/main/openapi/funding-circle-introducer-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Funding Circle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Funding Circle secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Funding Circle
provider_slug: funding-circle
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials grant (RFC 6749 Section 4.4). Base64-encode `client_id:client_secret` and POST to the token endpoint to receive an access_token valid for 24 hours. Send it as `Authorization: Bearer {access_token}` on every request except the presigned document-upload PUT.'
  flow: clientCredentials
  name: oauth2
  scopes: []
  sources:
  - openapi/funding-circle-introducer-openapi.yml
  token_ttl_seconds: 86400
  token_url_sandbox: https://auth.sandbox.api.fundingcircle.co.uk/oauth2/token
  type: oauth2
slug: funding-circle-authentication
source_filename: funding-circle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.fundingcircle.com/uk/partners/developer/api-doc/\ndocs: https://www.fundingcircle.com/uk/partners/developer/api-doc/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\nschemes:\n  - name: oauth2\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      OAuth 2.0 Client Credentials grant (RFC 6749 Section 4.4). Base64-encode\n      `client_id:client_secret` and POST to the token endpoint to receive an\n      access_token valid for 24 hours. Send it as `Authorization: Bearer\n      {access_token}` on every request except the presigned document-upload PUT.\n    token_url_sandbox: https://auth.sandbox.api.fundingcircle.co.uk/oauth2/token\n    token_ttl_seconds: 86400\n    scopes: []\n    sources: [openapi/funding-circle-introducer-openapi.yml]\nnotes:\n  - No OAuth scopes are documented (client-credentials, coarse-grained access).\n  - Do not attach the bearer token\
  \ to the presigned S3 document-upload PUT request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funding-circle/refs/heads/main/authentication/funding-circle-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Lending
- Small Business
- Fintech
- Loans
- Financial Services
- Payments
---
