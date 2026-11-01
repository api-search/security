---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-opensearch-domain-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Domain API
  slug: amazon-opensearch-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-domain-api-openapi.yml
- filename: amazon-opensearch-es-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Es API
  slug: amazon-opensearch-es-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-es-api-openapi.yml
- filename: amazon-opensearch-packages-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Packages API
  slug: amazon-opensearch-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-packages-api-openapi.yml
- filename: amazon-opensearch-tags-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Tags API
  slug: amazon-opensearch-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-tags-api-openapi.yml
- filename: amazon-opensearch-tags-removal-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Tags Removal API
  slug: amazon-opensearch-tags-removal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-tags-removal-api-openapi.yml
- filename: amazon-opensearch-capability-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Opensearch Capability API
  slug: amazon-opensearch-capability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-capability-api-openapi.yml
- filename: amazon-opensearch-config-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Opensearch Config API
  slug: amazon-opensearch-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-config-api-openapi.yml
- filename: amazon-opensearch-datasource-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Opensearch Datasource API
  slug: amazon-opensearch-datasource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-datasource-api-openapi.yml
- filename: amazon-opensearch-index-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Opensearch Index API
  slug: amazon-opensearch-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-index-api-openapi.yml
- filename: amazon-opensearch-opensearch-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Opensearch Opensearch API
  slug: amazon-opensearch-opensearch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-opensearch-api-openapi.yml
- filename: amazon-opensearch-operations-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Opensearch Operations API
  slug: amazon-opensearch-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-opensearch/openapi/amazon-opensearch-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Opensearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon OpenSearch Service API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-opensearch-openapi.yml
  type: apiKey
slug: amazon-opensearch-authentication
source_filename: amazon-opensearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-opensearch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-opensearch-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-opensearch/authentication/amazon-opensearch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Elasticsearch
- Search
---
