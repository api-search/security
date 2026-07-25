---
api_key_in:
- header
api_specs:
- filename: amazon-appsync-api-keys-api-openapi.yml
  format: yaml
  label: Amazon AppSync Api Keys API
  slug: amazon-appsync-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-api-keys-api-openapi.yml
- filename: amazon-appsync-data-sources-api-openapi.yml
  format: yaml
  label: Amazon AppSync Data Sources API
  slug: amazon-appsync-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-data-sources-api-openapi.yml
- filename: amazon-appsync-domain-names-api-openapi.yml
  format: yaml
  label: Amazon AppSync Domain Names API
  slug: amazon-appsync-domain-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-domain-names-api-openapi.yml
- filename: amazon-appsync-functions-api-openapi.yml
  format: yaml
  label: Amazon AppSync Functions API
  slug: amazon-appsync-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-functions-api-openapi.yml
- filename: amazon-appsync-graphql-apis-api-openapi.yml
  format: yaml
  label: Amazon AppSync GraphQL APIs API
  slug: amazon-appsync-graphql-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-graphql-apis-api-openapi.yml
- filename: amazon-appsync-resolvers-api-openapi.yml
  format: yaml
  label: Amazon AppSync Resolvers API
  slug: amazon-appsync-resolvers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-resolvers-api-openapi.yml
- filename: amazon-appsync-schema-api-openapi.yml
  format: yaml
  label: Amazon AppSync Schema API
  slug: amazon-appsync-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-schema-api-openapi.yml
- filename: amazon-appsync-tags-api-openapi.yml
  format: yaml
  label: Amazon AppSync Tags API
  slug: amazon-appsync-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-tags-api-openapi.yml
- filename: amazon-appsync-types-api-openapi.yml
  format: yaml
  label: Amazon AppSync Types API
  slug: amazon-appsync-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/openapi/amazon-appsync-types-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Appsync Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon AppSync secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon AppSync
provider_slug: amazon-appsync
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsAuth
  parameter: Authorization
  sources:
  - openapi/amazon-appsync-openapi.yml
  type: apiKey
slug: amazon-appsync-authentication
source_filename: amazon-appsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-appsync-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-appsync-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/authentication/amazon-appsync-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
---
