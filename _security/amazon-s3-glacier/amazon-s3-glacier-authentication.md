---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-s3-glacier-vaults-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier Vaults API
  slug: amazon-s3-glacier-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-vaults-api-openapi.yml
- filename: amazon-s3-glacier-access-policy-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Access Policy API
  slug: amazon-s3-glacier-access-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-access-policy-api-openapi.yml
- filename: amazon-s3-glacier-lock-policy-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Lock Policy API
  slug: amazon-s3-glacier-lock-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-lock-policy-api-openapi.yml
- filename: amazon-s3-glacier-multipart-uploads-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Multipart Uploads API
  slug: amazon-s3-glacier-multipart-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-multipart-uploads-api-openapi.yml
- filename: amazon-s3-glacier-notification-configuration-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Notification Configuration API
  slug: amazon-s3-glacier-notification-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-notification-configuration-api-openapi.yml
- filename: amazon-s3-glacier-operations-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Operations API
  slug: amazon-s3-glacier-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-operations-api-openapi.yml
- filename: amazon-s3-glacier-tags-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Tags API
  slug: amazon-s3-glacier-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon S3 Glacier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon S3 Glacier secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-s3-glacier-access-policy-api-openapi.yml
  - openapi/amazon-s3-glacier-lock-policy-api-openapi.yml
  - openapi/amazon-s3-glacier-multipart-uploads-api-openapi.yml
  - openapi/amazon-s3-glacier-notification-configuration-api-openapi.yml
  - openapi/amazon-s3-glacier-operations-api-openapi.yml
  - openapi/amazon-s3-glacier-tags-api-openapi.yml
  - openapi/amazon-s3-glacier-vaults-api-openapi.yml
  type: apiKey
slug: amazon-s3-glacier-authentication
source_filename: amazon-s3-glacier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-s3-glacier-access-policy-api-openapi.yml, openapi/amazon-s3-glacier-lock-policy-api-openapi.yml,\n  openapi/amazon-s3-glacier-multipart-uploads-api-openapi.yml, openapi/amazon-s3-glacier-notification-configuration-api-openapi.yml,\n  openapi/amazon-s3-glacier-operations-api-openapi.yml, openapi/amazon-s3-glacier-tags-api-openapi.yml,\n  openapi/amazon-s3-glacier-vaults-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-s3-glacier-access-policy-api-openapi.yml\n  - openapi/amazon-s3-glacier-lock-policy-api-openapi.yml\n  - openapi/amazon-s3-glacier-multipart-uploads-api-openapi.yml\n\
  \  - openapi/amazon-s3-glacier-notification-configuration-api-openapi.yml\n  - openapi/amazon-s3-glacier-operations-api-openapi.yml\n  - openapi/amazon-s3-glacier-tags-api-openapi.yml\n  - openapi/amazon-s3-glacier-vaults-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-s3-glacier/authentication/amazon-s3-glacier-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Archives
- Amazon Web Services
- Backup
- Storage
---
