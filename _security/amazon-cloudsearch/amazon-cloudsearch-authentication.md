---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloudsearch-domains-api-openapi.yml
  format: yaml
  label: Amazon CloudSearch Domains API
  slug: amazon-cloudsearch-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudsearch/openapi/amazon-cloudsearch-domains-api-openapi.yml
- filename: amazon-cloudsearch-index-fields-api-openapi.yml
  format: yaml
  label: Amazon CloudSearch Index Fields API
  slug: amazon-cloudsearch-index-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudsearch/openapi/amazon-cloudsearch-index-fields-api-openapi.yml
- filename: amazon-cloudsearch-operations-api-openapi.yml
  format: yaml
  label: Amazon CloudSearch Cloudsearch Operations API
  slug: amazon-cloudsearch-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudsearch/openapi/amazon-cloudsearch-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon CloudSearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudSearch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-cloudsearch-domains-api-openapi.yml
  - openapi/amazon-cloudsearch-index-fields-api-openapi.yml
  - openapi/amazon-cloudsearch-operations-api-openapi.yml
  type: apiKey
slug: amazon-cloudsearch-authentication
source_filename: amazon-cloudsearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-cloudsearch-domains-api-openapi.yml, openapi/amazon-cloudsearch-index-fields-api-openapi.yml,\n  openapi/amazon-cloudsearch-operations-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-cloudsearch-domains-api-openapi.yml\n  - openapi/amazon-cloudsearch-index-fields-api-openapi.yml\n  - openapi/amazon-cloudsearch-operations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloudsearch/authentication/amazon-cloudsearch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- CloudSearch
- Search
- Full-Text Search
- Managed
---
