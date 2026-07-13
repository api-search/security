---
api_key_in: []
api_specs:
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Clients API
  slug: provet-cloud-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Patients API
  slug: provet-cloud-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Appointments API
  slug: provet-cloud-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Consultations API
  slug: provet-cloud-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Billing & Invoicing API
  slug: provet-cloud-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Items & Reference Data API
  slug: provet-cloud-items-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Webhooks API
  slug: provet-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Provet Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Provet Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Provet Cloud
provider_slug: provet-cloud
scheme_count: 1
schemes:
- description: OAuth 2.0. Client Credentials for backend services; Authorization Code with PKCE for user-facing apps. Token endpoint is https://provetcloud.com/<provet_id>/oauth2/token/ with scope "restapi".
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://provetcloud.com/0/oauth2/token/
  - authorizationUrl: https://provetcloud.com/0/oauth2/authorize/
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://provetcloud.com/0/oauth2/token/
  name: oauth2
  sources:
  - openapi/provet-cloud-openapi.yml
  type: oauth2
slug: provet-cloud-authentication
source_filename: provet-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/provet-cloud-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://provetcloud.com/0/oauth2/token/\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://provetcloud.com/0/oauth2/authorize/\n    tokenUrl: https://provetcloud.com/0/oauth2/token/\n    scopes: 2\n  description: OAuth 2.0. Client Credentials for backend services; Authorization Code with PKCE\n    for user-facing apps. Token endpoint is https://provetcloud.com/<provet_id>/oauth2/token/\n    with scope \"restapi\".\n  sources:\n  - openapi/provet-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/authentication/provet-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- Nordhealth
- Animal Health
- Appointments
- Billing
---
