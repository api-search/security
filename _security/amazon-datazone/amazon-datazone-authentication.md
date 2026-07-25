---
api_key_in:
- header
api_specs:
- filename: amazon-datazone-assets-api-openapi.yml
  format: yaml
  label: Amazon DataZone Assets API
  slug: amazon-datazone-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-assets-api-openapi.yml
- filename: amazon-datazone-domains-api-openapi.yml
  format: yaml
  label: Amazon DataZone Domains API
  slug: amazon-datazone-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-domains-api-openapi.yml
- filename: amazon-datazone-environments-api-openapi.yml
  format: yaml
  label: Amazon DataZone Environments API
  slug: amazon-datazone-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-environments-api-openapi.yml
- filename: amazon-datazone-listings-api-openapi.yml
  format: yaml
  label: Amazon DataZone Listings API
  slug: amazon-datazone-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-listings-api-openapi.yml
- filename: amazon-datazone-projects-api-openapi.yml
  format: yaml
  label: Amazon DataZone Projects API
  slug: amazon-datazone-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-projects-api-openapi.yml
- filename: amazon-datazone-subscriptions-api-openapi.yml
  format: yaml
  label: Amazon DataZone Subscriptions API
  slug: amazon-datazone-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-subscriptions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Datazone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DataZone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DataZone
provider_slug: amazon-datazone
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-datazone-openapi.yml
  type: apiKey
slug: amazon-datazone-authentication
source_filename: amazon-datazone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-datazone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-datazone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/authentication/amazon-datazone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
---
