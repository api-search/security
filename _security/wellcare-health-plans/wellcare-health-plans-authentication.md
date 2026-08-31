---
api_key_in: []
api_specs:
- filename: wellcare-health-plans-condition-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Condition API
  slug: wellcare-health-plans-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-condition-api-openapi.yml
- filename: wellcare-health-plans-coverage-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Coverage API
  slug: wellcare-health-plans-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-coverage-api-openapi.yml
- filename: wellcare-health-plans-encounter-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Encounter API
  slug: wellcare-health-plans-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-encounter-api-openapi.yml
- filename: wellcare-health-plans-explanation-of-benefits-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Explanation of Benefits API
  slug: wellcare-health-plans-explanation-of-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-explanation-of-benefits-api-openapi.yml
- filename: wellcare-health-plans-immunization-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Immunization API
  slug: wellcare-health-plans-immunization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-immunization-api-openapi.yml
- filename: wellcare-health-plans-insurance-plan-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Insurance Plan API
  slug: wellcare-health-plans-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-insurance-plan-api-openapi.yml
- filename: wellcare-health-plans-location-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Location API
  slug: wellcare-health-plans-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-location-api-openapi.yml
- filename: wellcare-health-plans-medication-request-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Medication Request API
  slug: wellcare-health-plans-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-medication-request-api-openapi.yml
- filename: wellcare-health-plans-observation-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Observation API
  slug: wellcare-health-plans-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-observation-api-openapi.yml
- filename: wellcare-health-plans-organization-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Organization API
  slug: wellcare-health-plans-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-organization-api-openapi.yml
- filename: wellcare-health-plans-patient-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Patient API
  slug: wellcare-health-plans-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-patient-api-openapi.yml
- filename: wellcare-health-plans-practitioner-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Practitioner API
  slug: wellcare-health-plans-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-practitioner-api-openapi.yml
- filename: wellcare-health-plans-practitioner-role-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Practitioner Role API
  slug: wellcare-health-plans-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-practitioner-role-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wellcare Health Plans Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: WellCare Health Plans secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: WellCare Health Plans
provider_slug: wellcare-health-plans
scheme_count: 2
schemes:
- description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.
  flows:
  - authorizationUrl: https://partners.centene.com/oauth2/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://partners.centene.com/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/wellcare-fhir-patient-access-api-openapi.yml
  type: oauth2
- description: Bearer token from Centene Partner Portal OAuth 2.0 authorization.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wellcare-fhir-provider-directory-api-openapi.yml
  type: http
slug: wellcare-health-plans-authentication
source_filename: wellcare-health-plans-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellcare-fhir-patient-access-api-openapi.yml, openapi/wellcare-fhir-provider-directory-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://partners.centene.com/oauth2/authorize\n    tokenUrl: https://partners.centene.com/oauth2/token\n    scopes: 8\n  description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from Centene Partner Portal OAuth 2.0 authorization.\n  sources:\n  - openapi/wellcare-fhir-provider-directory-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/authentication/wellcare-health-plans-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fortune 500
---
