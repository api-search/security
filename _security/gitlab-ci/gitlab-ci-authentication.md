---
api_key_in:
- header
- query
api_specs:
- filename: gitlab-ci-openapi.yml
  format: yaml
  label: GitLab REST API v4 (CI/CD endpoints)
  slug: rest-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/openapi/gitlab-ci-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gitlab Ci Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitLab CI/CD secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GitLab CI/CD
provider_slug: gitlab-ci
scheme_count: 2
schemes:
- in: header
  name: access_token_header
  parameter: PRIVATE-TOKEN
  sources:
  - openapi/gitlab-ci-openapi.yml
  type: apiKey
- in: query
  name: access_token_query
  parameter: private_token
  sources:
  - openapi/gitlab-ci-openapi.yml
  type: apiKey
slug: gitlab-ci-authentication
source_filename: gitlab-ci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitlab-ci-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: access_token_header\n  type: apiKey\n  in: header\n  parameter: PRIVATE-TOKEN\n  sources:\n  - openapi/gitlab-ci-openapi.yml\n- name: access_token_query\n  type: apiKey\n  in: query\n  parameter: private_token\n  sources:\n  - openapi/gitlab-ci-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/authentication/gitlab-ci-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- DevOps
- CI/CD
- Pipelines
- GitLab
- DevSecOps
- Runners
- Container Registry
---
