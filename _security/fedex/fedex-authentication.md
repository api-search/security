---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fedex-authorization-api-openapi.yml
  format: yaml
  label: FedEx API Authorization
  slug: fedex-api-authorization
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-authorization-api-openapi.yml
- filename: fedex-rate-api-openapi.yml
  format: yaml
  label: FedEx Rates and Transit Times API
  slug: fedex-rates-and-transit-times-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-rate-api-openapi.yml
- filename: fedex-ship-api-openapi.yml
  format: yaml
  label: FedEx Ship API
  slug: fedex-ship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-ship-api-openapi.yml
- filename: fedex-pickup-api-openapi.yml
  format: yaml
  label: FedEx Pickup Request API
  slug: fedex-pickup-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-pickup-api-openapi.yml
- filename: fedex-track-api-openapi.yml
  format: yaml
  label: FedEx Basic Integrated Visibility
  slug: fedex-basic-integrated-visibility
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-track-api-openapi.yml
- filename: fedex-regulatory-api-openapi.yml
  format: yaml
  label: FedEx Regulatory API
  slug: fedex-regulatory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-regulatory-api-openapi.yml
- filename: fedex-address-api-openapi.yml
  format: yaml
  label: FedEx Address API
  slug: fedex-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-address-api-openapi.yml
- filename: fedex-availability-api-openapi.yml
  format: yaml
  label: FedEx Availability API
  slug: fedex-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-availability-api-openapi.yml
- filename: fedex-commodity-api-openapi.yml
  format: yaml
  label: FedEx Commodity API
  slug: fedex-commodity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-commodity-api-openapi.yml
- filename: fedex-country-api-openapi.yml
  format: yaml
  label: FedEx Country API
  slug: fedex-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-country-api-openapi.yml
- filename: fedex-documents-api-openapi.yml
  format: yaml
  label: FedEx Documents API
  slug: fedex-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-documents-api-openapi.yml
- filename: fedex-dutytax-api-openapi.yml
  format: yaml
  label: FedEx Dutytax API
  slug: fedex-dutytax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-dutytax-api-openapi.yml
- filename: fedex-globaltrade-api-openapi.yml
  format: yaml
  label: FedEx Globaltrade API
  slug: fedex-globaltrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-globaltrade-api-openapi.yml
- filename: fedex-irc-api-openapi.yml
  format: yaml
  label: FedEx Irc API
  slug: fedex-irc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-irc-api-openapi.yml
- filename: fedex-location-api-openapi.yml
  format: yaml
  label: FedEx Location API
  slug: fedex-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-location-api-openapi.yml
- filename: fedex-webhook-api-openapi.yml
  format: yaml
  label: FedEx Webhook API
  slug: fedex-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-webhook-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fedex Authentication
name_suffix: Authentication
oauth_flows: []
overview: FedEx declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FedEx
provider_slug: fedex
scheme_count: 1
schemes:
- credentials:
    child_Key: Customer Key - login credential for an Integrator, Compatible or Proprietary Parent Child customer (csp_credentials / client_pc_credentials)
    child_secret: Customer Secret paired with child_Key
    client_id: API Key received during FedEx Developer Portal registration
    client_secret: Secret Key received during FedEx Developer Portal registration
  docs: https://developer.fedex.com/api/en-us/catalog/authorization/v1/docs.html
  flow: clientCredentials
  grant_types:
  - client_credentials
  - csp_credentials
  - client_pc_credentials
  header: 'authorization: Bearer <token>'
  name: oauth2
  notes:
  - FedEx APIs do not support Cross-Origin Resource Sharing (CORS).
  - 'Best practices: cache the access token until an HTTP 401 is observed, then regenerate; never expose the token to the browser or end user; use TLS 1.2 or higher.'
  - 'Token-endpoint thresholds per public IP: burst 3 hits/second over 5 seconds, average 1 hit/second over 2 minutes; violation returns 403 for 10 minutes (see rate-limits/).'
  request_content_type: application/x-www-form-urlencoded
  sandbox_token_url: https://apis-sandbox.fedex.com/oauth/token
  scopes: []
  token_lifetime: An OAuth token is valid for an hour (Quotas & rate limits guide FAQ)
  token_url: https://apis.fedex.com/oauth/token
  type: oauth2
slug: fedex-authentication
source_filename: fedex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://developer.fedex.com/api/en-us/catalog/authorization/v1/docs.html\ndocs: https://developer.fedex.com/api/en-us/catalog/authorization/v1/docs.html\nsummary: 'OAuth 2.0 bearer tokens. Every FedEx API request carries an authorization header holding a token obtained from POST https://apis.fedex.com/oauth/token (sandbox: https://apis-sandbox.fedex.com/oauth/token) with the API Key (client_id) and Secret Key (client_secret) issued per project in the Developer Portal. The published OpenAPI fragments model authorization as a required header parameter rather than a securityScheme; the oauth2 scheme in the working specs was added by API Evangelist from this documentation.'\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://apis.fedex.com/oauth/token\n  sandbox_token_url: https://apis-sandbox.fedex.com/oauth/token\n  request_content_type: application/x-www-form-urlencoded\n  grant_types:\n\
  \  - client_credentials\n  - csp_credentials\n  - client_pc_credentials\n  credentials:\n    client_id: API Key received during FedEx Developer Portal registration\n    client_secret: Secret Key received during FedEx Developer Portal registration\n    child_Key: Customer Key - login credential for an Integrator, Compatible or Proprietary Parent Child customer (csp_credentials / client_pc_credentials)\n    child_secret: Customer Secret paired with child_Key\n  token_lifetime: An OAuth token is valid for an hour (Quotas & rate limits guide FAQ)\n  header: 'authorization: Bearer <token>'\n  scopes: []\n  notes:\n  - FedEx APIs do not support Cross-Origin Resource Sharing (CORS).\n  - 'Best practices: cache the access token until an HTTP 401 is observed, then regenerate; never expose the token to the browser or end user; use TLS 1.2 or higher.'\n  - 'Token-endpoint thresholds per public IP: burst 3 hits/second over 5 seconds, average 1 hit/second over 2 minutes; violation returns 403 for 10\
  \ minutes (see rate-limits/).'\n  docs: https://developer.fedex.com/api/en-us/catalog/authorization/v1/docs.html\nrelated:\n  rate_limits: rate-limits/fedex-rate-limits.yml\n  best_practices: https://developer.fedex.com/api/en-us/guides/best-practices.html\n"
source_yaml_url: https://artifacts.apis.io/fedex/authentication/fedex-authentication.yml
summary_line: 1 scheme
tags:
- Address Validation
- Freight
- Logistics
- Pickup
- Ratings
- Shipping
- Tracking
- Webhook
- Fortune 100
---
