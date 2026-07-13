---
api_key_in: []
api_specs:
- filename: deliverect-pos-api-openapi-original.yml
  format: yaml
  label: Deliverect POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-pos-api-openapi-original.yml
- filename: deliverect-commerce-api-openapi-original.yml
  format: yaml
  label: Deliverect Commerce API
  slug: commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-commerce-api-openapi-original.yml
- filename: deliverect-channel-api-openapi-original.yml
  format: yaml
  label: Deliverect Channel API
  slug: channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-channel-api-openapi-original.yml
- filename: deliverect-dispatch-api-openapi-original.yml
  format: yaml
  label: Deliverect Dispatch API
  slug: dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-dispatch-api-openapi-original.yml
- filename: deliverect-store-api-openapi-original.yml
  format: yaml
  label: Deliverect Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-store-api-openapi-original.yml
- filename: deliverect-pay-api-openapi-original.yml
  format: yaml
  label: Deliverect Pay API
  slug: pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-pay-api-openapi-original.yml
- filename: deliverect-crm-api-openapi-original.yml
  format: yaml
  label: Deliverect CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-crm-api-openapi-original.yml
- filename: deliverect-loyalty-api-openapi-original.yml
  format: yaml
  label: Deliverect Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-loyalty-api-openapi-original.yml
- filename: deliverect-kds-api-openapi-original.yml
  format: yaml
  label: Deliverect KDS API
  slug: kds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-kds-api-openapi-original.yml
- filename: deliverect-gift-cards-api-openapi-original.yml
  format: yaml
  label: Deliverect Gift Cards API
  slug: gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-gift-cards-api-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Deliverect Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Deliverect secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Deliverect
provider_slug: deliverect
scheme_count: 1
schemes:
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  sources:
  - openapi/deliverect-channel-api-openapi-original.yml
  - openapi/deliverect-commerce-api-openapi-original.yml
  - openapi/deliverect-crm-api-openapi-original.yml
  - openapi/deliverect-dispatch-api-openapi-original.yml
  - openapi/deliverect-gift-cards-api-openapi-original.yml
  - openapi/deliverect-kds-api-openapi-original.yml
  - openapi/deliverect-loyalty-api-openapi-original.yml
  - openapi/deliverect-pay-api-openapi-original.yml
  - openapi/deliverect-pos-api-openapi-original.yml
  - openapi/deliverect-store-api-openapi-original.yml
  type: oauth2
slug: deliverect-authentication
source_filename: deliverect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deliverect-channel-api-openapi-original.yml, openapi/deliverect-commerce-api-openapi-original.yml,\n  openapi/deliverect-crm-api-openapi-original.yml, openapi/deliverect-dispatch-api-openapi-original.yml,\n  openapi/deliverect-gift-cards-api-openapi-original.yml, openapi/deliverect-kds-api-openapi-original.yml,\n  openapi/deliverect-loyalty-api-openapi-original.yml, openapi/deliverect-pay-api-openapi-original.yml,\n  openapi/deliverect-pos-api-openapi-original.yml, openapi/deliverect-store-api-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n  sources:\n  - openapi/deliverect-channel-api-openapi-original.yml\n\
  \  - openapi/deliverect-commerce-api-openapi-original.yml\n  - openapi/deliverect-crm-api-openapi-original.yml\n  - openapi/deliverect-dispatch-api-openapi-original.yml\n  - openapi/deliverect-gift-cards-api-openapi-original.yml\n  - openapi/deliverect-kds-api-openapi-original.yml\n  - openapi/deliverect-loyalty-api-openapi-original.yml\n  - openapi/deliverect-pay-api-openapi-original.yml\n  - openapi/deliverect-pos-api-openapi-original.yml\n  - openapi/deliverect-store-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/authentication/deliverect-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Restaurant
- Delivery
- Online Ordering
- Point of Sale
- Order Management
- Integration
---
