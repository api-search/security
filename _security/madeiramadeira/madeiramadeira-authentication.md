---
api_key_in:
- header
api_specs:
- filename: madeiramadeira-callbacks-api-openapi.yml
  format: yaml
  label: Madeiramadeira Callbacks API
  slug: madeiramadeira-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-callbacks-api-openapi.yml
- filename: madeiramadeira-categorias-api-openapi.yml
  format: yaml
  label: Madeiramadeira Categorias API
  slug: madeiramadeira-categorias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-categorias-api-openapi.yml
- filename: madeiramadeira-financeiro-api-openapi.yml
  format: yaml
  label: Madeiramadeira Financeiro API
  slug: madeiramadeira-financeiro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-financeiro-api-openapi.yml
- filename: madeiramadeira-frete-api-openapi.yml
  format: yaml
  label: Madeiramadeira Frete API
  slug: madeiramadeira-frete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-frete-api-openapi.yml
- filename: madeiramadeira-mensageria-api-openapi.yml
  format: yaml
  label: Madeiramadeira Mensageria API
  slug: madeiramadeira-mensageria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-mensageria-api-openapi.yml
- filename: madeiramadeira-pedido-api-openapi.yml
  format: yaml
  label: Madeiramadeira Pedido API
  slug: madeiramadeira-pedido-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-pedido-api-openapi.yml
- filename: madeiramadeira-produtos-api-openapi.yml
  format: yaml
  label: Madeiramadeira Produtos API
  slug: madeiramadeira-produtos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-produtos-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Madeiramadeira Authentication
name_suffix: Authentication
oauth_flows: []
overview: Madeiramadeira secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Madeiramadeira
provider_slug: madeiramadeira
scheme_count: 2
schemes:
- description: Seller token issued in the Portal Marketplace under Administracao > Integracao. Bound to the seller account; requires a completed registration with signed Terms and Conditions.
  in: header
  name: TOKENMM
  parameter: TOKENMM
  sources:
  - openapi/madeiramadeira-marketplace-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT issued by the Mensageria auth endpoint (POST /v1/mensageria/auth/generate-token) via Keycloak, exchanged for an MMTOKEN. Used by the Mensageria (messaging) surface.
  name: BearerJWT
  scheme: bearer
  sources:
  - openapi/madeiramadeira-marketplace-openapi.yml
  type: http
slug: madeiramadeira-authentication
source_filename: madeiramadeira-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/madeiramadeira-marketplace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: TOKENMM\n  type: apiKey\n  in: header\n  parameter: TOKENMM\n  description: Seller token issued in the Portal Marketplace under Administracao > Integracao.\n    Bound to the seller account; requires a completed registration with signed Terms and Conditions.\n  sources:\n  - openapi/madeiramadeira-marketplace-openapi.yml\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT issued by the Mensageria auth endpoint (POST /v1/mensageria/auth/generate-token)\n    via Keycloak, exchanged for an MMTOKEN. Used by the Mensageria (messaging) surface.\n  sources:\n  - openapi/madeiramadeira-marketplace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/authentication/madeiramadeira-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Home Goods
- Furniture
- Brazil
- Seller Integration
- Product Catalog
- Order
- Shipping
- Logistics
---
