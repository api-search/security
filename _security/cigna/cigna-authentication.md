---
api_key_in: []
api_specs:
- filename: cigna-patient-access-api-openapi.yml
  format: yaml
  label: Cigna Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-patient-access-api-openapi.yml
- filename: cigna-provider-directory-api-openapi.yml
  format: yaml
  label: Cigna Provider Directory API
  slug: provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-provider-directory-api-openapi.yml
- filename: cigna-drug-formulary-api-openapi.yml
  format: yaml
  label: Cigna Drug Formulary API
  slug: drug-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-drug-formulary-api-openapi.yml
- filename: cigna-provider-access-api-openapi.yml
  format: yaml
  label: Cigna Provider Access API
  slug: provider-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-provider-access-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cigna Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cigna secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cigna
provider_slug: cigna
scheme_count: 2
schemes:
- description: SMART on FHIR authorization with patient-context launch
  flows:
  - authorizationUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token
  name: smartOnFhir
  sources:
  - openapi/cigna-patient-access-api-openapi.yml
  type: oauth2
- description: SMART Backend Services authorization for bulk FHIR export
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token
  name: bulkData
  sources:
  - openapi/cigna-provider-access-api-openapi.yml
  type: oauth2
slug: cigna-authentication
source_filename: cigna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cigna-patient-access-api-openapi.yml, openapi/cigna-provider-access-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/authorize\n    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token\n    scopes: 5\n  description: SMART on FHIR authorization with patient-context launch\n  sources:\n  - openapi/cigna-patient-access-api-openapi.yml\n- name: bulkData\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token\n    scopes: 1\n  description: SMART Backend Services authorization for bulk FHIR export\n  sources:\n  - openapi/cigna-provider-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/authentication/cigna-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 100
---
