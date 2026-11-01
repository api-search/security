---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: anpheros-com-access-requests-api-openapi.yml
  format: yaml
  label: anpheros-com Access requests API
  slug: anpheros-com-access-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-access-requests-api-openapi.yml
- filename: anpheros-com-admin-api-openapi.yml
  format: yaml
  label: anpheros-com Admin API
  slug: anpheros-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-admin-api-openapi.yml
- filename: anpheros-com-anpheros-search-api-openapi.yml
  format: yaml
  label: anpheros-com Anpheros Search API
  slug: anpheros-com-anpheros-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-anpheros-search-api-openapi.yml
- filename: anpheros-com-fhir-r4-api-openapi.yml
  format: yaml
  label: anpheros-com FHIR R4 API
  slug: anpheros-com-fhir-r4-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-fhir-r4-api-openapi.yml
- filename: anpheros-com-icd-10-to-icd-11-api-openapi.yml
  format: yaml
  label: anpheros-com ICD-10 to ICD-11 API
  slug: anpheros-com-icd-10-to-icd-11-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-icd-10-to-icd-11-api-openapi.yml
- filename: anpheros-com-oauth-api-openapi.yml
  format: yaml
  label: anpheros-com OAuth API
  slug: anpheros-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-oauth-api-openapi.yml
- filename: anpheros-com-patient-me-api-openapi.yml
  format: yaml
  label: anpheros-com Patient (me) API
  slug: anpheros-com-patient-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-patient-me-api-openapi.yml
- filename: anpheros-com-rest-v1-api-openapi.yml
  format: yaml
  label: anpheros-com REST v1 API
  slug: anpheros-com-rest-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-rest-v1-api-openapi.yml
- filename: anpheros-com-smart-health-links-api-openapi.yml
  format: yaml
  label: anpheros-com SMART Health Links API
  slug: anpheros-com-smart-health-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-smart-health-links-api-openapi.yml
- filename: anpheros-com-webhooks-api-openapi.yml
  format: yaml
  label: anpheros-com Webhooks API
  slug: anpheros-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Anpheros Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: anpheros-com secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: anpheros-com
provider_slug: anpheros-com
scheme_count: 3
schemes:
- description: A project API key (`sk_test_…` sandbox, `sk_live_…` production) or an OAuth access token (`at_…`).
  name: bearer
  scheme: bearer
  sources:
  - openapi/anpheros-com-openapi.json
  type: http
- description: The same project API key, as a header.
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/anpheros-com-openapi.json
  type: apiKey
- description: SMART on FHIR v2 scopes; authorization code with PKCE for a person's record, client_credentials for a project.
  flows:
  - authorizationUrl: https://platform.anpheros.com/oauth/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://platform.anpheros.com/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://platform.anpheros.com/oauth/token
  name: oauth2
  sources:
  - openapi/anpheros-com-openapi.json
  type: oauth2
slug: anpheros-com-authentication
source_filename: anpheros-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/anpheros-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A project API key (`sk_test_…` sandbox, `sk_live_…` production) or an OAuth access\n    token (`at_…`).\n  sources:\n  - openapi/anpheros-com-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: The same project API key, as a header.\n  sources:\n  - openapi/anpheros-com-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.anpheros.com/oauth/authorize\n    tokenUrl: https://platform.anpheros.com/oauth/token\n    scopes: 11\n  - flow: clientCredentials\n    tokenUrl: https://platform.anpheros.com/oauth/token\n    scopes: 0\n  description: SMART on FHIR v2 scopes;\
  \ authorization code with PKCE for a person's record,\n    client_credentials for a project.\n  sources:\n  - openapi/anpheros-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/anpheros-com/authentication/anpheros-com-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Health
- Digital-Health
- FHIR
- Medical-Records
- API
---
