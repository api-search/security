---
api_key_in: []
api_specs:
- filename: cognito-forms-openapi.yml
  format: yaml
  label: Cognito Forms REST API
  slug: cognito-forms-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognito-forms/refs/heads/main/openapi/cognito-forms-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cognito Forms Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cognito Forms secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cognito Forms
provider_slug: cognito-forms
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://cognitoforms.com/api-connection
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://cognitoforms.com/admin/oauthtoken
  name: oauth2Auth
  sources:
  - openapi/cognito-forms-openapi.yml
  type: oauth2
slug: cognito-forms-authentication
source_filename: cognito-forms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognito-forms-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cognitoforms.com/api-connection\n    tokenUrl: https://cognitoforms.com/admin/oauthtoken\n    scopes: 1\n  sources:\n  - openapi/cognito-forms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognito-forms/refs/heads/main/authentication/cognito-forms-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Forms
- Form Builder
- Form Entries
- Workflow Automation
- Data Collection
- OData
---
