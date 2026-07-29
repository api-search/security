---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Sendcloud Shipments API v3
  slug: shipments-api-v3
  spec_type: OpenAPI
  url: https://sendcloud.dev/.openapi/v3/shipments/openapi.yaml
- filename: sendcloud-v3-orders-openapi.yml
  format: yaml
  label: Sendcloud Orders API v3
  slug: orders-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-orders-openapi.yml
- filename: sendcloud-v3-ship-an-order-openapi.yml
  format: yaml
  label: Sendcloud Ship an Order API v3
  slug: ship-an-order-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-ship-an-order-openapi.yml
- filename: sendcloud-v3-returns-openapi.yml
  format: yaml
  label: Sendcloud Returns API v3
  slug: returns-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-returns-openapi.yml
- filename: sendcloud-v3-service-points-openapi.yml
  format: yaml
  label: Sendcloud Service Points API v3
  slug: service-points-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-service-points-openapi.yml
- filename: sendcloud-v3-parcel-tracking-openapi.yml
  format: yaml
  label: Sendcloud Parcel Tracking API v3
  slug: parcel-tracking-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-parcel-tracking-openapi.yml
- filename: sendcloud-v3-parcel-documents-openapi.yml
  format: yaml
  label: Sendcloud Parcel Documents API v3
  slug: parcel-documents-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-parcel-documents-openapi.yml
- filename: sendcloud-v3-webhooks-openapi.yml
  format: yaml
  label: Sendcloud Webhooks API v3
  slug: webhooks-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-webhooks-openapi.yml
- filename: sendcloud-v3-event-subscriptions-openapi.yml
  format: yaml
  label: Sendcloud Event Subscriptions API v3
  slug: event-subscriptions-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-event-subscriptions-openapi.yml
- filename: sendcloud-v3-integrations-openapi.yml
  format: yaml
  label: Sendcloud Integrations API v3
  slug: integrations-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-integrations-openapi.yml
- filename: sendcloud-v3-analytics-openapi.yml
  format: yaml
  label: Sendcloud Analytics API v3
  slug: analytics-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-analytics-openapi.yml
- filename: sendcloud-v3-reporting-openapi.yml
  format: yaml
  label: Sendcloud Reporting API v3
  slug: reporting-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-reporting-openapi.yml
- filename: sendcloud-v2-parcels-openapi.yml
  format: yaml
  label: Sendcloud Parcels API v2
  slug: parcels-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-parcels-openapi.yml
- filename: sendcloud-v2-labels-openapi.yml
  format: yaml
  label: Sendcloud Labels API v2
  slug: labels-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-labels-openapi.yml
- filename: sendcloud-v2-tracking-openapi.yml
  format: yaml
  label: Sendcloud Tracking API v2
  slug: tracking-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-tracking-openapi.yml
- filename: sendcloud-v2-webhooks-openapi.yml
  format: yaml
  label: Sendcloud Webhooks API v2
  slug: webhooks-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-webhooks-openapi.yml
- filename: sendcloud-v2-integrations-openapi.yml
  format: yaml
  label: Sendcloud Integrations API v2
  slug: integrations-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-integrations-openapi.yml
- filename: sendcloud-v2-analytics-openapi.yml
  format: yaml
  label: Sendcloud Analytics API v2
  slug: analytics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-analytics-openapi.yml
- filename: sendcloud-v2-reporting-openapi.yml
  format: yaml
  label: Sendcloud Reporting API v2
  slug: reporting-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-reporting-openapi.yml
- filename: sendcloud-v2-parcel-documents-openapi.yml
  format: yaml
  label: Sendcloud Parcel Documents API v2
  slug: parcel-documents-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-parcel-documents-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sendcloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sendcloud secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sendcloud
provider_slug: sendcloud
scheme_count: 3
schemes:
- description: Basic Authentication using API key and secrets is currently the main authentication mechanism.
  name: HTTPBasicAuth
  scheme: basic
  sources:
  - openapi/sendcloud-shipments-openapi.yml
  - openapi/sendcloud-v2-analytics-openapi.yml
  - openapi/sendcloud-v2-integrations-openapi.yml
  - openapi/sendcloud-v2-labels-openapi.yml
  - openapi/sendcloud-v2-parcel-documents-openapi.yml
  - openapi/sendcloud-v2-parcels-openapi.yml
  - openapi/sendcloud-v2-reporting-openapi.yml
  - openapi/sendcloud-v2-tracking-openapi.yml
  - openapi/sendcloud-v3-analytics-openapi.yml
  - openapi/sendcloud-v3-event-subscriptions-openapi.yml
  - openapi/sendcloud-v3-integrations-openapi.yml
  - openapi/sendcloud-v3-orders-openapi.yml
  - openapi/sendcloud-v3-parcel-documents-openapi.yml
  - openapi/sendcloud-v3-parcel-tracking-openapi.yml
  - openapi/sendcloud-v3-reporting-openapi.yml
  - openapi/sendcloud-v3-returns-openapi.yml
  - openapi/sendcloud-v3-service-points-openapi.yml
  - openapi/sendcloud-v3-ship-an-order-openapi.yml
  type: http
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  sources:
  - openapi/sendcloud-shipments-openapi.yml
  - openapi/sendcloud-v2-analytics-openapi.yml
  - openapi/sendcloud-v2-integrations-openapi.yml
  - openapi/sendcloud-v2-labels-openapi.yml
  - openapi/sendcloud-v2-parcel-documents-openapi.yml
  - openapi/sendcloud-v2-parcels-openapi.yml
  - openapi/sendcloud-v2-reporting-openapi.yml
  - openapi/sendcloud-v2-tracking-openapi.yml
  - openapi/sendcloud-v3-analytics-openapi.yml
  - openapi/sendcloud-v3-event-subscriptions-openapi.yml
  - openapi/sendcloud-v3-integrations-openapi.yml
  - openapi/sendcloud-v3-orders-openapi.yml
  - openapi/sendcloud-v3-parcel-documents-openapi.yml
  - openapi/sendcloud-v3-parcel-tracking-openapi.yml
  - openapi/sendcloud-v3-reporting-openapi.yml
  - openapi/sendcloud-v3-returns-openapi.yml
  - openapi/sendcloud-v3-service-points-openapi.yml
  - openapi/sendcloud-v3-ship-an-order-openapi.yml
  - openapi/sendcloud-v3-webhooks-openapi.yml
  type: oauth2
- in: header
  name: Sendcloud-Signature
  parameter: Sendcloud-Signature
  sources:
  - openapi/sendcloud-v2-webhooks-openapi.yml
  - openapi/sendcloud-v3-webhooks-openapi.yml
  type: apiKey
slug: sendcloud-authentication
source_filename: sendcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sendcloud-shipments-openapi.yml, openapi/sendcloud-v2-analytics-openapi.yml,\n  openapi/sendcloud-v2-integrations-openapi.yml, openapi/sendcloud-v2-labels-openapi.yml, openapi/sendcloud-v2-parcel-documents-openapi.yml,\n  openapi/sendcloud-v2-parcels-openapi.yml, openapi/sendcloud-v2-reporting-openapi.yml, openapi/sendcloud-v2-tracking-openapi.yml,\n  openapi/sendcloud-v2-webhooks-openapi.yml, openapi/sendcloud-v3-analytics-openapi.yml, openapi/sendcloud-v3-event-subscriptions-openapi.yml,\n  openapi/sendcloud-v3-integrations-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: HTTPBasicAuth\n  type: http\n  scheme: basic\n  description: Basic Authentication using API key and secrets is currently the main authentication\n    mechanism.\n  sources:\n  - openapi/sendcloud-shipments-openapi.yml\n  - openapi/sendcloud-v2-analytics-openapi.yml\n\
  \  - openapi/sendcloud-v2-integrations-openapi.yml\n  - openapi/sendcloud-v2-labels-openapi.yml\n  - openapi/sendcloud-v2-parcel-documents-openapi.yml\n  - openapi/sendcloud-v2-parcels-openapi.yml\n  - openapi/sendcloud-v2-reporting-openapi.yml\n  - openapi/sendcloud-v2-tracking-openapi.yml\n  - openapi/sendcloud-v3-analytics-openapi.yml\n  - openapi/sendcloud-v3-event-subscriptions-openapi.yml\n  - openapi/sendcloud-v3-integrations-openapi.yml\n  - openapi/sendcloud-v3-orders-openapi.yml\n  - openapi/sendcloud-v3-parcel-documents-openapi.yml\n  - openapi/sendcloud-v3-parcel-tracking-openapi.yml\n  - openapi/sendcloud-v3-reporting-openapi.yml\n  - openapi/sendcloud-v3-returns-openapi.yml\n  - openapi/sendcloud-v3-service-points-openapi.yml\n  - openapi/sendcloud-v3-ship-an-order-openapi.yml\n- name: OAuth2ClientCreds\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n    scopes: 1\n  description: OAuth2 is a standardized protocol\
  \ for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n  sources:\n  - openapi/sendcloud-shipments-openapi.yml\n  - openapi/sendcloud-v2-analytics-openapi.yml\n  - openapi/sendcloud-v2-integrations-openapi.yml\n  - openapi/sendcloud-v2-labels-openapi.yml\n  - openapi/sendcloud-v2-parcel-documents-openapi.yml\n  - openapi/sendcloud-v2-parcels-openapi.yml\n  - openapi/sendcloud-v2-reporting-openapi.yml\n  - openapi/sendcloud-v2-tracking-openapi.yml\n  - openapi/sendcloud-v3-analytics-openapi.yml\n  - openapi/sendcloud-v3-event-subscriptions-openapi.yml\n  - openapi/sendcloud-v3-integrations-openapi.yml\n  - openapi/sendcloud-v3-orders-openapi.yml\n  - openapi/sendcloud-v3-parcel-documents-openapi.yml\n  - openapi/sendcloud-v3-parcel-tracking-openapi.yml\n\
  \  - openapi/sendcloud-v3-reporting-openapi.yml\n  - openapi/sendcloud-v3-returns-openapi.yml\n  - openapi/sendcloud-v3-service-points-openapi.yml\n  - openapi/sendcloud-v3-ship-an-order-openapi.yml\n  - openapi/sendcloud-v3-webhooks-openapi.yml\n- name: Sendcloud-Signature\n  type: apiKey\n  in: header\n  parameter: Sendcloud-Signature\n  sources:\n  - openapi/sendcloud-v2-webhooks-openapi.yml\n  - openapi/sendcloud-v3-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/authentication/sendcloud-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Shipping
- Logistics
- Ecommerce
- Carriers
- Labels
- Returns
- Tracking
- Europe
---
