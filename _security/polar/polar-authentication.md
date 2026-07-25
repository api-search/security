---
api_key_in: []
api_specs:
- filename: polar-cardio-load-api-openapi.yml
  format: yaml
  label: Polar Cardio load API
  slug: polar-cardio-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-cardio-load-api-openapi.yml
- filename: polar-continuous-heart-rate-api-openapi.yml
  format: yaml
  label: Polar Continuous Heart Rate API
  slug: polar-continuous-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-continuous-heart-rate-api-openapi.yml
- filename: polar-daily-activity-api-openapi.yml
  format: yaml
  label: Polar Daily activity API
  slug: polar-daily-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-daily-activity-api-openapi.yml
- filename: polar-daily-activity-deprecated-api-openapi.yml
  format: yaml
  label: Polar Daily activity (deprecated) API
  slug: polar-daily-activity-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-daily-activity-deprecated-api-openapi.yml
- filename: polar-elixir-trade-biosensing-api-openapi.yml
  format: yaml
  label: Polar Elixir&trade; Biosensing API
  slug: polar-elixir-trade-biosensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-elixir-trade-biosensing-api-openapi.yml
- filename: polar-exercises-api-openapi.yml
  format: yaml
  label: Polar Exercises API
  slug: polar-exercises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-exercises-api-openapi.yml
- filename: polar-exercises-deprecated-api-openapi.yml
  format: yaml
  label: Polar Exercises (deprecated) API
  slug: polar-exercises-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-exercises-deprecated-api-openapi.yml
- filename: polar-nightly-recharge-api-openapi.yml
  format: yaml
  label: Polar Nightly Recharge API
  slug: polar-nightly-recharge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-nightly-recharge-api-openapi.yml
- filename: polar-physical-info-api-openapi.yml
  format: yaml
  label: Polar Physical info API
  slug: polar-physical-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-physical-info-api-openapi.yml
- filename: polar-physical-info-deprecated-api-openapi.yml
  format: yaml
  label: Polar Physical info (deprecated) API
  slug: polar-physical-info-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-physical-info-deprecated-api-openapi.yml
- filename: polar-player-training-sessions-api-openapi.yml
  format: yaml
  label: Polar Player training sessions API
  slug: polar-player-training-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-player-training-sessions-api-openapi.yml
- filename: polar-pull-notifications-api-openapi.yml
  format: yaml
  label: Polar Pull notifications API
  slug: polar-pull-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-pull-notifications-api-openapi.yml
- filename: polar-sleep-api-openapi.yml
  format: yaml
  label: Polar Sleep API
  slug: polar-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-sleep-api-openapi.yml
- filename: polar-sleepwise-trade-api-openapi.yml
  format: yaml
  label: Polar SleepWise&trade; API
  slug: polar-sleepwise-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-sleepwise-trade-api-openapi.yml
- filename: polar-team-api-openapi.yml
  format: yaml
  label: Polar Team API
  slug: polar-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-team-api-openapi.yml
- filename: polar-team-training-sessions-api-openapi.yml
  format: yaml
  label: Polar Team training sessions API
  slug: polar-team-training-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-team-training-sessions-api-openapi.yml
- filename: polar-users-api-openapi.yml
  format: yaml
  label: Polar Users API
  slug: polar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-users-api-openapi.yml
- filename: polar-webhooks-api-openapi.yml
  format: yaml
  label: Polar Webhooks API
  slug: polar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Polar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Polar secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Polar
provider_slug: polar
scheme_count: 2
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/polar-accesslink-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://flow.polar.com/oauth2/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://polarremote.com/v2/oauth2/token
  name: OAuth2
  sources:
  - openapi/polar-accesslink-api-openapi.yml
  - openapi/polar-teampro-api-openapi.yml
  type: oauth2
slug: polar-authentication
source_filename: polar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polar-accesslink-api-openapi.yml, openapi/polar-teampro-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/polar-accesslink-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://flow.polar.com/oauth2/authorization\n    tokenUrl: https://polarremote.com/v2/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/polar-accesslink-api-openapi.yml\n  - openapi/polar-teampro-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/authentication/polar-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fitness
- Health
- Wearables
- Heart Rate
- Sports
- Training
- Sleep
- Activity Tracking
- Sensors
- Bluetooth
---
