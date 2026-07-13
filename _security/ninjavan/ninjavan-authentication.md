---
api_key_in: []
api_specs:
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van OAuth API
  slug: ninjavan-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Order API
  slug: ninjavan-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Tracking API
  slug: ninjavan-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Webhooks API
  slug: ninjavan-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Tariff API
  slug: ninjavan-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van PUDO API
  slug: ninjavan-pudo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ninjavan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ninja Van secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ninja Van
provider_slug: ninjavan
scheme_count: 2
schemes:
- description: Ninja Van uses the OAuth2 client-credentials grant. POST your client_id, client_secret, and grant_type=client_credentials to /{countryCode}/2.0/oauth/access_token to receive a short-lived access token. The token should be cached with its expiry and regenerated within about five minutes of expiry, or whenever the API returns HTTP 401. Client credentials are issued per merchant during onboarding; production access additionally requires passing Ninja Van's integration audit.
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - openapi/ninjavan-openapi.yml
  - https://api-docs.ninjavan.co/
  tokenUrl: https://api.ninjavan.co/{countryCode}/2.0/oauth/access_token
  type: oauth2
- description: 'The OAuth2 access token is passed on every subsequent request as `Authorization: Bearer ACCESS_TOKEN`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ninjavan-openapi.yml
  type: http
slug: ninjavan-authentication
source_filename: ninjavan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/ninjavan-openapi.yml\nsummary:\n  types:\n  - oauth2\n  - http\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.ninjavan.co/{countryCode}/2.0/oauth/access_token\n  description: >-\n    Ninja Van uses the OAuth2 client-credentials grant. POST your client_id,\n    client_secret, and grant_type=client_credentials to\n    /{countryCode}/2.0/oauth/access_token to receive a short-lived access token.\n    The token should be cached with its expiry and regenerated within about five\n    minutes of expiry, or whenever the API returns HTTP 401. Client credentials\n    are issued per merchant during onboarding; production access additionally\n    requires passing Ninja Van's integration audit.\n  sources:\n  - openapi/ninjavan-openapi.yml\n  - https://api-docs.ninjavan.co/\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    The OAuth2 access token\
  \ is passed on every subsequent request as\n    `Authorization: Bearer ACCESS_TOKEN`.\n  sources:\n  - openapi/ninjavan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/authentication/ninjavan-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Logistics
- Last-Mile Delivery
- Shipping
- Southeast Asia
- Parcels
- Tracking
- Fulfillment
- E-commerce Logistics
- Waybill
- SaaS
---
