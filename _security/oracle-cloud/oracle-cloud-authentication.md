---
api_key_in: []
api_specs:
- filename: oracle-cloud-compute-openapi.yaml
  format: yaml
  label: Compute API
  slug: compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-compute-openapi.yaml
- filename: oracle-cloud-object-storage-openapi.yaml
  format: yaml
  label: Object Storage API
  slug: object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-object-storage-openapi.yaml
- filename: oracle-cloud-networking-openapi.yaml
  format: yaml
  label: Networking API
  slug: networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-networking-openapi.yaml
- filename: oracle-cloud-database-openapi.yaml
  format: yaml
  label: Database API
  slug: database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-database-openapi.yaml
- filename: oracle-cloud-iam-openapi.yaml
  format: yaml
  label: Identity and Access Management API
  slug: identity-and-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-iam-openapi.yaml
- filename: oracle-cloud-oke-openapi.yaml
  format: yaml
  label: Container Engine for Kubernetes API
  slug: container-engine-for-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-oke-openapi.yaml
- filename: oracle-cloud-functions-openapi.yaml
  format: yaml
  label: Functions API
  slug: functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-functions-openapi.yaml
- filename: oracle-cloud-monitoring-openapi.yaml
  format: yaml
  label: Monitoring API
  slug: monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-monitoring-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Cloud Infrastructure secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
scheme_count: 1
schemes:
- description: OCI request signature authentication using API signing keys.
  name: ociSignature
  scheme: bearer
  sources:
  - openapi/oracle-cloud-compute-openapi.yaml
  - openapi/oracle-cloud-database-openapi.yaml
  - openapi/oracle-cloud-functions-openapi.yaml
  - openapi/oracle-cloud-iam-openapi.yaml
  - openapi/oracle-cloud-monitoring-openapi.yaml
  - openapi/oracle-cloud-networking-openapi.yaml
  - openapi/oracle-cloud-object-storage-openapi.yaml
  - openapi/oracle-cloud-oke-openapi.yaml
  type: http
slug: oracle-cloud-authentication
source_filename: oracle-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-cloud-compute-openapi.yaml, openapi/oracle-cloud-database-openapi.yaml,\n  openapi/oracle-cloud-functions-openapi.yaml, openapi/oracle-cloud-iam-openapi.yaml, openapi/oracle-cloud-monitoring-openapi.yaml,\n  openapi/oracle-cloud-networking-openapi.yaml, openapi/oracle-cloud-object-storage-openapi.yaml,\n  openapi/oracle-cloud-oke-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: ociSignature\n  type: http\n  scheme: bearer\n  description: OCI request signature authentication using API signing keys.\n  sources:\n  - openapi/oracle-cloud-compute-openapi.yaml\n  - openapi/oracle-cloud-database-openapi.yaml\n  - openapi/oracle-cloud-functions-openapi.yaml\n  - openapi/oracle-cloud-iam-openapi.yaml\n  - openapi/oracle-cloud-monitoring-openapi.yaml\n  - openapi/oracle-cloud-networking-openapi.yaml\n  - openapi/oracle-cloud-object-storage-openapi.yaml\n  - openapi/oracle-cloud-oke-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/authentication/oracle-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
---
