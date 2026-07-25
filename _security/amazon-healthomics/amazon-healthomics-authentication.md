---
api_key_in:
- header
api_specs:
- filename: amazon-healthomics-annotationstore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics AnnotationStore API
  slug: amazon-healthomics-annotationstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-annotationstore-api-openapi.yml
- filename: amazon-healthomics-annotationstores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics AnnotationStores API
  slug: amazon-healthomics-annotationstores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-annotationstores-api-openapi.yml
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
- filename: amazon-healthomics-rungroup-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics RunGroup API
  slug: amazon-healthomics-rungroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-rungroup-api-openapi.yml
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
- filename: amazon-healthomics-variantstore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics VariantStore API
  slug: amazon-healthomics-variantstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-variantstore-api-openapi.yml
- filename: amazon-healthomics-variantstores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics VariantStores API
  slug: amazon-healthomics-variantstores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-variantstores-api-openapi.yml
- filename: amazon-healthomics-workflow-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Workflow API
  slug: amazon-healthomics-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-workflow-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
