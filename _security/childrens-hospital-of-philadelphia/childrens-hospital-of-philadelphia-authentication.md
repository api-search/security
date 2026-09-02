---
api_key_in: []
api_specs:
- filename: childrens-hospital-of-philadelphia-bulk-data-api-openapi.yml
  format: yaml
  label: Children's Hospital of Philadelphia Bulk Data API
  slug: childrens-hospital-of-philadelphia-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/openapi/childrens-hospital-of-philadelphia-bulk-data-api-openapi.yml
- filename: childrens-hospital-of-philadelphia-patient-access-api-openapi.yml
  format: yaml
  label: Children's Hospital of Philadelphia Patient Access API
  slug: childrens-hospital-of-philadelphia-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/openapi/childrens-hospital-of-philadelphia-patient-access-api-openapi.yml
- filename: childrens-hospital-of-philadelphia-provider-directory-api-openapi.yml
  format: yaml
  label: Children's Hospital of Philadelphia Provider Directory API
  slug: childrens-hospital-of-philadelphia-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/openapi/childrens-hospital-of-philadelphia-provider-directory-api-openapi.yml
- filename: childrens-hospital-of-philadelphia-smart-api-openapi.yml
  format: yaml
  label: Children's Hospital of Philadelphia SMART API
  slug: childrens-hospital-of-philadelphia-smart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/openapi/childrens-hospital-of-philadelphia-smart-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Childrens Hospital Of Philadelphia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Children's Hospital of Philadelphia secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Children's Hospital of Philadelphia
provider_slug: childrens-hospital-of-philadelphia
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://epicnsproxy.chop.edu/fhir/oauth2/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/chop-fhir-r4-openapi.yml
  type: oauth2
slug: childrens-hospital-of-philadelphia-authentication
source_filename: childrens-hospital-of-philadelphia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chop-fhir-r4-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicnsproxy.chop.edu/fhir/oauth2/authorize\n    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token\n    scopes: 5\n  - flow: clientCredentials\n    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/authentication/childrens-hospital-of-philadelphia-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Pediatrics
- FHIR
- SMART on FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Research Data
- Open Data
---
