---
api_key_in: []
api_specs:
- filename: google-cloud-iam-permissions-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Permissions API
  slug: google-cloud-iam-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/openapi/google-cloud-iam-permissions-api-openapi.yml
- filename: google-cloud-iam-roles-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Roles API
  slug: google-cloud-iam-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/openapi/google-cloud-iam-roles-api-openapi.yml
- filename: google-cloud-iam-service-account-keys-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Service Account Keys API
  slug: google-cloud-iam-service-account-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/openapi/google-cloud-iam-service-account-keys-api-openapi.yml
- filename: google-cloud-iam-service-accounts-api-openapi.yml
  format: yaml
  label: Google Cloud IAM Service Accounts API
  slug: google-cloud-iam-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/openapi/google-cloud-iam-service-accounts-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Iam Authentication
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/authentication/google-cloud-iam-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Access Management
- Google Cloud
- IAM
- Identity
- Permissions
- Security
---
