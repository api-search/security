---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Compute Engine API
  slug: compute-engine
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Storage API
  slug: cloud-storage
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Functions API
  slug: cloud-functions
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Pub/Sub API
  slug: cloud-pubsub
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: BigQuery API
  slug: bigquery
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Cloud Vision API
  slug: cloud-vision
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Natural Language API
  slug: cloud-natural-language
  spec_type: OpenAPI
  url: https://language.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Kubernetes Engine API
  slug: kubernetes-engine
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Firestore API
  slug: cloud-firestore
  spec_type: OpenAPI
  url: https://firestore.googleapis.com/$discovery/rest?version=v1
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gcp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Platform APIs secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Platform APIs
provider_slug: gcp
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/gcp-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gcp-openapi.yml
  type: http
slug: gcp-authentication
source_filename: gcp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gcp-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/gcp-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/gcp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/authentication/gcp-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Security
- Serverless
- Storage
---
