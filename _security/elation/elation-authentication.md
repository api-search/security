---
api_key_in: []
api_specs:
- filename: elation-allergies-api-openapi.yml
  format: yaml
  label: Elation Health Allergies API
  slug: elation-allergies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-allergies-api-openapi.yml
- filename: elation-appointments-api-openapi.yml
  format: yaml
  label: Elation Health Appointments API
  slug: elation-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-appointments-api-openapi.yml
- filename: elation-authentication-api-openapi.yml
  format: yaml
  label: Elation Health Authentication API
  slug: elation-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-authentication-api-openapi.yml
- filename: elation-billing-api-openapi.yml
  format: yaml
  label: Elation Health Billing API
  slug: elation-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-billing-api-openapi.yml
- filename: elation-insurance-api-openapi.yml
  format: yaml
  label: Elation Health Insurance API
  slug: elation-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-insurance-api-openapi.yml
- filename: elation-lab-orders-api-openapi.yml
  format: yaml
  label: Elation Health Lab Orders API
  slug: elation-lab-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-lab-orders-api-openapi.yml
- filename: elation-medications-api-openapi.yml
  format: yaml
  label: Elation Health Medications API
  slug: elation-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-medications-api-openapi.yml
- filename: elation-messaging-api-openapi.yml
  format: yaml
  label: Elation Health Messaging API
  slug: elation-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-messaging-api-openapi.yml
- filename: elation-patients-api-openapi.yml
  format: yaml
  label: Elation Health Patients API
  slug: elation-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-patients-api-openapi.yml
- filename: elation-physicians-api-openapi.yml
  format: yaml
  label: Elation Health Physicians API
  slug: elation-physicians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-physicians-api-openapi.yml
- filename: elation-practices-api-openapi.yml
  format: yaml
  label: Elation Health Practices API
  slug: elation-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-practices-api-openapi.yml
- filename: elation-problems-api-openapi.yml
  format: yaml
  label: Elation Health Problems API
  slug: elation-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-problems-api-openapi.yml
- filename: elation-visit-notes-api-openapi.yml
  format: yaml
  label: Elation Health Visit Notes API
  slug: elation-visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-visit-notes-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Elation Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Elation Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Elation Health
provider_slug: elation
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://sandbox.elationemr.com/api/2.0/oauth2/token/
  name: oauth2
  sources:
  - openapi/elation-elation-health-api-openapi.yml
  type: oauth2
slug: elation-authentication
source_filename: elation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elation-elation-health-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.elationemr.com/api/2.0/oauth2/token/\n    scopes: 1\n  sources:\n  - openapi/elation-elation-health-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/authentication/elation-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- EHR
- Electronic Health Records
- Primary Care
- Healthcare
- FHIR
- Clinical
- Patients
- Prescriptions
- Messaging
---
