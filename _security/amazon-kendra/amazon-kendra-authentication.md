---
api_key_in:
- header
api_specs:
- filename: amazon-kendra-data-sources-api-openapi.yml
  format: yaml
  label: Amazon Kendra Data Sources API
  slug: amazon-kendra-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-data-sources-api-openapi.yml
- filename: amazon-kendra-documents-api-openapi.yml
  format: yaml
  label: Amazon Kendra Documents API
  slug: amazon-kendra-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-documents-api-openapi.yml
- filename: amazon-kendra-experience-api-openapi.yml
  format: yaml
  label: Amazon Kendra Experience API
  slug: amazon-kendra-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-experience-api-openapi.yml
- filename: amazon-kendra-faqs-api-openapi.yml
  format: yaml
  label: Amazon Kendra FAQs API
  slug: amazon-kendra-faqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-faqs-api-openapi.yml
- filename: amazon-kendra-indexes-api-openapi.yml
  format: yaml
  label: Amazon Kendra Indexes API
  slug: amazon-kendra-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-indexes-api-openapi.yml
- filename: amazon-kendra-queries-api-openapi.yml
  format: yaml
  label: Amazon Kendra Queries API
  slug: amazon-kendra-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-queries-api-openapi.yml
- filename: amazon-kendra-query-suggestions-api-openapi.yml
  format: yaml
  label: Amazon Kendra Query Suggestions API
  slug: amazon-kendra-query-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-query-suggestions-api-openapi.yml
- filename: amazon-kendra-thesaurus-api-openapi.yml
  format: yaml
  label: Amazon Kendra Thesaurus API
  slug: amazon-kendra-thesaurus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-thesaurus-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Kendra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Kendra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Kendra
provider_slug: amazon-kendra
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-kendra-openapi.yml
  type: apiKey
slug: amazon-kendra-authentication
source_filename: amazon-kendra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-kendra-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-kendra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/authentication/amazon-kendra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Enterprise Search
- Knowledge-Management
- Machine-Learning
- Natural Language
---
