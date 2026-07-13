---
api_key_in:
- header
api_specs:
- filename: scaleway-instance-openapi.yml
  format: yaml
  label: Scaleway Instance API
  slug: scaleway-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-instance-openapi.yml
- filename: scaleway-kubernetes-openapi.yml
  format: yaml
  label: Scaleway Kubernetes API
  slug: scaleway-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-kubernetes-openapi.yml
- filename: scaleway-iam-openapi.yml
  format: yaml
  label: Scaleway IAM API
  slug: scaleway-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-iam-openapi.yml
- filename: scaleway-load-balancer-openapi.yml
  format: yaml
  label: Scaleway Load Balancer API
  slug: scaleway-load-balancer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-load-balancer-openapi.yml
- filename: scaleway-database-openapi.yml
  format: yaml
  label: Scaleway Managed Database API
  slug: scaleway-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-database-openapi.yml
- filename: scaleway-vpc-openapi.yml
  format: yaml
  label: Scaleway VPC API
  slug: scaleway-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-vpc-openapi.yml
- filename: scaleway-serverless-containers-openapi.yml
  format: yaml
  label: Scaleway Serverless Containers API
  slug: scaleway-serverless-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-serverless-containers-openapi.yml
- filename: scaleway-serverless-functions-openapi.yml
  format: yaml
  label: Scaleway Serverless Functions API
  slug: scaleway-serverless-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-serverless-functions-openapi.yml
- filename: scaleway-secret-manager-openapi.yml
  format: yaml
  label: Scaleway Secret Manager API
  slug: scaleway-secret-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-secret-manager-openapi.yml
- filename: scaleway-transactional-email-openapi.yml
  format: yaml
  label: Scaleway Transactional Email API
  slug: scaleway-transactional-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-transactional-email-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scaleway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scaleway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scaleway
provider_slug: scaleway
scheme_count: 1
schemes:
- in: header
  name: scaleway
  parameter: X-Auth-Token
  sources:
  - openapi/scaleway-database-openapi.yml
  - openapi/scaleway-iam-openapi.yml
  - openapi/scaleway-instance-openapi.yml
  - openapi/scaleway-kubernetes-openapi.yml
  - openapi/scaleway-load-balancer-openapi.yml
  - openapi/scaleway-secret-manager-openapi.yml
  - openapi/scaleway-serverless-containers-openapi.yml
  - openapi/scaleway-serverless-functions-openapi.yml
  - openapi/scaleway-transactional-email-openapi.yml
  - openapi/scaleway-vpc-openapi.yml
  type: apiKey
slug: scaleway-authentication
source_filename: scaleway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scaleway-database-openapi.yml, openapi/scaleway-iam-openapi.yml, openapi/scaleway-instance-openapi.yml,\n  openapi/scaleway-kubernetes-openapi.yml, openapi/scaleway-load-balancer-openapi.yml, openapi/scaleway-secret-manager-openapi.yml,\n  openapi/scaleway-serverless-containers-openapi.yml, openapi/scaleway-serverless-functions-openapi.yml,\n  openapi/scaleway-transactional-email-openapi.yml, openapi/scaleway-vpc-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: scaleway\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/scaleway-database-openapi.yml\n  - openapi/scaleway-iam-openapi.yml\n  - openapi/scaleway-instance-openapi.yml\n  - openapi/scaleway-kubernetes-openapi.yml\n  - openapi/scaleway-load-balancer-openapi.yml\n  - openapi/scaleway-secret-manager-openapi.yml\n  - openapi/scaleway-serverless-containers-openapi.yml\n  - openapi/scaleway-serverless-functions-openapi.yml\n\
  \  - openapi/scaleway-transactional-email-openapi.yml\n  - openapi/scaleway-vpc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/authentication/scaleway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Cloud Computing
- Containers
- Database
- European Cloud
- Infrastructure
- Kubernetes
- Serverless
- Storage
---
