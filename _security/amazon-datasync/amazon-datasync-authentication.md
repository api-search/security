---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-datasync-amazon-datasync-rest-api-api-openapi.yml
  format: yaml
  label: Amazon DataSync Amazon DataSync REST API
  slug: amazon-datasync-amazon-datasync-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-amazon-datasync-rest-api-api-openapi.yml
- filename: amazon-datasync-agent-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Agent API
  slug: amazon-datasync-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-agent-api-openapi.yml
- filename: amazon-datasync-location-azure-blob-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Azure Blob API
  slug: amazon-datasync-location-azure-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-azure-blob-api-openapi.yml
- filename: amazon-datasync-location-ef-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Ef API
  slug: amazon-datasync-location-ef-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-ef-api-openapi.yml
- filename: amazon-datasync-location-fsx-lustre-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Lustre API
  slug: amazon-datasync-location-fsx-lustre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-lustre-api-openapi.yml
- filename: amazon-datasync-location-fsx-ontap-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Ontap API
  slug: amazon-datasync-location-fsx-ontap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-ontap-api-openapi.yml
- filename: amazon-datasync-location-fsx-open-zf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Open Zf API
  slug: amazon-datasync-location-fsx-open-zf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-open-zf-api-openapi.yml
- filename: amazon-datasync-location-fsx-window-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Window API
  slug: amazon-datasync-location-fsx-window-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-window-api-openapi.yml
- filename: amazon-datasync-location-hdf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Hdf API
  slug: amazon-datasync-location-hdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-hdf-api-openapi.yml
- filename: amazon-datasync-location-nf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Nf API
  slug: amazon-datasync-location-nf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-nf-api-openapi.yml
- filename: amazon-datasync-location-object-storage-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Object Storage API
  slug: amazon-datasync-location-object-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-object-storage-api-openapi.yml
- filename: amazon-datasync-location-smb-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Smb API
  slug: amazon-datasync-location-smb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-smb-api-openapi.yml
- filename: amazon-datasync-operations-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Operations API
  slug: amazon-datasync-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-operations-api-openapi.yml
- filename: amazon-datasync-task-execution-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Task Execution API
  slug: amazon-datasync-task-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-task-execution-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Datasync Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DataSync secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DataSync
provider_slug: amazon-datasync
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-datasync-api-openapi.yml
  type: apiKey
slug: amazon-datasync-authentication
source_filename: amazon-datasync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-datasync-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-datasync-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-datasync/authentication/amazon-datasync-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
---
