---
api_key_in: []
api_specs:
- filename: google-adsense-accounts-api-openapi.yml
  format: yaml
  label: Google AdSense Management Accounts API
  slug: google-adsense-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-adsense/refs/heads/main/openapi/google-adsense-accounts-api-openapi.yml
- filename: google-adsense-adclients-api-openapi.yml
  format: yaml
  label: Google AdSense Management Adclients API
  slug: google-adsense-adclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-adsense/refs/heads/main/openapi/google-adsense-adclients-api-openapi.yml
- filename: google-adsense-adunits-api-openapi.yml
  format: yaml
  label: Google AdSense Management Adunits API
  slug: google-adsense-adunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-adsense/refs/heads/main/openapi/google-adsense-adunits-api-openapi.yml
- filename: google-adsense-payments-api-openapi.yml
  format: yaml
  label: Google AdSense Management Payments API
  slug: google-adsense-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-adsense/refs/heads/main/openapi/google-adsense-payments-api-openapi.yml
- filename: google-adsense-reports-generate-api-openapi.yml
  format: yaml
  label: Google AdSense Management Reports:generate API
  slug: google-adsense-reports-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-adsense/refs/heads/main/openapi/google-adsense-reports-generate-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Adsense Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google AdSense Management secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google AdSense Management
provider_slug: google-adsense
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
slug: google-adsense-authentication
source_filename: google-adsense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-adsense/refs/heads/main/authentication/google-adsense-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Ad Units
- AdSense
- Advertising
- Monetization
- Publishers
- Reports
- Revenue
---
