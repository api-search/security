---
api_key_in: []
api_specs:
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Quotations API
  slug: skydropx-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Shipments API
  slug: skydropx-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Orders and Labels API
  slug: skydropx-orders-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Pickups API
  slug: skydropx-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Address Templates API
  slug: skydropx-address-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Tracking API
  slug: skydropx-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Finance API
  slug: skydropx-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Catalog API
  slug: skydropx-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Skydropx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skydropx secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skydropx
provider_slug: skydropx
scheme_count: 2
schemes:
- description: 'Skydropx Pro API authentication. Exchange a client_id and client_secret at POST https://pro.skydropx.com/api/v1/oauth/token (Content-Type application/x-www-form-urlencoded, grant_type=client_credentials) for a Bearer access token, then send it as `Authorization: Bearer ACCESS_TOKEN`. Access tokens are valid for about two hours and must be refreshed. Requests are rate limited to roughly two per second.'
  flow: clientCredentials
  grantType: client_credentials
  name: oauth2ClientCredentials
  sources:
  - openapi/skydropx-openapi.yml
  - https://pro.skydropx.com/es-MX/api-docs
  tokenUrl: https://pro.skydropx.com/api/v1/oauth/token
  type: oauth2
- description: 'Classic Skydropx API authentication (base https://api.skydropx.com/v1). Pass your API key in the Authorization header as `Authorization: Token token=YOUR_API_KEY`. API keys are issued by Skydropx support on request. This scheme is documented but is not modeled in the Skydropx Pro OpenAPI.'
  in: header
  keyName: Authorization
  name: apiKeyToken
  sources:
  - https://docs.skydropx.com/
  - https://help.skydropx.com/articulos-cda/conectar-la-api-skydropx
  type: apiKey
slug: skydropx-authentication
source_filename: skydropx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/skydropx-openapi.yml\nsummary:\n  types:\n  - oauth2\n  - apiKey\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://pro.skydropx.com/api/v1/oauth/token\n  grantType: client_credentials\n  description: >-\n    Skydropx Pro API authentication. Exchange a client_id and client_secret at\n    POST https://pro.skydropx.com/api/v1/oauth/token (Content-Type\n    application/x-www-form-urlencoded, grant_type=client_credentials) for a\n    Bearer access token, then send it as `Authorization: Bearer ACCESS_TOKEN`.\n    Access tokens are valid for about two hours and must be refreshed. Requests\n    are rate limited to roughly two per second.\n  sources:\n  - openapi/skydropx-openapi.yml\n  - https://pro.skydropx.com/es-MX/api-docs\n- name: apiKeyToken\n  type: apiKey\n  in: header\n  keyName: Authorization\n  description: >-\n    Classic Skydropx API authentication (base https://api.skydropx.com/v1).\
  \ Pass\n    your API key in the Authorization header as\n    `Authorization: Token token=YOUR_API_KEY`. API keys are issued by Skydropx\n    support on request. This scheme is documented but is not modeled in the\n    Skydropx Pro OpenAPI.\n  sources:\n  - https://docs.skydropx.com/\n  - https://help.skydropx.com/articulos-cda/conectar-la-api-skydropx\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/authentication/skydropx-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Shipping
- Logistics
- Multi-Carrier
- Mexico
- Latin America
- Labels
- Rates
- Parcels
- Tracking
- Fulfillment
- SaaS
---
