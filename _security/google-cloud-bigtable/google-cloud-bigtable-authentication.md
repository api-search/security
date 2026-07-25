---
api_key_in: []
api_specs:
- filename: google-cloud-bigtable-clusters-api-openapi.yml
  format: yaml
  label: Google Cloud Bigtable Clusters API
  slug: google-cloud-bigtable-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/openapi/google-cloud-bigtable-clusters-api-openapi.yml
- filename: google-cloud-bigtable-instances-api-openapi.yml
  format: yaml
  label: Google Cloud Bigtable Instances API
  slug: google-cloud-bigtable-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/openapi/google-cloud-bigtable-instances-api-openapi.yml
- filename: google-cloud-bigtable-tables-api-openapi.yml
  format: yaml
  label: Google Cloud Bigtable Tables API
  slug: google-cloud-bigtable-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/openapi/google-cloud-bigtable-tables-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Bigtable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Bigtable secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Bigtable
provider_slug: google-cloud-bigtable
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/cloud-bigtable-openapi.yml
  type: oauth2
slug: google-cloud-bigtable-authentication
source_filename: google-cloud-bigtable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-bigtable-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/cloud-bigtable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/authentication/google-cloud-bigtable-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Bigtable
- Database
- Google Cloud
- NoSQL
- Wide Column
---
