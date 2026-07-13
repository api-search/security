---
api_key_in: []
api_specs:
- filename: fortellis-appointments-openapi.yml
  format: yaml
  label: Fortellis Service Appointments API
  slug: fortellis-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-appointments-openapi.yml
- filename: fortellis-user-service-openapi.yml
  format: yaml
  label: Fortellis User / Booking Sessions API
  slug: fortellis-user-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-user-service-openapi.yml
- filename: fortellis-parts-store-openapi.yml
  format: yaml
  label: Fortellis Parts Store API
  slug: fortellis-parts-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-parts-store-openapi.yml
- filename: fortellis-pet-adoption-openapi.yml
  format: yaml
  label: Fortellis Reference Pet Adoption API
  slug: fortellis-pet-adoption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-pet-adoption-openapi.yml
- filename: fortellis-event-relay-webhook-openapi.yml
  format: yaml
  label: Fortellis Event Relay Webhook
  slug: fortellis-event-relay-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-event-relay-webhook-openapi.yml
- filename: fortellis-event-relay-data-plane-proxy-asyncapi.yml
  format: yaml
  label: Fortellis Event Relay Data Plane Proxy (AsyncAPI)
  slug: fortellis-event-relay-data-plane
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-event-relay-data-plane-proxy-asyncapi.yml
- filename: fortellis-hello-world-asyncapi.yml
  format: yaml
  label: Fortellis AsyncAPI Hello World Reference
  slug: fortellis-async-hello-world
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-hello-world-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cdk Global Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: CDK Global secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: CDK Global
provider_slug: cdk-global
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://identity.fortellis.io/oauth2/
    flow: implicit
    scopes: 1
  name: permission-model
  sources:
  - openapi/fortellis-appointments-openapi.yml
  - openapi/fortellis-parts-store-openapi.yml
  - openapi/fortellis-pet-adoption-openapi.yml
  - openapi/fortellis-user-service-openapi.yml
  type: oauth2
slug: cdk-global-authentication
source_filename: cdk-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fortellis-appointments-openapi.yml, openapi/fortellis-parts-store-openapi.yml,\n  openapi/fortellis-pet-adoption-openapi.yml, openapi/fortellis-user-service-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: permission-model\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://identity.fortellis.io/oauth2/\n    scopes: 1\n  sources:\n  - openapi/fortellis-appointments-openapi.yml\n  - openapi/fortellis-parts-store-openapi.yml\n  - openapi/fortellis-pet-adoption-openapi.yml\n  - openapi/fortellis-user-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/authentication/cdk-global-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automotive
- Dealer Management
- DMS
- Auto Retail
- F&I
- Fixed Operations
- Parts
- CRM
- Digital Retail
- Marketplace
- Developer Platform
- Events
- Webhooks
- AsyncAPI
---
