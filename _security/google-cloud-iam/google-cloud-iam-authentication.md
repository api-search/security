---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-cloud-iam-folders-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Folders API
  slug: google-cloud-iam-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-folders-api-openapi.yml
- filename: google-cloud-iam-iam-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Iam API
  slug: google-cloud-iam-iam-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-iam-api-openapi.yml
- filename: google-cloud-iam-locations-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Locations API
  slug: google-cloud-iam-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-locations-api-openapi.yml
- filename: google-cloud-iam-operations-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Operations API
  slug: google-cloud-iam-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-operations-api-openapi.yml
- filename: google-cloud-iam-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Organizations API
  slug: google-cloud-iam-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-organizations-api-openapi.yml
- filename: google-cloud-iam-policies-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Policies API
  slug: google-cloud-iam-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-policies-api-openapi.yml
- filename: google-cloud-iam-projects-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Projects API
  slug: google-cloud-iam-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-projects-api-openapi.yml
- filename: google-cloud-iam-token-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Token API
  slug: google-cloud-iam-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-iam/openapi/google-cloud-iam-token-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Cloud IAM Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud IAM secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud IAM
provider_slug: google-cloud-iam
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-cloud-iam-authentication
source_filename: google-cloud-iam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-iam/authentication/google-cloud-iam-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Identity and Access Management
- Google Cloud
- Identity
- Permissions
- Security
---
