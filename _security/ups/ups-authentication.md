---
api_key_in: []
api_specs:
- filename: ups-address-validation-api-openapi.yml
  format: yaml
  label: UPS Address Validation API
  slug: ups-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-address-validation-api-openapi.yml
- filename: ups-oauth-api-openapi.yml
  format: yaml
  label: UPS OAuth API
  slug: ups-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-oauth-api-openapi.yml
- filename: ups-paperless-documents-api-openapi.yml
  format: yaml
  label: UPS Paperless Documents API
  slug: ups-paperless-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-paperless-documents-api-openapi.yml
- filename: ups-pickup-api-openapi.yml
  format: yaml
  label: UPS Pickup API
  slug: ups-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-pickup-api-openapi.yml
- filename: ups-rating-api-openapi.yml
  format: yaml
  label: UPS Rating API
  slug: ups-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-rating-api-openapi.yml
- filename: ups-shipping-api-openapi.yml
  format: yaml
  label: UPS Shipping API
  slug: ups-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-shipping-api-openapi.yml
- filename: ups-time-in-transit-api-openapi.yml
  format: yaml
  label: UPS Time In Transit API
  slug: ups-time-in-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-time-in-transit-api-openapi.yml
- filename: ups-tracking-api-openapi.yml
  format: yaml
  label: UPS Tracking API
  slug: ups-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-tracking-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ups Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: UPS secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: UPS
provider_slug: ups
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/ups-shipping-openapi.yml
  type: oauth2
- description: OAuth 2.0 bearer token from /security/v1/oauth/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ups-shipping-openapi.yml
  type: http
slug: ups-authentication
source_filename: ups-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ups-shipping-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/ups-shipping-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token from /security/v1/oauth/token\n  sources:\n  - openapi/ups-shipping-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/authentication/ups-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Logistics
- Shipping
- Fortune 500
- Supply Chain
---
