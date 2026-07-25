---
api_key_in: []
api_specs:
- filename: fitbit-user-api-openapi.yml
  format: yaml
  label: Fitbit User API
  slug: fitbit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-user-api-openapi.yml
- filename: fitbit-foods-api-openapi.yml
  format: yaml
  label: Fitbit Foods API
  slug: fitbit-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-foods-api-openapi.yml
- filename: fitbit-oauth2-api-openapi.yml
  format: yaml
  label: Fitbit Oauth2 API
  slug: fitbit-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-oauth2-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fitbit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fitbit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fitbit
provider_slug: fitbit
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    scopes: 15
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/fitbit-activity-api-openapi.yml
  - openapi/fitbit-body-api-openapi.yml
  - openapi/fitbit-devices-api-openapi.yml
  - openapi/fitbit-ecg-irn-api-openapi.yml
  - openapi/fitbit-friends-api-openapi.yml
  - openapi/fitbit-heart-rate-api-openapi.yml
  - openapi/fitbit-nutrition-api-openapi.yml
  - openapi/fitbit-sleep-api-openapi.yml
  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml
  - openapi/fitbit-subscriptions-api-openapi.yml
  - openapi/fitbit-user-api-openapi.yml
  type: oauth2
slug: fitbit-authentication
source_filename: fitbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fitbit-activity-api-openapi.yml, openapi/fitbit-body-api-openapi.yml, openapi/fitbit-devices-api-openapi.yml,\n  openapi/fitbit-ecg-irn-api-openapi.yml, openapi/fitbit-friends-api-openapi.yml, openapi/fitbit-heart-rate-api-openapi.yml,\n  openapi/fitbit-nutrition-api-openapi.yml, openapi/fitbit-sleep-api-openapi.yml, openapi/fitbit-spo2-breathing-temperature-api-openapi.yml,\n  openapi/fitbit-subscriptions-api-openapi.yml, openapi/fitbit-user-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n    scopes: 15\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-body-api-openapi.yml\n  - openapi/fitbit-devices-api-openapi.yml\n  - openapi/fitbit-ecg-irn-api-openapi.yml\n\
  \  - openapi/fitbit-friends-api-openapi.yml\n  - openapi/fitbit-heart-rate-api-openapi.yml\n  - openapi/fitbit-nutrition-api-openapi.yml\n  - openapi/fitbit-sleep-api-openapi.yml\n  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n  - openapi/fitbit-subscriptions-api-openapi.yml\n  - openapi/fitbit-user-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/authentication/fitbit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Wearable
- Health
- Fitness
- Activity Tracking
- Heart Rate
- Sleep
- Google
- IoT
---
