---
api_key_in:
- header
api_specs:
- filename: mindbody-public-api-v6-openapi-original.yml
  format: yaml
  label: Mindbody Public API v6
  slug: public-api-v6
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-public-api-v6-openapi-original.yml
- filename: mindbody-webhooks-api-openapi-original.yml
  format: yaml
  label: Mindbody Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-webhooks-api-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mindbody Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mindbody secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mindbody
provider_slug: mindbody
scheme_count: 2
schemes:
- description: Mindbody-issued API key (server-to-server). Required on every request.
  in: header
  name: ApiKeyAuth
  parameter: API-Key
  sources:
  - openapi/mindbody-public-api-v6-openapi-original.yml
  - openapi/mindbody-webhooks-api-openapi-original.yml
  type: apiKey
- description: OpenID Connect bearer token issued by Mindbody Identity Service (signin.mindbodyonline.com). Required for endpoints that act on behalf of a staff or client user.
  flows:
  - authorizationUrl: https://signin.mindbodyonline.com/connect/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://signin.mindbodyonline.com/connect/token
  name: OAuth2
  sources:
  - openapi/mindbody-public-api-v6-openapi-original.yml
  type: oauth2
slug: mindbody-authentication
source_filename: mindbody-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mindbody-public-api-v6-openapi-original.yml, openapi/mindbody-webhooks-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: Mindbody-issued API key (server-to-server). Required on every request.\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n  - openapi/mindbody-webhooks-api-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.mindbodyonline.com/connect/authorize\n    tokenUrl: https://signin.mindbodyonline.com/connect/token\n    scopes: 5\n  description: OpenID Connect bearer token issued by Mindbody Identity Service (signin.mindbodyonline.com).\n    Required for endpoints that act on behalf of a staff or client user.\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/authentication/mindbody-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Fitness
- Wellness
- Beauty
- Scheduling
- Booking
- Point of Sale
- Studios
- Salons
- Spas
- Webhooks
---
