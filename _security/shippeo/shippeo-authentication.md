---
api_key_in: []
api_specs:
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo Transport Orders API
  slug: shippeo-transport-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo Positions API
  slug: shippeo-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo ETA and Status API
  slug: shippeo-eta-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo Event Subscriptions (Events-out Webhooks) API
  slug: shippeo-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: researched
name: Shippeo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shippeo secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shippeo
provider_slug: shippeo
scheme_count: 2
schemes:
- description: OAuth2 client-credentials. A client_id / client_secret pair is issued when you create an application in the Shippeo Developer Portal (each application corresponds to an API user / clientID). The client credentials are exchanged for an access token, which is then presented on API calls. The exact token endpoint is documented in the login-gated portal and is not reproduced here.
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - https://developers.shippeo.com/
  type: oauth2
- description: 'The OAuth2 access token is presented on each request as `Authorization: Bearer ACCESS_TOKEN`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shippeo-openapi.yml
  type: http
slug: shippeo-authentication
source_filename: shippeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: researched\nsource: developers.shippeo.com portal + public product documentation\nsummary:\n  types:\n  - oauth2\n  - http\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth2 client-credentials. A client_id / client_secret pair is issued when\n    you create an application in the Shippeo Developer Portal (each application\n    corresponds to an API user / clientID). The client credentials are\n    exchanged for an access token, which is then presented on API calls. The\n    exact token endpoint is documented in the login-gated portal and is not\n    reproduced here.\n  sources:\n  - https://developers.shippeo.com/\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    The OAuth2 access token is presented on each request as\n    `Authorization: Bearer ACCESS_TOKEN`.\n  sources:\n  - openapi/shippeo-openapi.yml\nnotes: >-\n  Shippeo is enterprise, customer-provisioned\
  \ - API credentials require a\n  contracted account. Shippeo additionally supports SSO with just-in-time (JIT)\n  user provisioning for platform/portal users, which is a login mechanism for\n  humans rather than an API authentication scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/authentication/shippeo-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Supply Chain
- Transportation Visibility
- Real-Time Visibility
- Logistics
- Shipment Tracking
- ETA
- Freight
- Supply Chain Visibility
- SaaS
---
