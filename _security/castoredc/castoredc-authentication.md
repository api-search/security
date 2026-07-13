---
api_key_in: []
api_specs:
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Studies API
  slug: castoredc-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Participants (Records) API
  slug: castoredc-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Institutes API
  slug: castoredc-institutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Users API
  slug: castoredc-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Fields API
  slug: castoredc-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Study Data Points API
  slug: castoredc-study-data-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Reports (Repeating Data) API
  slug: castoredc-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Surveys API
  slug: castoredc-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Audit Trail API
  slug: castoredc-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Data Export API
  slug: castoredc-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Castoredc Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Castor secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Castor
provider_slug: castoredc
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://data.castoredc.com/api/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/castoredc-openapi.yml
  type: oauth2
slug: castoredc-authentication
source_filename: castoredc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/castoredc-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://data.castoredc.com/api/oauth/token\n    scopes: 0\n  sources:\n  - openapi/castoredc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/authentication/castoredc-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- Healthcare
- Life Sciences
- Research
---
