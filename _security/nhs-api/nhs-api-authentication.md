---
api_key_in: []
api_specs:
- filename: nhs-api-codesystem-api-openapi.yml
  format: yaml
  label: NHS API CodeSystem API
  slug: nhs-api-codesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-codesystem-api-openapi.yml
- filename: nhs-api-list-id-api-openapi.yml
  format: yaml
  label: NHS API List{id} API
  slug: nhs-api-list-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-list-id-api-openapi.yml
- filename: nhs-api-metadata-api-openapi.yml
  format: yaml
  label: NHS API Metadata API
  slug: nhs-api-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-metadata-api-openapi.yml
- filename: nhs-api-organization-api-openapi.yml
  format: yaml
  label: NHS API Organization API
  slug: nhs-api-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-organization-api-openapi.yml
- filename: nhs-api-organizationaffiliation-api-openapi.yml
  format: yaml
  label: NHS API OrganizationAffiliation API
  slug: nhs-api-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-organizationaffiliation-api-openapi.yml
- filename: nhs-api-r4-api-openapi.yml
  format: yaml
  label: NHS API R4 API
  slug: nhs-api-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-r4-api-openapi.yml
- filename: nhs-api-stu3-api-openapi.yml
  format: yaml
  label: NHS API STU3 API
  slug: nhs-api-stu3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-stu3-api-openapi.yml
- filename: nhs-api-valueset-api-openapi.yml
  format: yaml
  label: NHS API ValueSet API
  slug: nhs-api-valueset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-valueset-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nhs Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: NHS API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NHS API
provider_slug: nhs-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/e-referrals-service-api.yaml
  type: http
slug: nhs-api-authentication
source_filename: nhs-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/e-referrals-service-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/e-referrals-service-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/authentication/nhs-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- FHIR
- NHS
- UK
- HL7
- Electronic Prescriptions
- Patient Demographics
- GP Connect
- NHS Login
- Interoperability
---
