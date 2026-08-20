---
api_key_in: []
api_specs:
- filename: alphaus-admin-api-openapi.yml
  format: yaml
  label: Alphaus Admin API
  slug: alphaus-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-admin-api-openapi.yml
- filename: alphaus-billing-api-openapi.yml
  format: yaml
  label: Alphaus Billing API
  slug: alphaus-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-billing-api-openapi.yml
- filename: alphaus-cost-api-openapi.yml
  format: yaml
  label: Alphaus Cost API
  slug: alphaus-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-cost-api-openapi.yml
- filename: alphaus-cover-api-openapi.yml
  format: yaml
  label: Alphaus Cover API
  slug: alphaus-cover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-cover-api-openapi.yml
- filename: alphaus-flags-api-openapi.yml
  format: yaml
  label: Alphaus Flags API
  slug: alphaus-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-flags-api-openapi.yml
- filename: alphaus-flow-api-openapi.yml
  format: yaml
  label: Alphaus Flow API
  slug: alphaus-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-flow-api-openapi.yml
- filename: alphaus-guaranteedcommitments-api-openapi.yml
  format: yaml
  label: Alphaus GuaranteedCommitments API
  slug: alphaus-guaranteedcommitments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-guaranteedcommitments-api-openapi.yml
- filename: alphaus-iam-api-openapi.yml
  format: yaml
  label: Alphaus Iam API
  slug: alphaus-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-iam-api-openapi.yml
- filename: alphaus-luster-api-openapi.yml
  format: yaml
  label: Alphaus Luster API
  slug: alphaus-luster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-luster-api-openapi.yml
- filename: alphaus-operations-api-openapi.yml
  format: yaml
  label: Alphaus Operations API
  slug: alphaus-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-operations-api-openapi.yml
- filename: alphaus-organization-api-openapi.yml
  format: yaml
  label: Alphaus Organization API
  slug: alphaus-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-organization-api-openapi.yml
- filename: alphaus-preferences-api-openapi.yml
  format: yaml
  label: Alphaus Preferences API
  slug: alphaus-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-preferences-api-openapi.yml
- filename: alphaus-pricing-api-openapi.yml
  format: yaml
  label: Alphaus Pricing API
  slug: alphaus-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-pricing-api-openapi.yml
- filename: alphaus-prism-api-openapi.yml
  format: yaml
  label: Alphaus Prism API
  slug: alphaus-prism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-prism-api-openapi.yml
- filename: alphaus-vortex-api-openapi.yml
  format: yaml
  label: Alphaus Vortex API
  slug: alphaus-vortex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-vortex-api-openapi.yml
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
---
