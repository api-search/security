---
api_key_in:
- query
api_specs:
- filename: google-cloud-platform-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Folders API
  slug: google-cloud-platform-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-folders-api-openapi.yml
- filename: google-cloud-platform-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Operations API
  slug: google-cloud-platform-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-operations-api-openapi.yml
- filename: google-cloud-platform-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Organizations API
  slug: google-cloud-platform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-organizations-api-openapi.yml
- filename: google-cloud-platform-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Projects API
  slug: google-cloud-platform-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-projects-api-openapi.yml
- filename: google-cloud-platform-tagbindings-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagBindings API
  slug: google-cloud-platform-tagbindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagbindings-api-openapi.yml
- filename: google-cloud-platform-tagkeys-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagKeys API
  slug: google-cloud-platform-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagkeys-api-openapi.yml
- filename: google-cloud-platform-tagvalues-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagValues API
  slug: google-cloud-platform-tagvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagvalues-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Cloud Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Platform secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication using Google Cloud service accounts or user credentials. Supports both service-to-service and end-user authentication flows.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/cloud-resource-manager-openapi.yml
  type: oauth2
- description: API key for identifying the calling project.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/cloud-resource-manager-openapi.yml
  type: apiKey
slug: google-cloud-platform-authentication
source_filename: google-cloud-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/cloud-resource-manager-openapi.yml\ndocs: https://cloud.google.com/docs/authentication\noidc_discovery: well-known/google-cloud-platform-openid-configuration.json\nnotes: >-\n  Google Cloud authenticates with OAuth 2.0 access tokens minted for either an\n  end user (3-legged) or a service account (2-legged, via signed JWT or\n  Application Default Credentials / Workload Identity Federation). The optional\n  API key (query `key`) only identifies the calling project and does not grant\n  authorization. OIDC discovery confirmed live at accounts.google.com (200).\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  description: OAuth 2.0 authentication\
  \ using Google Cloud service accounts or user credentials.\n    Supports both service-to-service and end-user authentication flows.\n  sources:\n  - openapi/cloud-resource-manager-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key for identifying the calling project.\n  sources:\n  - openapi/cloud-resource-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/authentication/google-cloud-platform-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
---
