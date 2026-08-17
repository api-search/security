---
api_key_in: []
api_specs:
- filename: meditech-allergy-api-openapi.yml
  format: yaml
  label: meditech Allergy API
  slug: meditech-allergy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-allergy-api-openapi.yml
- filename: meditech-capability-api-openapi.yml
  format: yaml
  label: meditech Capability API
  slug: meditech-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-capability-api-openapi.yml
- filename: meditech-condition-api-openapi.yml
  format: yaml
  label: meditech Condition API
  slug: meditech-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-condition-api-openapi.yml
- filename: meditech-diagnostic-api-openapi.yml
  format: yaml
  label: meditech Diagnostic API
  slug: meditech-diagnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-diagnostic-api-openapi.yml
- filename: meditech-encounter-api-openapi.yml
  format: yaml
  label: meditech Encounter API
  slug: meditech-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-encounter-api-openapi.yml
- filename: meditech-medication-api-openapi.yml
  format: yaml
  label: meditech Medication API
  slug: meditech-medication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-medication-api-openapi.yml
- filename: meditech-observation-api-openapi.yml
  format: yaml
  label: meditech Observation API
  slug: meditech-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-observation-api-openapi.yml
- filename: meditech-patient-api-openapi.yml
  format: yaml
  label: meditech Patient API
  slug: meditech-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-patient-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Meditech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MEDITECH secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MEDITECH
provider_slug: meditech
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://yourhospital.meditech.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://yourhospital.meditech.com/oauth/token
  name: SMART_OAuth2
  sources:
  - openapi/meditech-allergy-api-openapi.yml
  - openapi/meditech-capability-api-openapi.yml
  - openapi/meditech-condition-api-openapi.yml
  - openapi/meditech-diagnostic-api-openapi.yml
  - openapi/meditech-encounter-api-openapi.yml
  - openapi/meditech-medication-api-openapi.yml
  - openapi/meditech-observation-api-openapi.yml
  - openapi/meditech-patient-api-openapi.yml
  type: oauth2
slug: meditech-authentication
source_filename: meditech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/meditech-allergy-api-openapi.yml, openapi/meditech-capability-api-openapi.yml,\n  openapi/meditech-condition-api-openapi.yml, openapi/meditech-diagnostic-api-openapi.yml, openapi/meditech-encounter-api-openapi.yml,\n  openapi/meditech-medication-api-openapi.yml, openapi/meditech-observation-api-openapi.yml,\n  openapi/meditech-patient-api-openapi.yml\nx-provenance:\n  reviewed: '2026-08-14'\n  origin: api-evangelist-derived\n  note: >-\n    Derived from an API Evangelist model of US Core FHIR R4, NOT from MEDITECH-published\n    material. The authorizationUrl/tokenUrl below use the `yourhospital` placeholder from that\n    model; real SMART on FHIR endpoints are issued per customer facility. For MEDITECH's actual\n    live Greenfield sandbox endpoints (verified first-hand, not a placeholder), see\n    authentication/meditech-greenfield-oauth.yml -- that file supersedes this one wherever they\n    disagree. Do not treat\
  \ the URLs below as callable.\n  reconcile_against: https://greenfield.meditech.com/explorer/authorization\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: SMART_OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourhospital.meditech.com/oauth/authorize\n    tokenUrl: https://yourhospital.meditech.com/oauth/token\n    scopes: 5\n  description: SMART on FHIR OAuth 2.0 authorization\n  sources:\n  - openapi/meditech-allergy-api-openapi.yml\n  - openapi/meditech-capability-api-openapi.yml\n  - openapi/meditech-condition-api-openapi.yml\n  - openapi/meditech-diagnostic-api-openapi.yml\n  - openapi/meditech-encounter-api-openapi.yml\n  - openapi/meditech-medication-api-openapi.yml\n  - openapi/meditech-observation-api-openapi.yml\n  - openapi/meditech-patient-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/authentication/meditech-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- EHR
- Healthcare
- FHIR
- HL7
- Interoperability
---
