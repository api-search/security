---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-fsx-filesystems-api-openapi.yml
  format: yaml
  label: Amazon FSx Filesystems API
  slug: amazon-fsx-filesystems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-filesystems-api-openapi.yml
- filename: amazon-fsx-backup-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Backup API
  slug: amazon-fsx-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-backup-api-openapi.yml
- filename: amazon-fsx-data-repository-association-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Data Repository Association API
  slug: amazon-fsx-data-repository-association-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-data-repository-association-api-openapi.yml
- filename: amazon-fsx-data-repository-task-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Data Repository Task API
  slug: amazon-fsx-data-repository-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-data-repository-task-api-openapi.yml
- filename: amazon-fsx-file-cache-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx File Cache API
  slug: amazon-fsx-file-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-file-cache-api-openapi.yml
- filename: amazon-fsx-file-system-aliase-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx File System Aliase API
  slug: amazon-fsx-file-system-aliase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-file-system-aliase-api-openapi.yml
- filename: amazon-fsx-operations-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Operations API
  slug: amazon-fsx-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-operations-api-openapi.yml
- filename: amazon-fsx-snapshot-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Snapshot API
  slug: amazon-fsx-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-snapshot-api-openapi.yml
- filename: amazon-fsx-storage-virtual-machine-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Storage Virtual Machine API
  slug: amazon-fsx-storage-virtual-machine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-storage-virtual-machine-api-openapi.yml
- filename: amazon-fsx-volume-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Volume API
  slug: amazon-fsx-volume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-volume-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon FSx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon FSx secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon FSx
provider_slug: amazon-fsx
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-fsx-backup-api-openapi.yml
  - openapi/amazon-fsx-data-repository-association-api-openapi.yml
  - openapi/amazon-fsx-data-repository-task-api-openapi.yml
  - openapi/amazon-fsx-file-cache-api-openapi.yml
  - openapi/amazon-fsx-file-system-aliase-api-openapi.yml
  - openapi/amazon-fsx-filesystems-api-openapi.yml
  - openapi/amazon-fsx-operations-api-openapi.yml
  - openapi/amazon-fsx-snapshot-api-openapi.yml
  - openapi/amazon-fsx-storage-virtual-machine-api-openapi.yml
  - openapi/amazon-fsx-volume-api-openapi.yml
  type: apiKey
slug: amazon-fsx-authentication
source_filename: amazon-fsx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-fsx-backup-api-openapi.yml, openapi/amazon-fsx-data-repository-association-api-openapi.yml,\n  openapi/amazon-fsx-data-repository-task-api-openapi.yml, openapi/amazon-fsx-file-cache-api-openapi.yml,\n  openapi/amazon-fsx-file-system-aliase-api-openapi.yml, openapi/amazon-fsx-filesystems-api-openapi.yml,\n  openapi/amazon-fsx-operations-api-openapi.yml, openapi/amazon-fsx-snapshot-api-openapi.yml,\n  openapi/amazon-fsx-storage-virtual-machine-api-openapi.yml, openapi/amazon-fsx-volume-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-fsx-backup-api-openapi.yml\n\
  \  - openapi/amazon-fsx-data-repository-association-api-openapi.yml\n  - openapi/amazon-fsx-data-repository-task-api-openapi.yml\n  - openapi/amazon-fsx-file-cache-api-openapi.yml\n  - openapi/amazon-fsx-file-system-aliase-api-openapi.yml\n  - openapi/amazon-fsx-filesystems-api-openapi.yml\n  - openapi/amazon-fsx-operations-api-openapi.yml\n  - openapi/amazon-fsx-snapshot-api-openapi.yml\n  - openapi/amazon-fsx-storage-virtual-machine-api-openapi.yml\n  - openapi/amazon-fsx-volume-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-fsx/authentication/amazon-fsx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Filesystem
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
---
