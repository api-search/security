---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-codecommit-approval-rule-template-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Approval Rule Template API
  slug: amazon-codecommit-approval-rule-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-approval-rule-template-api-openapi.yml
- filename: amazon-codecommit-branch-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Branch API
  slug: amazon-codecommit-branch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-branch-api-openapi.yml
- filename: amazon-codecommit-comment-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Comment API
  slug: amazon-codecommit-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-comment-api-openapi.yml
- filename: amazon-codecommit-commit-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Commit API
  slug: amazon-codecommit-commit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-commit-api-openapi.yml
- filename: amazon-codecommit-file-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit File API
  slug: amazon-codecommit-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-file-api-openapi.yml
- filename: amazon-codecommit-merge-conflict-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Merge Conflict API
  slug: amazon-codecommit-merge-conflict-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-merge-conflict-api-openapi.yml
- filename: amazon-codecommit-operations-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Operations API
  slug: amazon-codecommit-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-operations-api-openapi.yml
- filename: amazon-codecommit-pull-request-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Pull Request API
  slug: amazon-codecommit-pull-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-pull-request-api-openapi.yml
- filename: amazon-codecommit-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Repository API
  slug: amazon-codecommit-repository-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-repository-api-openapi.yml
- filename: amazon-codecommit-repository-trigger-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Repository Trigger API
  slug: amazon-codecommit-repository-trigger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-repository-trigger-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon CodeCommit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeCommit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeCommit
provider_slug: amazon-codecommit
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-codecommit-approval-rule-template-api-openapi.yml
  - openapi/amazon-codecommit-branch-api-openapi.yml
  - openapi/amazon-codecommit-comment-api-openapi.yml
  - openapi/amazon-codecommit-commit-api-openapi.yml
  - openapi/amazon-codecommit-file-api-openapi.yml
  - openapi/amazon-codecommit-merge-conflict-api-openapi.yml
  - openapi/amazon-codecommit-operations-api-openapi.yml
  - openapi/amazon-codecommit-pull-request-api-openapi.yml
  - openapi/amazon-codecommit-repository-api-openapi.yml
  - openapi/amazon-codecommit-repository-trigger-api-openapi.yml
  type: apiKey
slug: amazon-codecommit-authentication
source_filename: amazon-codecommit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-codecommit-approval-rule-template-api-openapi.yml, openapi/amazon-codecommit-branch-api-openapi.yml,\n  openapi/amazon-codecommit-comment-api-openapi.yml, openapi/amazon-codecommit-commit-api-openapi.yml,\n  openapi/amazon-codecommit-file-api-openapi.yml, openapi/amazon-codecommit-merge-conflict-api-openapi.yml,\n  openapi/amazon-codecommit-operations-api-openapi.yml, openapi/amazon-codecommit-pull-request-api-openapi.yml,\n  openapi/amazon-codecommit-repository-api-openapi.yml, openapi/amazon-codecommit-repository-trigger-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n\
  \  - openapi/amazon-codecommit-approval-rule-template-api-openapi.yml\n  - openapi/amazon-codecommit-branch-api-openapi.yml\n  - openapi/amazon-codecommit-comment-api-openapi.yml\n  - openapi/amazon-codecommit-commit-api-openapi.yml\n  - openapi/amazon-codecommit-file-api-openapi.yml\n  - openapi/amazon-codecommit-merge-conflict-api-openapi.yml\n  - openapi/amazon-codecommit-operations-api-openapi.yml\n  - openapi/amazon-codecommit-pull-request-api-openapi.yml\n  - openapi/amazon-codecommit-repository-api-openapi.yml\n  - openapi/amazon-codecommit-repository-trigger-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-codecommit/authentication/amazon-codecommit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Version Control
- Amazon Web Services
- Cloud
---
