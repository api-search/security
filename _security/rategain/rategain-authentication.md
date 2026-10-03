---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rategain-developer-portal-api-openapi.yml
  format: yaml
  label: RateGain Developer Portal API
  slug: rategain-developer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rategain/refs/heads/main/openapi/rategain-developer-portal-api-openapi.yml
- filename: rategain-our-products-api-openapi.yml
  format: yaml
  label: RateGain Our Products API
  slug: rategain-our-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rategain/refs/heads/main/openapi/rategain-our-products-api-openapi.yml
- filename: rategain-ultradirect-api-openapi.yml
  format: yaml
  label: RateGain Ultradirect API
  slug: rategain-ultradirect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rategain/refs/heads/main/openapi/rategain-ultradirect-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rategain Authentication
name_suffix: Authentication
oauth_flows: []
overview: RateGain declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RateGain
provider_slug: rategain
scheme_count: 3
schemes:
- evidence: All request messages exchanged between the OTA and DirectConnect must be authenticated using the  Basic Authorization. This is sent in HttpRequest Header.
  header: Authorization
  location: header
  name: Basic Authorization
  type: http-basic
- evidence: 'Smart Distribution uses **API Key–based authentication**. Every request to the API must include the following headers:


    ```

    ApiKey: <Your unique API key>

    ApiSecret: <Your API secret>

    ```'
  header: ApiKey
  location: header
  name: ApiKey
  type: apiKey
- evidence: 'Smart Distribution uses **API Key–based authentication**. Every request to the API must include the following headers:


    ```

    ApiKey: <Your unique API key>

    ApiSecret: <Your API secret>

    ```'
  header: ApiSecret
  location: header
  name: ApiSecret
  type: apiKey
slug: rategain-authentication
source_filename: rategain-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.rategain.com/our-products/channel-manager/direct-connect-demand-push/interface-specifications-reservation-notification-service/technical-overview/authentication.md
source_yaml: "generated: '2026-09-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.rategain.com/our-products/channel-manager/direct-connect-demand-push/interface-specifications-reservation-notification-service/technical-overview/authentication.md\nsources:\n- https://developer.rategain.com/our-products/channel-manager/direct-connect-demand-push/interface-specifications-reservation-notification-service/technical-overview/authentication.md\n- https://developer.rategain.com/our-products/smart-distribution/developer-guide/authentication-method.md\n- https://developer.rategain.com/our-products/channel-manager/integration-and-onboarding-flow.md\n- https://developer.rategain.com/our-products/channel-manager/rg-bridge-supply-push/integration-overview/technical-feasibility-of-integration/test-property-setup.md\nschemes:\n- type: http-basic\n  name: Basic Authorization\n  evidence: All request messages exchanged between the OTA and DirectConnect must be\
  \ authenticated using the  Basic Authorization. This is sent\n    in HttpRequest Header.\n  location: header\n  header: Authorization\n- type: apiKey\n  name: ApiKey\n  evidence: 'Smart Distribution uses **API Key–based authentication**. Every request to the API must include the following headers:\n\n\n    ```\n\n    ApiKey: <Your unique API key>\n\n    ApiSecret: <Your API secret>\n\n    ```'\n  location: header\n  header: ApiKey\n- type: apiKey\n  name: ApiSecret\n  evidence: 'Smart Distribution uses **API Key–based authentication**. Every request to the API must include the following headers:\n\n\n    ```\n\n    ApiKey: <Your unique API key>\n\n    ApiSecret: <Your API secret>\n\n    ```'\n  location: header\n  header: ApiSecret\nnote: Credentials are obtained by contacting the @RateGain Team (for ApiKey/ApiSecret) or provided during onboarding (for Basic Authorization).\ndocs: https://developer.rategain.com/our-products/channel-manager/direct-connect-demand-push/interface-specifications-reservation-notification-service/technical-overview/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rategain/refs/heads/main/authentication/rategain-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Hospitality
- Travel Tech
- Software-as-a-Service
- Revenue Management
---
