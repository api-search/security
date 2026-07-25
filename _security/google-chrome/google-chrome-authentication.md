---
api_key_in: []
api_specs:
- filename: google-chrome-app-details-api-openapi.yml
  format: yaml
  label: Google Chrome App Details API
  slug: google-chrome-app-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-app-details-api-openapi.yml
- filename: google-chrome-reports-api-openapi.yml
  format: yaml
  label: Google Chrome Reports API
  slug: google-chrome-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-reports-api-openapi.yml
- filename: google-chrome-telemetry-devices-api-openapi.yml
  format: yaml
  label: Google Chrome Telemetry Devices API
  slug: google-chrome-telemetry-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-telemetry-devices-api-openapi.yml
- filename: google-chrome-telemetry-events-api-openapi.yml
  format: yaml
  label: Google Chrome Telemetry Events API
  slug: google-chrome-telemetry-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-telemetry-events-api-openapi.yml
- filename: google-chrome-telemetry-notification-configs-api-openapi.yml
  format: yaml
  label: Google Chrome Telemetry Notification Configs API
  slug: google-chrome-telemetry-notification-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-telemetry-notification-configs-api-openapi.yml
- filename: google-chrome-telemetry-users-api-openapi.yml
  format: yaml
  label: Google Chrome Telemetry Users API
  slug: google-chrome-telemetry-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-telemetry-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Chrome Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Chrome secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Chrome
provider_slug: google-chrome
scheme_count: 1
schemes:
- description: Google OAuth 2.0 authentication. Requires appropriate Chrome Management API scopes.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-chrome-management-api-openapi.json
  type: oauth2
slug: google-chrome-authentication
source_filename: google-chrome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-chrome-management-api-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  description: Google OAuth 2.0 authentication. Requires appropriate Chrome Management API scopes.\n  sources:\n  - openapi/google-chrome-management-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/authentication/google-chrome-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Browser
- Chrome Extensions
- Developer Tools
- Web Platform
---
