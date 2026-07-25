---
api_key_in: []
api_specs:
- filename: gcp-cloud-storage-bucketaccesscontrols-api-openapi.yml
  format: yaml
  label: Google Cloud Storage BucketAccessControls API
  slug: gcp-cloud-storage-bucketaccesscontrols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/openapi/gcp-cloud-storage-bucketaccesscontrols-api-openapi.yml
- filename: gcp-cloud-storage-buckets-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Buckets API
  slug: gcp-cloud-storage-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/openapi/gcp-cloud-storage-buckets-api-openapi.yml
- filename: gcp-cloud-storage-defaultobjectaccesscontrols-api-openapi.yml
  format: yaml
  label: Google Cloud Storage DefaultObjectAccessControls API
  slug: gcp-cloud-storage-defaultobjectaccesscontrols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/openapi/gcp-cloud-storage-defaultobjectaccesscontrols-api-openapi.yml
- filename: gcp-cloud-storage-objectaccesscontrols-api-openapi.yml
  format: yaml
  label: Google Cloud Storage ObjectAccessControls API
  slug: gcp-cloud-storage-objectaccesscontrols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/openapi/gcp-cloud-storage-objectaccesscontrols-api-openapi.yml
- filename: gcp-cloud-storage-objects-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Objects API
  slug: gcp-cloud-storage-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/openapi/gcp-cloud-storage-objects-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gcp Cloud Storage Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Storage secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication for Google Cloud APIs
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/gcp-cloud-storage-json-api-openapi.yml
  type: oauth2
- description: Bearer token authentication using a Google Cloud access token obtained via service account or user credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gcp-cloud-storage-json-api-openapi.yml
  type: http
slug: gcp-cloud-storage-authentication
source_filename: gcp-cloud-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gcp-cloud-storage-json-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 5\n  description: OAuth 2.0 authentication for Google Cloud APIs\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a Google Cloud access token obtained via service\n    account or user credentials.\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/authentication/gcp-cloud-storage-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
---
