---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: stellantis-grouping-api-openapi.yml
  format: yaml
  label: Stellantis Grouping API
  slug: stellantis-grouping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-grouping-api-openapi.yml
- filename: stellantis-data-stream-api-openapi.yml
  format: yaml
  label: Stellantis Data Stream API
  slug: stellantis-data-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-data-stream-api-openapi.yml
- filename: stellantis-auth-api-openapi.yml
  format: yaml
  label: Stellantis Auth API
  slug: stellantis-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-auth-api-openapi.yml
- filename: stellantis-bugs-api-openapi.yml
  format: yaml
  label: Stellantis Bugs API
  slug: stellantis-bugs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-bugs-api-openapi.yml
- filename: stellantis-cloud-data-treatment-api-openapi.yml
  format: yaml
  label: Stellantis Vehicles API
  slug: stellantis-cloud-data-treatment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-data-treatment-api-openapi.yml
- filename: stellantis-cloud-docg-device-management-api-openapi.yml
  format: yaml
  label: Stellantis Cloud Docg Device Management API
  slug: stellantis-cloud-docg-device-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-docg-device-management-api-openapi.yml
- filename: stellantis-cloud-notification-center-api-openapi.yml
  format: yaml
  label: Stellantis Cloud Notification Center API
  slug: stellantis-cloud-notification-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-notification-center-api-openapi.yml
- filename: stellantis-connected-car-b2b-api-openapi.yml
  format: yaml
  label: Stellantis Capabilities API
  slug: stellantis-connected-car-b2b-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-connected-car-b2b-api-openapi.yml
- filename: stellantis-connected-car-b2c-api-openapi.yml
  format: yaml
  label: Stellantis Connected Car B2C API
  slug: stellantis-connected-car-b2c-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-connected-car-b2c-api-openapi.yml
- filename: stellantis-data-api-openapi.yml
  format: yaml
  label: Stellantis Data API
  slug: stellantis-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-data-api-openapi.yml
- filename: stellantis-feedback-api-openapi.yml
  format: yaml
  label: Stellantis Feedback API
  slug: stellantis-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-feedback-api-openapi.yml
- filename: stellantis-geofence-breaches-api-openapi.yml
  format: yaml
  label: Stellantis Geofence Breaches API
  slug: stellantis-geofence-breaches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofence-breaches-api-openapi.yml
- filename: stellantis-geofence-collection-api-openapi.yml
  format: yaml
  label: Stellantis Geofence Collection API
  slug: stellantis-geofence-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofence-collection-api-openapi.yml
- filename: stellantis-geofencing-notifications-api-openapi.yml
  format: yaml
  label: Stellantis Geofencing Notifications API
  slug: stellantis-geofencing-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofencing-notifications-api-openapi.yml
- filename: stellantis-hackathon-register-api-openapi.yml
  format: yaml
  label: Stellantis Hackathon Register API
  slug: stellantis-hackathon-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-hackathon-register-api-openapi.yml
- filename: stellantis-hackathon-unsubscribe-api-openapi.yml
  format: yaml
  label: Stellantis Hackathon Unsubscribe API
  slug: stellantis-hackathon-unsubscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-hackathon-unsubscribe-api-openapi.yml
- filename: stellantis-popup-api-openapi.yml
  format: yaml
  label: Stellantis Popup API
  slug: stellantis-popup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-popup-api-openapi.yml
- filename: stellantis-remote-api-openapi.yml
  format: yaml
  label: Stellantis Remote API
  slug: stellantis-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-remote-api-openapi.yml
- filename: stellantis-stream-api-openapi.yml
  format: yaml
  label: Stellantis Stream API
  slug: stellantis-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-stream-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: Stellantis Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Stellantis secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Stellantis
provider_slug: stellantis
scheme_count: 5
schemes:
- in: query
  name: api_keyAuth
  parameter: client_id
  sources:
  - openapi/stellantis-cloud-data-treatment-api-openapi.yml
  - openapi/stellantis-connected-car-b2b-api-openapi.yml
  - openapi/stellantis-connected-car-b2c-api-openapi.yml
  type: apiKey
- description: This API uses OAuth 2 with the implicit grant flow. [More info](https://api.example.com/docs/auth)
  flows:
  - authorizationUrl: https://api.mpsa.com/api/connectedcar/v2/oauth/authorize
    flow: implicit
    scopes: 47
  name: api_oauth
  sources:
  - openapi/stellantis-cloud-data-treatment-api-openapi.yml
  - openapi/stellantis-connected-car-b2c-api-openapi.yml
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/stellantis-cloud-platform-notification-webhooks-openapi.yml
  - openapi/stellantis-connected-car-b2b-api-openapi.yml
  - openapi/stellantis-connected-car-b2b-webhooks-openapi.yml
  - openapi/stellantis-connected-car-b2c-webhooks-openapi.yml
  type: http
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/stellantis-connected-vehicle-api-openapi.json
  type: apiKey
- in: header
  name: SDK-Cognito-Authorizer
  parameter: Authorization
  sources:
  - openapi/stellantis-connected-vehicle-api-openapi.json
  type: apiKey
slug: stellantis-authentication
source_filename: stellantis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/stellantis-cloud-data-treatment-api-openapi.yml, openapi/stellantis-cloud-platform-notification-webhooks-openapi.yml,\n  openapi/stellantis-connected-car-b2b-api-openapi.yml, openapi/stellantis-connected-car-b2b-webhooks-openapi.yml,\n  openapi/stellantis-connected-car-b2c-api-openapi.yml, openapi/stellantis-connected-car-b2c-webhooks-openapi.yml,\n  openapi/stellantis-connected-vehicle-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - implicit\nschemes:\n- name: api_keyAuth\n  type: apiKey\n  in: query\n  parameter: client_id\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2b-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- name: api_oauth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.mpsa.com/api/connectedcar/v2/oauth/authorize\n\
  \    scopes: 47\n  description: This API uses OAuth 2 with the implicit grant flow. [More info](https://api.example.com/docs/auth)\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/stellantis-cloud-platform-notification-webhooks-openapi.yml\n  - openapi/stellantis-connected-car-b2b-api-openapi.yml\n  - openapi/stellantis-connected-car-b2b-webhooks-openapi.yml\n  - openapi/stellantis-connected-car-b2c-webhooks-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/stellantis-connected-vehicle-api-openapi.json\n- name: SDK-Cognito-Authorizer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/stellantis-connected-vehicle-api-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/stellantis/authentication/stellantis-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Automotive
- Manufacturing
- Mobility
- Sustainability
---
