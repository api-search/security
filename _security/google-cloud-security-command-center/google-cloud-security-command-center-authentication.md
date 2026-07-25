---
api_key_in: []
api_specs:
- filename: google-cloud-security-command-center-assets-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center Assets API
  slug: google-cloud-security-command-center-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-security-command-center/refs/heads/main/openapi/google-cloud-security-command-center-assets-api-openapi.yml
- filename: google-cloud-security-command-center-findings-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center Findings API
  slug: google-cloud-security-command-center-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-security-command-center/refs/heads/main/openapi/google-cloud-security-command-center-findings-api-openapi.yml
- filename: google-cloud-security-command-center-notificationconfigs-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center NotificationConfigs API
  slug: google-cloud-security-command-center-notificationconfigs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-security-command-center/refs/heads/main/openapi/google-cloud-security-command-center-notificationconfigs-api-openapi.yml
- filename: google-cloud-security-command-center-sources-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center Sources API
  slug: google-cloud-security-command-center-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-security-command-center/refs/heads/main/openapi/google-cloud-security-command-center-sources-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Security Command Center Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Security Command Center secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Security Command Center
provider_slug: google-cloud-security-command-center
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/security-command-center-api-openapi.yml
  type: oauth2
slug: google-cloud-security-command-center-authentication
source_filename: google-cloud-security-command-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/security-command-center-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/security-command-center-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-security-command-center/refs/heads/main/authentication/google-cloud-security-command-center-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Security
- Compliance
- Risk Management
- Security
- Threat Detection
- Vulnerability Management
---
