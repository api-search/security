---
api_key_in: []
api_specs:
- filename: google-admob-accounts-api-openapi.yml
  format: yaml
  label: Google AdMob Accounts API
  slug: google-admob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-accounts-api-openapi.yml
- filename: google-admob-adunits-api-openapi.yml
  format: yaml
  label: Google AdMob adUnits API
  slug: google-admob-adunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-adunits-api-openapi.yml
- filename: google-admob-apps-api-openapi.yml
  format: yaml
  label: Google AdMob Apps API
  slug: google-admob-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-apps-api-openapi.yml
- filename: google-admob-mediationgroups-api-openapi.yml
  format: yaml
  label: Google AdMob mediationGroups API
  slug: google-admob-mediationgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-mediationgroups-api-openapi.yml
- filename: google-admob-networkreport-generate-api-openapi.yml
  format: yaml
  label: Google AdMob networkReport:generate API
  slug: google-admob-networkreport-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-networkreport-generate-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Admob Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google AdMob secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google AdMob
provider_slug: google-admob
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-admob-authentication
source_filename: google-admob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/authentication/google-admob-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Ad Mediation
- AdMob
- App Monetization
- Mobile Advertising
- Mobile Apps
- Reports
---
