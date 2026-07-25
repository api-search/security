---
api_key_in: []
api_specs:
- filename: elation-api-authentication.json
  format: json
  label: Elation OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-api-authentication.json
- filename: elation-patient-profile-api.json
  format: json
  label: Elation Patient Profile API
  slug: patient-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-profile-api.json
- filename: elation-visit-notes-api.json
  format: json
  label: Elation Visit Notes API
  slug: visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-visit-notes-api.json
- filename: elation-patient-document-api.json
  format: json
  label: Elation Patient Document API
  slug: patient-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-document-api.json
- filename: elation-orders-api.json
  format: json
  label: Elation Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-orders-api.json
- filename: elation-scheduling-api.json
  format: json
  label: Elation Scheduling API
  slug: scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-scheduling-api.json
- filename: elation-billing-api.json
  format: json
  label: Elation Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-billing-api.json
- filename: elation-insurance-api.json
  format: json
  label: Elation Insurance API
  slug: insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-insurance-api.json
- filename: elation-premium-patient-insurance-api.json
  format: json
  label: Elation Patient Insurance API (Premium) & Eligibility
  slug: patient-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-premium-patient-insurance-api.json
- filename: elation-practice-api.json
  format: json
  label: Elation Practice API
  slug: practice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-practice-api.json
- filename: elation-user-management-api.json
  format: json
  label: Elation User Management API
  slug: user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-user-management-api.json
- filename: elation-messaging-api.json
  format: json
  label: Elation Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-messaging-api.json
- filename: elation-event-subscription-api.json
  format: json
  label: Elation Event Subscription API
  slug: event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-event-subscription-api.json
- filename: elation-reference-data-api.json
  format: json
  label: Elation Reference Data API
  slug: reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-reference-data-api.json
- filename: elation-care-gaps-api-1.json
  format: json
  label: Elation Care Gaps API
  slug: care-gaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-care-gaps-api-1.json
- filename: elation-elation-import-api.json
  format: json
  label: Elation Import API
  slug: import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-elation-import-api.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Elation Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Elation Health secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Elation Health
provider_slug: elation-health
scheme_count: 4
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/elation-api-authentication.json
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  sources:
  - openapi/elation-api-settings.json
  - openapi/elation-billing-api.json
  - openapi/elation-event-subscription-api.json
  - openapi/elation-insurance-api.json
  - openapi/elation-messaging-api.json
  - openapi/elation-orders-api.json
  - openapi/elation-patient-document-api.json
  - openapi/elation-patient-profile-api.json
  - openapi/elation-practice-api.json
  - openapi/elation-premium-patient-insurance-api.json
  - openapi/elation-reference-data-api.json
  - openapi/elation-scheduling-api.json
  - openapi/elation-user-management-api.json
  type: oauth2
- flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/elation-care-gaps-api-1.json
  - openapi/elation-elation-import-api.json
  type: oauth2
- name: RequireAuthentication
  scheme: bearer
  sources:
  - openapi/elation-visit-notes-api.json
  type: http
slug: elation-health-authentication
source_filename: elation-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/elation-api-authentication.json, openapi/elation-api-settings.json, openapi/elation-billing-api.json,\n  openapi/elation-care-gaps-api-1.json, openapi/elation-elation-import-api.json, openapi/elation-event-subscription-api.json,\n  openapi/elation-insurance-api.json, openapi/elation-messaging-api.json, openapi/elation-orders-api.json,\n  openapi/elation-patient-document-api.json, openapi/elation-patient-profile-api.json, openapi/elation-practice-api.json\n  ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elation-api-authentication.json\n- name: sec0\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/elation-api-settings.json\n  - openapi/elation-billing-api.json\n  - openapi/elation-event-subscription-api.json\n\
  \  - openapi/elation-insurance-api.json\n  - openapi/elation-messaging-api.json\n  - openapi/elation-orders-api.json\n  - openapi/elation-patient-document-api.json\n  - openapi/elation-patient-profile-api.json\n  - openapi/elation-practice-api.json\n  - openapi/elation-premium-patient-insurance-api.json\n  - openapi/elation-reference-data-api.json\n  - openapi/elation-scheduling-api.json\n  - openapi/elation-user-management-api.json\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/elation-care-gaps-api-1.json\n  - openapi/elation-elation-import-api.json\n- name: RequireAuthentication\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/elation-visit-notes-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/authentication/elation-health-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Primary Care
- Value-Based Care
- Eligibility
- Clinical Data
- Scheduling
- e-Prescribing
- Digital Health
---
