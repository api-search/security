---
api_key_in: []
api_specs:
- filename: gcp-disks-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Disks API
  slug: gcp-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-disks-api-openapi.yml
- filename: gcp-firewalls-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Firewalls API
  slug: gcp-firewalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-firewalls-api-openapi.yml
- filename: gcp-images-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Images API
  slug: gcp-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-images-api-openapi.yml
- filename: gcp-instances-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Instances API
  slug: gcp-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-instances-api-openapi.yml
- filename: gcp-machinetypes-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs MachineTypes API
  slug: gcp-machinetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-machinetypes-api-openapi.yml
- filename: gcp-networks-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Networks API
  slug: gcp-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-networks-api-openapi.yml
- filename: gcp-snapshots-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Snapshots API
  slug: gcp-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-snapshots-api-openapi.yml
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
- Machine-Learning
- Networking
- Security
- Serverless
- Storage
---
