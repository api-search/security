---
api_key_in:
- header
api_specs:
- filename: amazon-memorydb-acls-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB ACLs API
  slug: amazon-memorydb-acls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-acls-api-openapi.yml
- filename: amazon-memorydb-clusters-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Clusters API
  slug: amazon-memorydb-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-clusters-api-openapi.yml
- filename: amazon-memorydb-engineversions-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB EngineVersions API
  slug: amazon-memorydb-engineversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-engineversions-api-openapi.yml
- filename: amazon-memorydb-events-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Events API
  slug: amazon-memorydb-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-events-api-openapi.yml
- filename: amazon-memorydb-nodetypes-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB NodeTypes API
  slug: amazon-memorydb-nodetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-nodetypes-api-openapi.yml
- filename: amazon-memorydb-parametergroups-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB ParameterGroups API
  slug: amazon-memorydb-parametergroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-parametergroups-api-openapi.yml
- filename: amazon-memorydb-reservednodes-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB ReservedNodes API
  slug: amazon-memorydb-reservednodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-reservednodes-api-openapi.yml
- filename: amazon-memorydb-shards-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Shards API
  slug: amazon-memorydb-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-shards-api-openapi.yml
- filename: amazon-memorydb-snapshots-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Snapshots API
  slug: amazon-memorydb-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-snapshots-api-openapi.yml
- filename: amazon-memorydb-subnetgroups-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB SubnetGroups API
  slug: amazon-memorydb-subnetgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-subnetgroups-api-openapi.yml
- filename: amazon-memorydb-tags-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Tags API
  slug: amazon-memorydb-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-tags-api-openapi.yml
- filename: amazon-memorydb-users-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Users API
  slug: amazon-memorydb-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Memorydb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MemoryDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: awsSigV4
  parameter: Authorization
  sources:
  - openapi/amazon-memorydb-openapi-original.yml
  type: apiKey
slug: amazon-memorydb-authentication
source_filename: amazon-memorydb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-memorydb-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-memorydb-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/authentication/amazon-memorydb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
