---
anonymous_access: false
api_key_in: []
api_specs:
- filename: withreach-transaction-details-api-openapi.yml
  format: yaml
  label: Transaction Details API
  slug: transaction-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-transaction-details-api-openapi.yml
- filename: withreach-get-api-openapi.yml
  format: yaml
  label: Reach GET API
  slug: withreach-get-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-get-api-openapi.yml
- filename: withreach-order-api-openapi.yml
  format: yaml
  label: Reach Order API
  slug: withreach-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-order-api-openapi.yml
- filename: withreach-post-api-openapi.yml
  format: yaml
  label: Reach POST API
  slug: withreach-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-post-api-openapi.yml
- filename: withreach-quote-api-openapi.yml
  format: yaml
  label: Reach Quote API
  slug: withreach-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-quote-api-openapi.yml
- filename: withreach-session-api-openapi.yml
  format: yaml
  label: Reach Session API
  slug: withreach-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-session-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Withreach Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reach declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Reach
provider_slug: withreach
scheme_count: 1
schemes:
- description: HTTP Basic Authorization using API username and password supplied by Reach.
  format: Basic base64(username:password)
  header: Authorization
  scheme: basic
  type: http
slug: withreach-authentication
source_filename: withreach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.withreach.com/reference/authentication.md\nschemes:\n  - type: http\n    scheme: basic\n    description: HTTP Basic Authorization using API username and password supplied by Reach.\n    header: Authorization\n    format: Basic base64(username:password)"
source_yaml_url: https://artifacts.apis.io/withreach/authentication/withreach-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Tax
- Compliance
- E-commerce
- Merchant of Record
---
