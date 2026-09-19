---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-healthomics-import-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Import API
  slug: amazon-healthomics-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-import-api-openapi.yml
- filename: amazon-healthomics-referencestore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Referencestore API
  slug: amazon-healthomics-referencestore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-referencestore-api-openapi.yml
- filename: amazon-healthomics-referencestores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Referencestores API
  slug: amazon-healthomics-referencestores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-referencestores-api-openapi.yml
- filename: amazon-healthomics-run-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Run API
  slug: amazon-healthomics-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-run-api-openapi.yml
- filename: amazon-healthomics-sequencestore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Sequencestore API
  slug: amazon-healthomics-sequencestore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-sequencestore-api-openapi.yml
- filename: amazon-healthomics-sequencestores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Sequencestores API
  slug: amazon-healthomics-sequencestores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-sequencestores-api-openapi.yml
- filename: amazon-healthomics-tags-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Tags API
  slug: amazon-healthomics-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-tags-api-openapi.yml
- filename: amazon-healthomics-workflow-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Workflow API
  slug: amazon-healthomics-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-workflow-api-openapi.yml
- filename: amazon-healthomics-annotation-store-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Annotation Store API
  slug: amazon-healthomics-annotation-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-annotation-store-api-openapi.yml
- filename: amazon-healthomics-annotation-stores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Annotation Stores API
  slug: amazon-healthomics-annotation-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-annotation-stores-api-openapi.yml
- filename: amazon-healthomics-run-group-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Run Group API
  slug: amazon-healthomics-run-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-run-group-api-openapi.yml
- filename: amazon-healthomics-variant-store-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Variant Store API
  slug: amazon-healthomics-variant-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-variant-store-api-openapi.yml
- filename: amazon-healthomics-variant-stores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Variant Stores API
  slug: amazon-healthomics-variant-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-variant-stores-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Healthomics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon HealthOmics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-healthomics-openapi.yaml
  type: apiKey
slug: amazon-healthomics-authentication
source_filename: amazon-healthomics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-healthomics-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-healthomics-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/authentication/amazon-healthomics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
---
