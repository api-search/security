---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Patients Know Best Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Patients Know Best secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Patients Know Best
provider_slug: patients-know-best
scheme_count: 1
schemes:
- applied_to: all FHIR resource and operation endpoints
  bearer: true
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://patientsknowbest.com/fhir/
  type: oauth2
slug: patients-know-best-authentication
source_filename: patients-know-best-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://patientsknowbest.com/fhir/\ndocs: https://wiki.patientsknowbest.com/space/api\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    The PKB FHIR API is secured with OAuth 2.0. Partner/system integrations\n    use the client-credentials (system-to-system) workflow to obtain a\n    bearer access token, which is presented on each FHIR request. OAuth 2.0\n    support was released April 2020 with further enhancements June 2020. The\n    published FHIR CapabilityStatement does not enumerate an oauth2 security\n    scheme block, so token and authorization endpoints are provisioned per\n    integrating organisation rather than advertised in metadata.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  bearer: true\n  sources:\n  - https://patientsknowbest.com/fhir/\n  applied_to: all FHIR resource and operation endpoints\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patients-know-best/refs/heads/main/authentication/patients-know-best-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Health
- Healthcare
- Electronic Health Records
- Personal Health Record
- FHIR
- Interoperability
- NHS
- Patient Data
- Medical Records
---
