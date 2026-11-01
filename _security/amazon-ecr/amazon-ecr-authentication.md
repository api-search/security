---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
  format: yaml
  label: Amazon ECR Amazon ECR Amazon Elastic Container Registry (ECR) API
  slug: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
- filename: amazon-ecr-lifecycle-policy-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Lifecycle Policy API
  slug: amazon-ecr-lifecycle-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-lifecycle-policy-api-openapi.yml
- filename: amazon-ecr-operations-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Operations API
  slug: amazon-ecr-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-operations-api-openapi.yml
- filename: amazon-ecr-pull-through-cache-rule-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Pull Through Cache Rule API
  slug: amazon-ecr-pull-through-cache-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-pull-through-cache-rule-api-openapi.yml
- filename: amazon-ecr-pull-time-update-exclusion-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Pull Time Update Exclusion API
  slug: amazon-ecr-pull-time-update-exclusion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-pull-time-update-exclusion-api-openapi.yml
- filename: amazon-ecr-registry-policy-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Registry Policy API
  slug: amazon-ecr-registry-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-registry-policy-api-openapi.yml
- filename: amazon-ecr-replication-backfill-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Replication Backfill API
  slug: amazon-ecr-replication-backfill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-replication-backfill-api-openapi.yml
- filename: amazon-ecr-repository-creation-template-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Repository Creation Template API
  slug: amazon-ecr-repository-creation-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-repository-creation-template-api-openapi.yml
- filename: amazon-ecr-repository-policy-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Repository Policy API
  slug: amazon-ecr-repository-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-repository-policy-api-openapi.yml
- filename: amazon-ecr-signing-configuration-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Signing Configuration API
  slug: amazon-ecr-signing-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-signing-configuration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Ecr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon ECR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon ECR
provider_slug: amazon-ecr
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-ecr-openapi.yml
  type: apiKey
slug: amazon-ecr-authentication
source_filename: amazon-ecr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ecr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-ecr-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-ecr/authentication/amazon-ecr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Container Images
- Container Registry
- Containers
- Docker
- ECR
- OCI
---
