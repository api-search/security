---
api_key_in: []
api_specs:
- filename: banno-consumer-api-openapi.yml
  format: yaml
  label: Banno Consumer API
  slug: banno-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-consumer-api-openapi.yml
- filename: banno-admin-api-openapi.yml
  format: yaml
  label: Banno Admin API
  slug: banno-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-admin-api-openapi.yml
- filename: banno-plugin-framework-openapi.yml
  format: yaml
  label: Banno Plugin Framework
  slug: banno-plugin-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-plugin-framework-openapi.yml
- filename: banno-authentication-framework-openapi.yml
  format: yaml
  label: Banno Authentication Framework
  slug: banno-authentication-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-authentication-framework-openapi.yml
- filename: jxchange-rest-openapi.yml
  format: yaml
  label: jXchange REST
  slug: jxchange-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/jxchange-rest-openapi.yml
- filename: jack-henry-payments-openapi.yml
  format: yaml
  label: Jack Henry Payments
  slug: jack-henry-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/jack-henry-payments-openapi.yml
- filename: enterprise-event-system-asyncapi.yml
  format: yaml
  label: Enterprise Event System
  slug: enterprise-event-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/asyncapi/enterprise-event-system-asyncapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Jack Henry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jack Henry & Associates secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jack Henry & Associates
provider_slug: jack-henry
scheme_count: 2
schemes:
- name: openIdConnect
  openIdConnectUrl: https://api.banno.com/a/oidc/.well-known/openid-configuration
  sources:
  - openapi/banno-admin-api-openapi.yml
  - openapi/banno-consumer-api-openapi.yml
  type: openIdConnect
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/banno-authentication-framework-openapi.yml
  - openapi/jack-henry-payments-openapi.yml
  - openapi/jxchange-rest-openapi.yml
  type: http
slug: jack-henry-authentication
source_filename: jack-henry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/banno-admin-api-openapi.yml, openapi/banno-authentication-framework-openapi.yml,\n  openapi/banno-consumer-api-openapi.yml, openapi/jack-henry-payments-openapi.yml, openapi/jxchange-rest-openapi.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.banno.com/a/oidc/.well-known/openid-configuration\n  sources:\n  - openapi/banno-admin-api-openapi.yml\n  - openapi/banno-consumer-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/banno-authentication-framework-openapi.yml\n  - openapi/jack-henry-payments-openapi.yml\n  - openapi/jxchange-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/authentication/jack-henry-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Financial Services
- Banking
- Core Banking
- Digital Banking
- Payments
- Lending
- Fraud
- Open Banking
- Community Banks
- Credit Unions
- Fintech
- OAuth
- OpenID Connect
---
