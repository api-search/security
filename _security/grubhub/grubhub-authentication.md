---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: grubhub-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: grubhub-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: grubhub-merchant-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: grubhub-merchant-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-busy-intervals-openapi.yml
  format: yaml
  label: Grubhub Busy Intervals API
  slug: grubhub-busy-intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-busy-intervals-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: grubhub-deliveries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-connect-endpoints-openapi.yml
  format: yaml
  label: Grubhub Connect (Delivery as a Service) API
  slug: grubhub-connect-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-endpoints-openapi.yml
- filename: grubhub-connect-webhooks-openapi.yml
  format: yaml
  label: Grubhub Connect Webhooks
  slug: grubhub-connect-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-webhooks-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: grubhub-onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
- filename: grubhub-reporting-endpoints-openapi.yml
  format: yaml
  label: Grubhub Merchant Reporting API
  slug: grubhub-reporting-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-endpoints-openapi.yml
- filename: grubhub-reporting-webhooks-openapi.yml
  format: yaml
  label: Grubhub Reporting Webhooks
  slug: grubhub-reporting-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-webhooks-openapi.yml
- filename: grubhub-testing-openapi.yml
  format: yaml
  label: Grubhub Testing API
  slug: grubhub-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-testing-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Grubhub Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: Grubhub secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: Grubhub
provider_slug: grubhub
scheme_count: 2
schemes:
- description: Partner identity key issued by Grubhub during partner onboarding. Declared as a header parameter on 31 operations. It is required:true on the eight Onboarding operations (schema type string, format uuid) and required:false on the Connect (DaaS), Orders, Menu and Reporting operations that declare it.
  evidence:
  - openapi/grubhub-connect-endpoints-openapi.yml
  - openapi/grubhub-onboarding-openapi.yml
  - openapi/grubhub-orders-openapi.yml
  - openapi/grubhub-menu-openapi.yml
  - openapi/grubhub-reporting-endpoints-openapi.yml
  format: uuid
  in: header
  name: partnerKey
  operations: 31
  parameter: X-GH-PARTNER-KEY
  required_in_spec: mixed
  type: apiKey
- authorization_endpoint: https://api-gtm.grubhub.com/oauth2/authorize
  code_challenge_methods_supported:
  - S256
  - plain
  description: Grubhub runs an RFC 8414 OAuth 2.0 authorization server whose metadata is served anonymously from the partner API hosts. It advertises dynamic client registration (RFC 7591), PKCE with S256 and plain, client_secret_post token endpoint authentication, and the scopes openid and diner.
  discovery: well-known/grubhub-oauth-authorization-server.json
  evidence:
  - fetched: '2026-09-17'
    status: 200
    url: https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server
  issuer: https://api-gtm.grubhub.com
  name: grubhubOAuth
  registration_endpoint: https://api-gtm.grubhub.com/oauth/register
  scopes_supported:
  - openid
  - diner
  service_documentation: https://developer.grubhub.com
  token_endpoint: https://api-gtm.grubhub.com/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  type: oauth2
slug: grubhub-authentication
source_filename: grubhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  openapi/_harvested/*.json (Grubhub's own twelve OpenAPI documents, fetched 2026-09-17 from\n  https://developer.grubhub.com/resource/partner-docs/api-docs/) plus the live RFC 8414 document\n  at https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server\nnote: >-\n  Grubhub's partner OpenAPI documents declare NO components.securitySchemes. Authentication is\n  expressed instead as an explicit X-GH-PARTNER-KEY request header on 31 operations across the\n  Connect (DaaS), Menu, Orders, Onboarding and Reporting documents, and the Onboarding document\n  states in prose that merchant association/deactivation is validated \"using Oauth2\". The\n  OAuth authorization server is real and discoverable: it publishes RFC 8414 metadata\n  anonymously on both partner hosts.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorization_code\n  securityschemes_declared_in_spec:\
  \ false\n  mfa_or_signing: unknown\nschemes:\n- name: partnerKey\n  type: apiKey\n  in: header\n  parameter: X-GH-PARTNER-KEY\n  format: uuid\n  required_in_spec: mixed\n  description: >-\n    Partner identity key issued by Grubhub during partner onboarding. Declared as a header\n    parameter on 31 operations. It is required:true on the eight Onboarding operations (schema\n    type string, format uuid) and required:false on the Connect (DaaS), Orders, Menu and\n    Reporting operations that declare it.\n  operations: 31\n  evidence:\n  - openapi/grubhub-connect-endpoints-openapi.yml\n  - openapi/grubhub-onboarding-openapi.yml\n  - openapi/grubhub-orders-openapi.yml\n  - openapi/grubhub-menu-openapi.yml\n  - openapi/grubhub-reporting-endpoints-openapi.yml\n- name: grubhubOAuth\n  type: oauth2\n  description: >-\n    Grubhub runs an RFC 8414 OAuth 2.0 authorization server whose metadata is served\n    anonymously from the partner API hosts. It advertises dynamic client registration\n  \
  \  (RFC 7591), PKCE with S256 and plain, client_secret_post token endpoint authentication,\n    and the scopes openid and diner.\n  discovery: well-known/grubhub-oauth-authorization-server.json\n  issuer: https://api-gtm.grubhub.com\n  authorization_endpoint: https://api-gtm.grubhub.com/oauth2/authorize\n  token_endpoint: https://api-gtm.grubhub.com/oauth2/token\n  registration_endpoint: https://api-gtm.grubhub.com/oauth/register\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  scopes_supported:\n  - openid\n  - diner\n  service_documentation: https://developer.grubhub.com\n  evidence:\n  - url: https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server\n    status: 200\n    fetched: '2026-09-17'\nenvironments:\n- name: production\n  base_url: https://api-third-party-gtm.grubhub.com\n  issuer: https://api-gtm.grubhub.com\n- name: preproduction\n  base_url: https://api-third-party-gtm-pp.grubhub.com\n\
  \  issuer: https://api-order-taking-pp.grubhub.com\n  evidence:\n  - url: https://api-third-party-gtm-pp.grubhub.com/.well-known/oauth-authorization-server\n    status: 200\n    fetched: '2026-09-17'\ngaps:\n- No securitySchemes block in any published OpenAPI document, so no operation carries a machine-readable\n  security requirement; a client cannot tell from the contract which credential an operation needs.\n- No /.well-known/openid-configuration and no jwks_uri published on any host probed.\n- No /.well-known/oauth-protected-resource, so the resource-server side of RFC 9728 is undiscoverable.\n- The prose auth guide lives on developer.grubhub.com, which renders client-side from Contentful and\n  is not machine-readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/authentication/grubhub-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Food Delivery
- Restaurant
- Marketplace
- Online Ordering
- Point-of-Sale
- Logistics
- Last Mile Delivery
- Menu Management
- Hospitality
- Local Commerce
---
