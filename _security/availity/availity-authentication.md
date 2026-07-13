---
api_key_in: []
api_specs:
- filename: availity-eligibility-openapi.yml
  format: yaml
  label: Availity Eligibility & Benefits API
  slug: availity-eligibility-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-eligibility-openapi.yml
- filename: availity-claim-status-openapi.yml
  format: yaml
  label: Availity Claim Status API
  slug: availity-claims-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-status-openapi.yml
- filename: availity-claim-attachments-openapi.yml
  format: yaml
  label: Availity Claim Attachments API
  slug: availity-claim-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-attachments-openapi.yml
- filename: availity-service-reviews-openapi.yml
  format: yaml
  label: Availity Service Reviews (Prior Authorization) API
  slug: availity-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-service-reviews-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Availity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: availity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: availity
provider_slug: availity
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.availity.com/availity/v1/token
  name: oauth2
  sources:
  - openapi/availity-claim-attachments-openapi.yml
  - openapi/availity-claim-status-openapi.yml
  - openapi/availity-eligibility-openapi.yml
  - openapi/availity-service-reviews-openapi.yml
  type: oauth2
slug: availity-authentication
source_filename: availity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/availity-claim-attachments-openapi.yml, openapi/availity-claim-status-openapi.yml,\n  openapi/availity-eligibility-openapi.yml, openapi/availity-service-reviews-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.availity.com/availity/v1/token\n    scopes: 1\n  sources:\n  - openapi/availity-claim-attachments-openapi.yml\n  - openapi/availity-claim-status-openapi.yml\n  - openapi/availity-eligibility-openapi.yml\n  - openapi/availity-service-reviews-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/authentication/availity-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
