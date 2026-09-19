---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cloudflare-openapi-original.yml
  format: yaml
  label: Cloudflare API
  slug: cloudflare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/cloudflare-openapi-original.yml
- filename: github-openapi-original.yml
  format: yaml
  label: GitHub REST API
  slug: github
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/github-openapi-original.yml
- filename: postman-openapi-original.yml
  format: yaml
  label: Postman API
  slug: postman
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/postman-openapi-original.yml
- filename: aws-api-gateway-openapi-original.yml
  format: yaml
  label: Amazon API Gateway
  slug: aws-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/aws-api-gateway-openapi-original.yml
- filename: aws-iam-openapi-original.yml
  format: yaml
  label: AWS Identity and Access Management
  slug: aws-iam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/aws-iam-openapi-original.yml
- filename: aws-lambda-openapi-original.yml
  format: yaml
  label: AWS Lambda
  slug: aws-lambda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/aws-lambda-openapi-original.yml
- filename: microsoft-cognitive-news-search-openapi-original.yml
  format: yaml
  label: Bing News Search API
  slug: microsoft-cognitive-news-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/microsoft-cognitive-news-search-openapi-original.yml
- filename: microsoft-cognitive-video-search-openapi-original.yml
  format: yaml
  label: Bing Video Search API
  slug: microsoft-cognitive-video-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/microsoft-cognitive-video-search-openapi-original.yml
- filename: microsoft-cognitive-web-search-openapi-original.yml
  format: yaml
  label: Bing Web Search API
  slug: microsoft-cognitive-web-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/microsoft-cognitive-web-search-openapi-original.yml
- filename: aws-rds-openapi-original.yml
  format: yaml
  label: Amazon Relational Database Service
  slug: aws-rds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/aws-rds-openapi-original.yml
- filename: aws-s3-openapi-original.yml
  format: yaml
  label: Amazon Simple Storage Service
  slug: aws-s3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/aws-s3-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: Engineering Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIs.io Engineering Platform secures its APIs with apiKey and http across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APIs.io Engineering Platform
provider_slug: engineering-platform
scheme_count: 7
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/aws-api-gateway-openapi-original.yml
  - openapi/aws-iam-openapi-original.yml
  - openapi/aws-lambda-openapi-original.yml
  - openapi/postman-openapi-original.yml
  type: apiKey
- in: header
  name: api_email
  parameter: X-Auth-Email
  sources:
  - openapi/cloudflare-openapi-original.yml
  type: apiKey
- in: header
  name: api_key
  parameter: X-Auth-Key
  sources:
  - openapi/cloudflare-openapi-original.yml
  type: apiKey
- name: api_token
  scheme: bearer
  sources:
  - openapi/cloudflare-openapi-original.yml
  type: http
- in: header
  name: user_service_key
  parameter: X-Auth-User-Service-Key
  sources:
  - openapi/cloudflare-openapi-original.yml
  type: apiKey
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/microsoft-cognitive-news-search-openapi-original.yml
  - openapi/microsoft-cognitive-video-search-openapi-original.yml
  - openapi/microsoft-cognitive-web-search-openapi-original.yml
  type: apiKey
- in: header
  name: PostmanApiKey
  parameter: x-api-key
  sources:
  - openapi/postman-openapi-original.yml
  type: apiKey
slug: engineering-platform-authentication
source_filename: engineering-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-api-gateway-openapi-original.yml, openapi/aws-iam-openapi-original.yml,\n  openapi/aws-lambda-openapi-original.yml, openapi/cloudflare-openapi-original.yml, openapi/microsoft-cognitive-news-search-openapi-original.yml,\n  openapi/microsoft-cognitive-video-search-openapi-original.yml, openapi/microsoft-cognitive-web-search-openapi-original.yml,\n  openapi/postman-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/aws-api-gateway-openapi-original.yml\n  - openapi/aws-iam-openapi-original.yml\n  - openapi/aws-lambda-openapi-original.yml\n  - openapi/postman-openapi-original.yml\n- name: api_email\n  type: apiKey\n  in: header\n  parameter: X-Auth-Email\n  sources:\n  - openapi/cloudflare-openapi-original.yml\n- name: api_key\n\
  \  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  sources:\n  - openapi/cloudflare-openapi-original.yml\n- name: api_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cloudflare-openapi-original.yml\n- name: user_service_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-User-Service-Key\n  sources:\n  - openapi/cloudflare-openapi-original.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/microsoft-cognitive-news-search-openapi-original.yml\n  - openapi/microsoft-cognitive-video-search-openapi-original.yml\n  - openapi/microsoft-cognitive-web-search-openapi-original.yml\n- name: PostmanApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/postman-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/authentication/engineering-platform-authentication.yml
summary_line: apiKey/http · 7 schemes
tags:
- APIs.io
- Engineering
- Platform
---
