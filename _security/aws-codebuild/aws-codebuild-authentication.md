---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aws-codebuild-aws-codebuild-api-api-openapi.yml
  format: yaml
  label: AWS CodeBuild AWS CodeBuild API
  slug: aws-codebuild-aws-codebuild-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-api-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-deletereport-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.DeleteReport… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-deletereport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-deletereport-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listbuilds-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.ListBuilds… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listbuilds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listbuilds-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listprojects-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.ListProjects… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listprojects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listprojects-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listreports-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.ListReports… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listreports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-listreports-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-retrybuild-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.RetryBuild… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-retrybuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-retrybuild-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-startbuild-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.StartBuild… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-startbuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-startbuild-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-stopbuild-api-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild 20161006.StopBuild API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-stopbuild-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-20161006-stopbuild-api-api-openapi.yml
- filename: aws-codebuild-aws-codebuild-x-amz-target-codebuild-api-openapi.yml
  format: yaml
  label: 'AWS CodeBuild AWS CodeBuild #X Amz Target=CodeBuild… API'
  slug: aws-codebuild-aws-codebuild-x-amz-target-codebuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-aws-codebuild-x-amz-target-codebuild-api-openapi.yml
- filename: aws-codebuild-builds-api-openapi.yml
  format: yaml
  label: AWS CodeBuild Builds API
  slug: aws-codebuild-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-builds-api-openapi.yml
- filename: aws-codebuild-projects-api-openapi.yml
  format: yaml
  label: AWS CodeBuild Projects API
  slug: aws-codebuild-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/openapi/aws-codebuild-projects-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Aws Codebuild Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS CodeBuild secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS CodeBuild
provider_slug: aws-codebuild
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-codebuild-openapi.yml
  type: apiKey
slug: aws-codebuild-authentication
source_filename: aws-codebuild-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-codebuild-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-codebuild-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-codebuild/refs/heads/main/authentication/aws-codebuild-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Builds
- CI/CD
- Continuous Integration
- Developer Tools
- DevOps
---
