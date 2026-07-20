---
api_key_in: []
api_specs:
- filename: alphaus-blueapi-openapi-original.json
  format: json
  label: Blue API
  slug: blue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-blueapi-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Alphaus Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alphaus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alphaus
provider_slug: alphaus
scheme_count: 1
schemes:
- credentials:
    client_id: Obtained from Ripple or WavePro (API client).
    client_secret: Obtained from Ripple or WavePro (API client).
  example: "curl -X POST \\\n  -F client_id={client-id} \\\n  -F client_secret={client-secret} \\\n  -F grant_type=client_credentials \\\n  -F scope=openid \\\n  https://login.alphaus.cloud/ripple/access_token\n"
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  scope: openid
  token_response:
  - access_token
  - token_type
  - expires_in
  - refresh_token
  token_urls:
  - product: ripple-octo
    url: https://login.alphaus.cloud/ripple/access_token
  - product: wavepro
    url: https://login.alphaus.cloud/access_token
  type: oauth2
  usage: 'Authorization: Bearer $ACCESS_TOKEN'
slug: alphaus-authentication
source_filename: alphaus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://labs.alphaus.cloud/docs/blueapi/authentication/\ndocs: https://labs.alphaus.cloud/docs/blueapi/authentication/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_header: 'Authorization: Bearer <token>'\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    grant_type: client_credentials\n    scope: openid\n    token_urls:\n      - product: ripple-octo\n        url: https://login.alphaus.cloud/ripple/access_token\n      - product: wavepro\n        url: https://login.alphaus.cloud/access_token\n    credentials:\n      client_id: Obtained from Ripple or WavePro (API client).\n      client_secret: Obtained from Ripple or WavePro (API client).\n    example: |\n      curl -X POST \\\n        -F client_id={client-id} \\\n        -F client_secret={client-secret} \\\n        -F grant_type=client_credentials \\\n        -F scope=openid \\\n        https://login.alphaus.cloud/ripple/access_token\n\
  \    token_response: [access_token, token_type, expires_in, refresh_token]\n    usage: 'Authorization: Bearer $ACCESS_TOKEN'\nnote: >-\n  The generated OpenAPI (grpc-gateway) does not declare securitySchemes, so this profile is captured\n  from the Blue API authentication docs (searched), not derived from the spec. RBAC/authorization is\n  managed via the Iam service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/authentication/alphaus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- FinOps
- Cloud Cost Management
- Cloud
- Billing
- Multi-Cloud
- Azure
- GCP
- gRPC
- Cost Optimization
- Reseller Billing
- API
---
