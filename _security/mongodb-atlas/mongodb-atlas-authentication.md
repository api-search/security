---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: MongoDB Atlas Administration API v2
  slug: administration-api-v2
  spec_type: OpenAPI
  url: https://mongodb-mms-prod-build-server.s3.amazonaws.com/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mongodb Atlas Authentication
name_suffix: Authentication
oauth_flows: []
overview: MongoDB Atlas secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MongoDB Atlas
provider_slug: mongodb-atlas
scheme_count: 2
schemes:
- description: HTTP Digest auth using public/private API key pair.
  name: httpDigest
  scheme: digest
  sources:
  - openapi/mongodb-atlas-openapi.yml
  type: http
- description: OAuth 2.0 bearer access token issued to an Atlas service account.
  name: bearer
  scheme: bearer
  sources:
  - openapi/mongodb-atlas-openapi.yml
  type: http
slug: mongodb-atlas-authentication
source_filename: mongodb-atlas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mongodb-atlas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: httpDigest\n  type: http\n  scheme: digest\n  description: HTTP Digest auth using public/private API key pair.\n  sources:\n  - openapi/mongodb-atlas-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer access token issued to an Atlas service account.\n  sources:\n  - openapi/mongodb-atlas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mongodb-atlas/refs/heads/main/authentication/mongodb-atlas-authentication.yml
summary_line: http · 2 schemes
tags:
- Database
- Document Database
- NoSQL
- MongoDB
- Cloud Database
- DBaaS
- Vector Search
- Atlas
---
