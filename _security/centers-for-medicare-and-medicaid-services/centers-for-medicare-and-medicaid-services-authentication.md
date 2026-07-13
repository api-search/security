---
api_key_in: []
api_specs:
- filename: centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: cms-blue-button-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Centers For Medicare And Medicaid Services Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Centers for Medicare and Medicaid Services secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Centers for Medicare and Medicaid Services
provider_slug: centers-for-medicare-and-medicaid-services
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow used by Medicare beneficiaries to grant access to a third-party application.
  flows:
  - authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/
  name: oauth2
  sources:
  - openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
  type: oauth2
slug: centers-for-medicare-and-medicaid-services-authentication
source_filename: centers-for-medicare-and-medicaid-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/\n    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/\n    scopes: 3\n  description: OAuth 2.0 authorization code flow used by Medicare beneficiaries to grant access\n    to a third-party application.\n  sources:\n  - openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/authentication/centers-for-medicare-and-medicaid-services-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- BCDA
- Blue Button
- CMS
- Claims
- DPC
- FHIR
- Federal Government
- Healthcare
- Interoperability
- Marketplace
- Medicaid
- Medicare
- Open Data
- Provider Data
- Socrata
---
