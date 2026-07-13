---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Google Compute Engine API
  slug: google-compute-engine-api
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Storage API
  slug: google-cloud-storage-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Kubernetes Engine API
  slug: google-kubernetes-engine-api
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Functions API
  slug: google-cloud-functions-api
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google BigQuery API
  slug: google-bigquery-api
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Google Cloud Pub/Sub API
  slug: google-cloud-pubsub-api
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Vision API
  slug: google-cloud-vision-api
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud SQL Admin API
  slug: google-cloud-sql-admin-api
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Platform secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Platform
provider_slug: google-cloud
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-cloud-openapi.yml
  type: oauth2
slug: google-cloud-authentication
source_filename: google-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/google-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud/refs/heads/main/authentication/google-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Computing
- Data Analytics
- Infrastructure
- Machine Learning
- Platform as a Service
---
