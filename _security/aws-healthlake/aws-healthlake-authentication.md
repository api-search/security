---
api_key_in:
- header
api_specs:
- filename: aws-healthlake-datastore-api-openapi.yml
  format: yaml
  label: AWS HealthLake Datastore API
  slug: aws-healthlake-datastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-healthlake/refs/heads/main/openapi/aws-healthlake-datastore-api-openapi.yml
- filename: aws-healthlake-export-api-openapi.yml
  format: yaml
  label: AWS HealthLake Export API
  slug: aws-healthlake-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-healthlake/refs/heads/main/openapi/aws-healthlake-export-api-openapi.yml
- filename: aws-healthlake-import-api-openapi.yml
  format: yaml
  label: AWS HealthLake Import API
  slug: aws-healthlake-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-healthlake/refs/heads/main/openapi/aws-healthlake-import-api-openapi.yml
- filename: aws-healthlake-tags-api-openapi.yml
  format: yaml
  label: AWS HealthLake Tags API
  slug: aws-healthlake-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-healthlake/refs/heads/main/openapi/aws-healthlake-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Healthlake Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS HealthLake secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS HealthLake
provider_slug: aws-healthlake
scheme_count: 1
schemes:
- description: 'AWS Signature Version 4. Sign requests with your AWS access key and secret key. See: https://docs.aws.amazon.com/general/latest/gr/signing_aws_api_requests.html'
  in: header
  name: aws_v4
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
slug: aws-healthlake-authentication
source_filename: aws-healthlake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'AWS Signature Version 4. Sign requests with your AWS access key and secret key.\n    See: https://docs.aws.amazon.com/general/latest/gr/signing_aws_api_requests.html'\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-healthlake/refs/heads/main/authentication/aws-healthlake-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- FHIR
- Health Data
- Clinical Data
- HIPAA
- Interoperability
- NLP
- Medical
- HL7
---
