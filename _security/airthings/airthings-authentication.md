---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airthings-accounts-api-openapi.yml
  format: yaml
  label: Airthings Accounts API
  slug: airthings-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-accounts-api-openapi.yml
- filename: airthings-device-api-openapi.yml
  format: yaml
  label: Airthings Device API
  slug: airthings-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-device-api-openapi.yml
- filename: airthings-devices-api-openapi.yml
  format: yaml
  label: Airthings Devices API
  slug: airthings-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-devices-api-openapi.yml
- filename: airthings-health-api-openapi.yml
  format: yaml
  label: Airthings Health API
  slug: airthings-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-health-api-openapi.yml
- filename: airthings-locations-api-openapi.yml
  format: yaml
  label: Airthings Locations API
  slug: airthings-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-locations-api-openapi.yml
- filename: airthings-organizations-api-openapi.yml
  format: yaml
  label: Airthings Organizations API
  slug: airthings-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-organizations-api-openapi.yml
- filename: airthings-segments-api-openapi.yml
  format: yaml
  label: Airthings Segments API
  slug: airthings-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-segments-api-openapi.yml
- filename: airthings-sensor-api-openapi.yml
  format: yaml
  label: Airthings Sensor API
  slug: airthings-sensor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-sensor-api-openapi.yml
- filename: airthings-spaces-api-openapi.yml
  format: yaml
  label: Airthings Spaces API
  slug: airthings-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-spaces-api-openapi.yml
- filename: airthings-thresholds-api-openapi.yml
  format: yaml
  label: Airthings Thresholds API
  slug: airthings-thresholds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-thresholds-api-openapi.yml
- filename: airthings-webhooks-api-openapi.yml
  format: yaml
  label: Airthings Webhooks API
  slug: airthings-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Airthings Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Airthings secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Airthings
provider_slug: airthings
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.airthings.com/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://accounts-api.airthings.com/v1/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://accounts-api.airthings.com/v1/token
  name: AirthingsAccounts
  sources:
  - openapi/airthings-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/airthings-openapi.yaml
  type: http
slug: airthings-authentication
source_filename: airthings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/airthings-api-openapi.yml, openapi/airthings-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: AirthingsAccounts\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.airthings.com/authorize\n    tokenUrl: https://accounts-api.airthings.com/v1/token\n    scopes: 2\n  - flow: clientCredentials\n    tokenUrl: https://accounts-api.airthings.com/v1/token\n    scopes: 2\n  sources:\n  - openapi/airthings-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/airthings-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/airthings/authentication/airthings-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- AirQuality
- Radon
- Sensors
- IoT
---
