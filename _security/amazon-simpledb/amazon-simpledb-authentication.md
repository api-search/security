---
api_key_in:
- header
api_specs:
- filename: amazon-simpledb-action-batchdeleteattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=BatchDeleteAttributes API'
  slug: amazon-simpledb-action-batchdeleteattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-batchdeleteattributes-api-openapi.yml
- filename: amazon-simpledb-action-batchputattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=BatchPutAttributes API'
  slug: amazon-simpledb-action-batchputattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-batchputattributes-api-openapi.yml
- filename: amazon-simpledb-action-createdomain-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=CreateDomain API'
  slug: amazon-simpledb-action-createdomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-createdomain-api-openapi.yml
- filename: amazon-simpledb-action-deleteattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=DeleteAttributes API'
  slug: amazon-simpledb-action-deleteattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-deleteattributes-api-openapi.yml
- filename: amazon-simpledb-action-deletedomain-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=DeleteDomain API'
  slug: amazon-simpledb-action-deletedomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-deletedomain-api-openapi.yml
- filename: amazon-simpledb-action-domainmetadata-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=DomainMetadata API'
  slug: amazon-simpledb-action-domainmetadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-domainmetadata-api-openapi.yml
- filename: amazon-simpledb-action-getattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=GetAttributes API'
  slug: amazon-simpledb-action-getattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-getattributes-api-openapi.yml
- filename: amazon-simpledb-action-listdomains-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=ListDomains API'
  slug: amazon-simpledb-action-listdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-listdomains-api-openapi.yml
- filename: amazon-simpledb-action-putattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=PutAttributes API'
  slug: amazon-simpledb-action-putattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-putattributes-api-openapi.yml
- filename: amazon-simpledb-action-select-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=Select API'
  slug: amazon-simpledb-action-select-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-select-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Simpledb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SimpleDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
scheme_count: 1
schemes:
- description: Amazon Signature authorization v2
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-simpledb.yaml
  type: apiKey
slug: amazon-simpledb-authentication
source_filename: amazon-simpledb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-simpledb.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v2\n  sources:\n  - openapi/amazon-simpledb.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/authentication/amazon-simpledb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
---
