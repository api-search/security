---
api_key_in: []
api_specs:
- filename: whoop-co-activity-id-mapping-api-openapi.yml
  format: yaml
  label: WHOOP Activity ID Mapping API
  slug: whoop-co-activity-id-mapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-activity-id-mapping-api-openapi.yml
- filename: whoop-co-cycle-api-openapi.yml
  format: yaml
  label: WHOOP Cycle API
  slug: whoop-co-cycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-cycle-api-openapi.yml
- filename: whoop-co-partner-api-openapi.yml
  format: yaml
  label: WHOOP Partner API
  slug: whoop-co-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-partner-api-openapi.yml
- filename: whoop-co-recovery-api-openapi.yml
  format: yaml
  label: WHOOP Recovery API
  slug: whoop-co-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-recovery-api-openapi.yml
- filename: whoop-co-sleep-api-openapi.yml
  format: yaml
  label: WHOOP Sleep API
  slug: whoop-co-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-sleep-api-openapi.yml
- filename: whoop-co-user-api-openapi.yml
  format: yaml
  label: WHOOP User API
  slug: whoop-co-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-user-api-openapi.yml
- filename: whoop-co-workout-api-openapi.yml
  format: yaml
  label: WHOOP Workout API
  slug: whoop-co-workout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-co-workout-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Whoop Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: WHOOP secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: WHOOP
provider_slug: whoop-co
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.prod.whoop.com/oauth/oauth2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.prod.whoop.com/oauth/oauth2/token
  name: OAuth
  sources:
  - openapi/whoop-api-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.prod.whoop.com/developer/v2/partner/token
  name: Trusted Partner
  sources:
  - openapi/whoop-api-openapi.yml
  type: oauth2
slug: whoop-co-authentication
source_filename: whoop-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whoop-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.prod.whoop.com/oauth/oauth2/auth\n    tokenUrl: https://api.prod.whoop.com/oauth/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/whoop-api-openapi.yml\n- name: Trusted Partner\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prod.whoop.com/developer/v2/partner/token\n    scopes: 1\n  sources:\n  - openapi/whoop-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/authentication/whoop-co-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Fitness
- Wearables
- Health
- Recovery
- Sleep
- Strain
- Heart Rate
- Workout
- Biometrics
---
