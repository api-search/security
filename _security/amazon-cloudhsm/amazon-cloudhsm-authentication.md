---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloudhsm-hapg-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Hapg API
  slug: amazon-cloudhsm-hapg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-hapg-api-openapi.yml
- filename: amazon-cloudhsm-hsm-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Hsm API
  slug: amazon-cloudhsm-hsm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-hsm-api-openapi.yml
- filename: amazon-cloudhsm-luna-client-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Luna Client API
  slug: amazon-cloudhsm-luna-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-luna-client-api-openapi.yml
- filename: amazon-cloudhsm-operations-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Operations API
  slug: amazon-cloudhsm-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-operations-api-openapi.yml
- filename: amazon-cloudhsm-tag-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Tag API
  slug: amazon-cloudhsm-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-tag-api-openapi.yml
- filename: amazon-cloudhsm-backup-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Backup API
  slug: amazon-cloudhsm-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-backup-api-openapi.yml
- filename: amazon-cloudhsm-cluster-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Cluster API
  slug: amazon-cloudhsm-cluster-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-cluster-api-openapi.yml
- filename: amazon-cloudhsm-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Resource Policy API
  slug: amazon-cloudhsm-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-resource-policy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon CloudHSM Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudHSM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudHSM
provider_slug: amazon-cloudhsm
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-cloudhsm-backup-api-openapi.yml
  - openapi/amazon-cloudhsm-cluster-api-openapi.yml
  - openapi/amazon-cloudhsm-hapg-api-openapi.yml
  - openapi/amazon-cloudhsm-hsm-api-openapi.yml
  - openapi/amazon-cloudhsm-luna-client-api-openapi.yml
  - openapi/amazon-cloudhsm-operations-api-openapi.yml
  - openapi/amazon-cloudhsm-resource-policy-api-openapi.yml
  - openapi/amazon-cloudhsm-tag-api-openapi.yml
  type: apiKey
slug: amazon-cloudhsm-authentication
source_filename: amazon-cloudhsm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-cloudhsm-backup-api-openapi.yml, openapi/amazon-cloudhsm-cluster-api-openapi.yml,\n  openapi/amazon-cloudhsm-hapg-api-openapi.yml, openapi/amazon-cloudhsm-hsm-api-openapi.yml,\n  openapi/amazon-cloudhsm-luna-client-api-openapi.yml, openapi/amazon-cloudhsm-operations-api-openapi.yml,\n  openapi/amazon-cloudhsm-resource-policy-api-openapi.yml, openapi/amazon-cloudhsm-tag-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-cloudhsm-backup-api-openapi.yml\n  - openapi/amazon-cloudhsm-cluster-api-openapi.yml\n  - openapi/amazon-cloudhsm-hapg-api-openapi.yml\n\
  \  - openapi/amazon-cloudhsm-hsm-api-openapi.yml\n  - openapi/amazon-cloudhsm-luna-client-api-openapi.yml\n  - openapi/amazon-cloudhsm-operations-api-openapi.yml\n  - openapi/amazon-cloudhsm-resource-policy-api-openapi.yml\n  - openapi/amazon-cloudhsm-tag-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloudhsm/authentication/amazon-cloudhsm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- CloudHSM
- Security
- Cryptography
- HSM
- Compliance
---
