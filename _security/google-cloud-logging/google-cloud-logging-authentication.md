---
api_key_in: []
api_specs:
- filename: google-cloud-logging-bucket-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Bucket API
  slug: google-cloud-logging-bucket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-bucket-api-openapi.yml
- filename: google-cloud-logging-buckets-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Buckets API
  slug: google-cloud-logging-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-buckets-api-openapi.yml
- filename: google-cloud-logging-entries-copy-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:copy API
  slug: google-cloud-logging-entries-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-copy-api-openapi.yml
- filename: google-cloud-logging-entries-list-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:list API
  slug: google-cloud-logging-entries-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-list-api-openapi.yml
- filename: google-cloud-logging-entries-tail-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:tail API
  slug: google-cloud-logging-entries-tail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-tail-api-openapi.yml
- filename: google-cloud-logging-entries-write-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:write API
  slug: google-cloud-logging-entries-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-write-api-openapi.yml
- filename: google-cloud-logging-exclusions-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Exclusions API
  slug: google-cloud-logging-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-exclusions-api-openapi.yml
- filename: google-cloud-logging-google-cloud-logging-api-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Google Cloud Logging API API
  slug: google-cloud-logging-google-cloud-logging-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-google-cloud-logging-api-api-openapi.yml
- filename: google-cloud-logging-sinks-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Sinks API
  slug: google-cloud-logging-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-sinks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Logging Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Logging secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Logging
provider_slug: google-cloud-logging
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-cloud-logging-openapi.yml
  type: oauth2
slug: google-cloud-logging-authentication
source_filename: google-cloud-logging-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-logging-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 4\n  sources:\n  - openapi/google-cloud-logging-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/authentication/google-cloud-logging-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud
- Logging
- Monitoring
- Observability
---
