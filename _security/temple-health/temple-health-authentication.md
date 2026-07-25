---
api_key_in: []
api_specs:
- filename: temple-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Temple Health Allergy Intolerance API
  slug: temple-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-allergy-intolerance-api-openapi.yml
- filename: temple-health-bulk-data-api-openapi.yml
  format: yaml
  label: Temple Health Bulk Data API
  slug: temple-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-bulk-data-api-openapi.yml
- filename: temple-health-condition-api-openapi.yml
  format: yaml
  label: Temple Health Condition API
  slug: temple-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-condition-api-openapi.yml
- filename: temple-health-document-reference-api-openapi.yml
  format: yaml
  label: Temple Health Document Reference API
  slug: temple-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-document-reference-api-openapi.yml
- filename: temple-health-encounter-api-openapi.yml
  format: yaml
  label: Temple Health Encounter API
  slug: temple-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-encounter-api-openapi.yml
- filename: temple-health-medication-request-api-openapi.yml
  format: yaml
  label: Temple Health Medication Request API
  slug: temple-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-medication-request-api-openapi.yml
- filename: temple-health-metadata-api-openapi.yml
  format: yaml
  label: Temple Health Metadata API
  slug: temple-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-metadata-api-openapi.yml
- filename: temple-health-observation-api-openapi.yml
  format: yaml
  label: Temple Health Observation API
  slug: temple-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-observation-api-openapi.yml
- filename: temple-health-patient-api-openapi.yml
  format: yaml
  label: Temple Health Patient API
  slug: temple-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-patient-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Temple Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Temple Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Temple Health
provider_slug: temple-health
scheme_count: 1
schemes:
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    scopes: 13
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/temple-health-temple-health-fhir-r4-api-openapi.yml
  type: oauth2
slug: temple-health-authentication
source_filename: temple-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temple-health-temple-health-fhir-r4-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n    scopes: 13\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app\n    launches.\n  sources:\n  - openapi/temple-health-temple-health-fhir-r4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/authentication/temple-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Academic Medical Center
- CMS Interoperability
- Cures Act
- DSTU2
- Epic
- FHIR
- Fox Chase Cancer Center
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Price Transparency
- R4
- SMART on FHIR
- Temple University
- US Core
- USCDI
---
