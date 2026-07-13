---
api_key_in: []
api_specs:
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Athlete API
  slug: trainingpeaks-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workouts API
  slug: trainingpeaks-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workout Details API
  slug: trainingpeaks-workout-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workout of the Day API
  slug: trainingpeaks-workout-of-the-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Metrics API
  slug: trainingpeaks-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Nutrition API
  slug: trainingpeaks-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Coach API
  slug: trainingpeaks-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks File Upload API
  slug: trainingpeaks-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Events and Routes API
  slug: trainingpeaks-events-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Webhooks API
  slug: trainingpeaks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trainingpeaks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TrainingPeaks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TrainingPeaks
provider_slug: trainingpeaks
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow. Tokens are short-lived (expires_in seconds) and refreshed with the refresh_token grant. Scopes are not inclusive (e.g. workouts:details does not include workouts:read) and are limited to those granted to your application.
  flows:
  - authorizationUrl: https://oauth.trainingpeaks.com/OAuth/Authorize
    flow: authorizationCode
    scopes: 17
    tokenUrl: https://oauth.trainingpeaks.com/oauth/token
  name: OAuth2
  sources:
  - openapi/trainingpeaks-openapi.yml
  type: oauth2
slug: trainingpeaks-authentication
source_filename: trainingpeaks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trainingpeaks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.trainingpeaks.com/OAuth/Authorize\n    tokenUrl: https://oauth.trainingpeaks.com/oauth/token\n    scopes: 17\n  description: OAuth 2.0 authorization code flow. Tokens are short-lived (expires_in seconds)\n    and refreshed with the refresh_token grant. Scopes are not inclusive (e.g. workouts:details\n    does not include workouts:read) and are limited to those granted to your application.\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/authentication/trainingpeaks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fitness
- Endurance Training
- Workouts
- Coaching
- Sports
- Health
- Wearables
---
