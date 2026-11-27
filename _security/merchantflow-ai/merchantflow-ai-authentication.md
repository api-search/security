---
anonymous_access: false
api_key_in: []
api_specs:
- filename: merchantflow-ai-metrics-api-openapi.yml
  format: yaml
  label: MerchantFlow Metrics API
  slug: merchantflow-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-metrics-api-openapi.yml
- filename: merchantflow-ai-orders-api-openapi.yml
  format: yaml
  label: MerchantFlow Orders API
  slug: merchantflow-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-orders-api-openapi.yml
- filename: merchantflow-ai-products-api-openapi.yml
  format: yaml
  label: MerchantFlow Products API
  slug: merchantflow-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-products-api-openapi.yml
- filename: merchantflow-ai-profitability-api-openapi.yml
  format: yaml
  label: MerchantFlow Profitability API
  slug: merchantflow-ai-profitability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-profitability-api-openapi.yml
- filename: merchantflow-ai-store-api-openapi.yml
  format: yaml
  label: MerchantFlow Store API
  slug: merchantflow-ai-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-store-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MerchantFlow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MerchantFlow secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MerchantFlow
provider_slug: merchantflow-ai
scheme_count: 1
schemes:
- description: 'OAuth 2.1 authorization code flow with PKCE (S256 required).


    Send the RFC 8707 resource indicator `resource=https://merchantflow.ai/api/v1` at both

    the authorize and token endpoints. If you omit it, MerchantFlow infers it from

    your requested scopes, but sending it explicitly is strongly preferred.


    Request `offline_access` alongside your data scopes to receive a refresh token;

    without it your acc'
  flows:
  - authorizationUrl: https://merchantflow.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://merchantflow.ai/api/auth/oauth2/token
  name: oauth2
  sources:
  - openapi/merchantflow-ai-openapi.json
  type: oauth2
slug: merchantflow-ai-authentication
source_filename: merchantflow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/merchantflow-ai-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://merchantflow.ai/api/auth/oauth2/authorize\n    tokenUrl: https://merchantflow.ai/api/auth/oauth2/token\n    scopes: 9\n  description: |-\n    OAuth 2.1 authorization code flow with PKCE (S256 required).\n\n    Send the RFC 8707 resource indicator `resource=https://merchantflow.ai/api/v1` at both\n    the authorize and token endpoints. If you omit it, MerchantFlow infers it from\n    your requested scopes, but sending it explicitly is strongly preferred.\n\n    Request `offline_access` alongside your data scopes to receive a refresh token;\n    without it your acc\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/merchantflow-ai/authentication/merchantflow-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- E-Commerce
- Analytics
- Software-as-a-Service
- Profitability
- Shopify
- WooCommerce
---
