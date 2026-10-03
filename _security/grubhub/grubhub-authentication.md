---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: grubhub-delivery-quotes-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Quotes API
  slug: grubhub-delivery-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-quotes-api-openapi.yml
- filename: grubhub-delivery-refunds-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Refunds API
  slug: grubhub-delivery-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-refunds-api-openapi.yml
- filename: grubhub-delivery-service-areas-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Service Areas API
  slug: grubhub-delivery-service-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-service-areas-api-openapi.yml
- filename: grubhub-delivery-status-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Status API
  slug: grubhub-delivery-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-status-api-openapi.yml
- filename: grubhub-delivery-tests-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Tests API
  slug: grubhub-delivery-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-tests-api-openapi.yml
- filename: grubhub-delivery-updates-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Updates API
  slug: grubhub-delivery-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-updates-api-openapi.yml
- filename: grubhub-delivery-webhooks-emulation-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Webhooks Emulation API
  slug: grubhub-delivery-webhooks-emulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-webhooks-emulation-api-openapi.yml
- filename: grubhub-endpoints-api-openapi.yml
  format: yaml
  label: Grubhub Endpoints API
  slug: grubhub-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-endpoints-api-openapi.yml
- filename: grubhub-requesting-reports-api-openapi.yml
  format: yaml
  label: Grubhub Requesting Reports API
  slug: grubhub-requesting-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-requesting-reports-api-openapi.yml
- filename: grubhub-webhooks-api-openapi.yml
  format: yaml
  label: Grubhub Webhooks API
  slug: grubhub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-webhooks-api-openapi.yml
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
- Delivery
---
