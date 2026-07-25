---
api_key_in: []
api_specs:
- filename: jefferson-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Jefferson Health Allergy Intolerance API
  slug: jefferson-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-allergy-intolerance-api-openapi.yml
- filename: jefferson-health-bulk-data-api-openapi.yml
  format: yaml
  label: Jefferson Health Bulk Data API
  slug: jefferson-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-bulk-data-api-openapi.yml
- filename: jefferson-health-condition-api-openapi.yml
  format: yaml
  label: Jefferson Health Condition API
  slug: jefferson-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-condition-api-openapi.yml
- filename: jefferson-health-document-reference-api-openapi.yml
  format: yaml
  label: Jefferson Health Document Reference API
  slug: jefferson-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-document-reference-api-openapi.yml
- filename: jefferson-health-encounter-api-openapi.yml
  format: yaml
  label: Jefferson Health Encounter API
  slug: jefferson-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-encounter-api-openapi.yml
- filename: jefferson-health-endpoint-api-openapi.yml
  format: yaml
  label: Jefferson Health Endpoint API
  slug: jefferson-health-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-endpoint-api-openapi.yml
- filename: jefferson-health-healthcare-service-api-openapi.yml
  format: yaml
  label: Jefferson Health Healthcare Service API
  slug: jefferson-health-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-healthcare-service-api-openapi.yml
- filename: jefferson-health-insurance-plan-api-openapi.yml
  format: yaml
  label: Jefferson Health Insurance Plan API
  slug: jefferson-health-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-insurance-plan-api-openapi.yml
- filename: jefferson-health-location-api-openapi.yml
  format: yaml
  label: Jefferson Health Location API
  slug: jefferson-health-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-location-api-openapi.yml
- filename: jefferson-health-medication-request-api-openapi.yml
  format: yaml
  label: Jefferson Health Medication Request API
  slug: jefferson-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-medication-request-api-openapi.yml
- filename: jefferson-health-metadata-api-openapi.yml
  format: yaml
  label: Jefferson Health Metadata API
  slug: jefferson-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-metadata-api-openapi.yml
- filename: jefferson-health-observation-api-openapi.yml
  format: yaml
  label: Jefferson Health Observation API
  slug: jefferson-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-observation-api-openapi.yml
- filename: jefferson-health-organization-api-openapi.yml
  format: yaml
  label: Jefferson Health Organization API
  slug: jefferson-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-organization-api-openapi.yml
- filename: jefferson-health-patient-api-openapi.yml
  format: yaml
  label: Jefferson Health Patient API
  slug: jefferson-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-patient-api-openapi.yml
- filename: jefferson-health-practitioner-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner API
  slug: jefferson-health-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-api-openapi.yml
- filename: jefferson-health-practitioner-role-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner Role API
  slug: jefferson-health-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-role-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Jefferson Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jefferson Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jefferson Health
provider_slug: jefferson-health
scheme_count: 1
schemes:
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize
    flow: authorizationCode
    scopes: 13
    tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml
  type: oauth2
slug: jefferson-health-authentication
source_filename: jefferson-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize\n    tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token\n    scopes: 13\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app\n    launches.\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/authentication/jefferson-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Academic Medical Center
- CARIN Blue Button
- CMS Interoperability
- Cures Act
- Da Vinci Plan-Net
- Epic
- FHIR
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Provider Directory
- SMART on FHIR
- US Core
- USCDI
---
