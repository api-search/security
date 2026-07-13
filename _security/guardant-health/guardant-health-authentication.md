---
api_key_in: []
api_specs:
- filename: guardant-health-openapi.yml
  format: yaml
  label: Guardant Health EMR Ordering Integration
  slug: guardant-health-emr-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-openapi.yml
- filename: guardant-health-openapi.yml
  format: yaml
  label: Guardant Health Results Delivery Integration
  slug: guardant-health-results-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Guardant Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Guardant Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Guardant Health
provider_slug: guardant-health
scheme_count: 1
schemes:
- description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding; no public auth flow is documented.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://example.invalid/guardant-health/oauth/token
  name: partnerOAuth2
  sources:
  - openapi/guardant-health-openapi.yml
  type: oauth2
slug: guardant-health-authentication
source_filename: guardant-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guardant-health-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: partnerOAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.invalid/guardant-health/oauth/token\n    scopes: 0\n  description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding;\n    no public auth flow is documented.\n  sources:\n  - openapi/guardant-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/authentication/guardant-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Precision Oncology
- Liquid Biopsy
- Genomics
- EMR Integration
---
