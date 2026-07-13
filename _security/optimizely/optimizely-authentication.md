---
api_key_in:
- header
- query
api_specs:
- filename: optimizely-web-experimentation-openapi.yml
  format: yaml
  label: Optimizely Web Experimentation REST API
  slug: web-experimentation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-web-experimentation-openapi.yml
- filename: optimizely-feature-experimentation-openapi.yml
  format: yaml
  label: Optimizely Feature Experimentation REST API
  slug: feature-experimentation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-feature-experimentation-openapi.yml
- filename: optimizely-campaign-openapi.yml
  format: yaml
  label: Optimizely Campaign REST API
  slug: campaign
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-campaign-openapi.yml
- filename: optimizely-content-delivery-openapi.yml
  format: yaml
  label: Optimizely Content Delivery API
  slug: content-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-content-delivery-openapi.yml
- filename: optimizely-content-management-openapi.yml
  format: yaml
  label: Optimizely Content Management API
  slug: content-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-content-management-openapi.yml
- filename: optimizely-graph-openapi.yml
  format: yaml
  label: Optimizely Graph API
  slug: graph
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-graph-openapi.yml
- filename: optimizely-data-platform-openapi.yml
  format: yaml
  label: Optimizely Data Platform REST API
  slug: data-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-data-platform-openapi.yml
- filename: optimizely-cmp-openapi.yml
  format: yaml
  label: Optimizely CMP Open REST API
  slug: cmp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-cmp-openapi.yml
- filename: optimizely-commerce-service-openapi.yml
  format: yaml
  label: Optimizely Commerce Service API
  slug: commerce-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-commerce-service-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Optimizely Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Optimizely secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Optimizely
provider_slug: optimizely
scheme_count: 6
schemes:
- description: HTTP Basic authentication using the Optimizely Campaign API credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/optimizely-campaign-openapi.yml
  - openapi/optimizely-graph-openapi.yml
  type: http
- description: OAuth 2.0 authentication for the CMP API.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.cmp.optimizely.com/oauth/token
  name: oauth2
  sources:
  - openapi/optimizely-cmp-openapi.yml
  type: oauth2
- description: Bearer token for authenticated Commerce Service API access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/optimizely-commerce-service-openapi.yml
  - openapi/optimizely-content-delivery-openapi.yml
  - openapi/optimizely-content-management-openapi.yml
  - openapi/optimizely-feature-experimentation-openapi.yml
  - openapi/optimizely-web-experimentation-openapi.yml
  type: http
- description: Public API Key (Tracker ID) for sending data to ODP. May be exposed publicly on the internet.
  in: header
  name: publicApiKey
  parameter: x-api-key
  sources:
  - openapi/optimizely-data-platform-openapi.yml
  type: apiKey
- description: Single key authentication provides read-only access to publicly available GraphQL data. Use format epi-single followed by the token.
  in: query
  name: singleKeyAuth
  parameter: auth
  sources:
  - openapi/optimizely-graph-openapi.yml
  type: apiKey
- description: HMAC authentication for secure server-to-server access using App Key and App Secret.
  in: header
  name: hmacAuth
  parameter: Authorization
  sources:
  - openapi/optimizely-graph-openapi.yml
  type: apiKey
slug: optimizely-authentication
source_filename: optimizely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/optimizely-campaign-openapi.yml, openapi/optimizely-cmp-openapi.yml, openapi/optimizely-commerce-service-openapi.yml,\n  openapi/optimizely-content-delivery-openapi.yml, openapi/optimizely-content-management-openapi.yml,\n  openapi/optimizely-data-platform-openapi.yml, openapi/optimizely-feature-experimentation-openapi.yml,\n  openapi/optimizely-graph-openapi.yml, openapi/optimizely-web-experimentation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the Optimizely Campaign API credentials.\n  sources:\n  - openapi/optimizely-campaign-openapi.yml\n  - openapi/optimizely-graph-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.cmp.optimizely.com/oauth/token\n \
  \   scopes: 0\n  description: OAuth 2.0 authentication for the CMP API.\n  sources:\n  - openapi/optimizely-cmp-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for authenticated Commerce Service API access.\n  sources:\n  - openapi/optimizely-commerce-service-openapi.yml\n  - openapi/optimizely-content-delivery-openapi.yml\n  - openapi/optimizely-content-management-openapi.yml\n  - openapi/optimizely-feature-experimentation-openapi.yml\n  - openapi/optimizely-web-experimentation-openapi.yml\n- name: publicApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Public API Key (Tracker ID) for sending data to ODP. May be exposed publicly\n    on the internet.\n  sources:\n  - openapi/optimizely-data-platform-openapi.yml\n- name: singleKeyAuth\n  type: apiKey\n  in: query\n  parameter: auth\n  description: Single key authentication provides read-only access to publicly available GraphQL\n    data. Use format epi-single followed\
  \ by the token.\n  sources:\n  - openapi/optimizely-graph-openapi.yml\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC authentication for secure server-to-server access using App Key and App\n    Secret.\n  sources:\n  - openapi/optimizely-graph-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/authentication/optimizely-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- A/B Testing
- Content Management
- Customer Data
- E-Commerce
- Experimentation
- Feature Flags
- Marketing
---
