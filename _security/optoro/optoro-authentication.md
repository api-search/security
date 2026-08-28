---
api_key_in: []
api_specs:
- filename: optoro-auth-openapi.yml
  format: yaml
  label: Optoro Auth API
  slug: optoro-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-auth-openapi.yml
- filename: optoro-catalogs-openapi.yml
  format: yaml
  label: Optoro Catalogs API
  slug: optoro-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-catalogs-openapi.yml
- filename: optoro-facilities-openapi.yml
  format: yaml
  label: Optoro Facilities API
  slug: optoro-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-facilities-openapi.yml
- filename: optoro-rtv-openapi.yml
  format: yaml
  label: Optoro RTV Vendor API
  slug: optoro-rtv-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-rtv-openapi.yml
- filename: optoro-asn-openapi.yml
  format: yaml
  label: Optoro Inbound ASN API
  slug: optoro-inbound-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-asn-openapi.yml
- filename: optoro-external-bin-changes-openapi.yml
  format: yaml
  label: Optoro External Bin Changes API
  slug: optoro-external-bin-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-external-bin-changes-openapi.yml
- filename: optoro-drop-ship-openapi.yml
  format: yaml
  label: Optoro Drop Ship API
  slug: optoro-drop-ship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-drop-ship-openapi.yml
- filename: optoro-returns-portal-orders-openapi.yml
  format: yaml
  label: Optoro Returns Portal Orders API
  slug: optoro-returns-portal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-returns-portal-orders-openapi.yml
- filename: optoro-rmas-openapi.yml
  format: yaml
  label: Optoro Event Webhooks and Customer Endpoints
  slug: optoro-event-webhooks-and-customer-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-rmas-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Optoro Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Optoro secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Optoro
provider_slug: optoro
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/optoro-asn-openapi.yml
  - openapi/optoro-external-bin-changes-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.optiturn.com/oauth/token
  name: oAuth2
  sources:
  - openapi/optoro-catalogs-openapi.yml
  - openapi/optoro-drop-ship-openapi.yml
  - openapi/optoro-facilities-openapi.yml
  - openapi/optoro-rtv-openapi.yml
  type: oauth2
slug: optoro-authentication
source_filename: optoro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/optoro-asn-openapi.yml, openapi/optoro-catalogs-openapi.yml, openapi/optoro-drop-ship-openapi.yml,\n  openapi/optoro-external-bin-changes-openapi.yml, openapi/optoro-facilities-openapi.yml, openapi/optoro-rtv-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/optoro-asn-openapi.yml\n  - openapi/optoro-external-bin-changes-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.optiturn.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/optoro-catalogs-openapi.yml\n  - openapi/optoro-drop-ship-openapi.yml\n  - openapi/optoro-facilities-openapi.yml\n  - openapi/optoro-rtv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/authentication/optoro-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Returns Management
- Reverse Logistics
- Retail
- Supply Chain
- eCommerce
- Fulfillment
- Drop Ship
- Inventory
- Webhooks
- Order Management
---
