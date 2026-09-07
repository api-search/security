---
anonymous_access: false
api_key_in: []
api_specs:
- filename: delta-lake-delta-sharing-protocol-openapi.yml
  format: yaml
  label: Delta Sharing Protocol
  slug: delta-sharing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-lake/refs/heads/main/openapi/delta-lake-delta-sharing-protocol-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Delta Lake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delta Lake secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Delta Lake
provider_slug: delta-lake
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/delta-lake-delta-sharing-protocol-openapi.yml
  type: http
slug: delta-lake-authentication
source_filename: delta-lake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/delta-lake-delta-sharing-protocol-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/delta-lake-delta-sharing-protocol-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-lake/refs/heads/main/authentication/delta-lake-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Data Lake
- Lakehouse
- Linux Foundation
- Open-Source
- Storage
- Streaming
---
