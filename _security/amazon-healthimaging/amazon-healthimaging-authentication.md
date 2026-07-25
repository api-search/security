---
api_key_in:
- header
api_specs:
- filename: amazon-healthimaging-datastore-api-openapi.yml
  format: yaml
  label: Amazon HealthImaging Datastore API
  slug: amazon-healthimaging-datastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/openapi/amazon-healthimaging-datastore-api-openapi.yml
- filename: amazon-healthimaging-getdicomimportjob-api-openapi.yml
  format: yaml
  label: Amazon HealthImaging GetDICOMImportJob API
  slug: amazon-healthimaging-getdicomimportjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/openapi/amazon-healthimaging-getdicomimportjob-api-openapi.yml
- filename: amazon-healthimaging-listdicomimportjobs-api-openapi.yml
  format: yaml
  label: Amazon HealthImaging ListDICOMImportJobs API
  slug: amazon-healthimaging-listdicomimportjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/openapi/amazon-healthimaging-listdicomimportjobs-api-openapi.yml
- filename: amazon-healthimaging-startdicomimportjob-api-openapi.yml
  format: yaml
  label: Amazon HealthImaging StartDICOMImportJob API
  slug: amazon-healthimaging-startdicomimportjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/openapi/amazon-healthimaging-startdicomimportjob-api-openapi.yml
- filename: amazon-healthimaging-tags-api-openapi.yml
  format: yaml
  label: Amazon HealthImaging Tags API
  slug: amazon-healthimaging-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/openapi/amazon-healthimaging-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Healthimaging Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon HealthImaging secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-healthimaging-openapi.yaml
  type: apiKey
slug: amazon-healthimaging-authentication
source_filename: amazon-healthimaging-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-healthimaging-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-healthimaging-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/authentication/amazon-healthimaging-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
---
