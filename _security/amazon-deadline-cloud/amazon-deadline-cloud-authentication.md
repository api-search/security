---
api_key_in:
- header
api_specs:
- filename: amazon-deadline-cloud-farms-api-openapi.yml
  format: yaml
  label: Amazon Deadline Cloud Farms API
  slug: amazon-deadline-cloud-farms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/openapi/amazon-deadline-cloud-farms-api-openapi.yml
- filename: amazon-deadline-cloud-fleets-api-openapi.yml
  format: yaml
  label: Amazon Deadline Cloud Fleets API
  slug: amazon-deadline-cloud-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/openapi/amazon-deadline-cloud-fleets-api-openapi.yml
- filename: amazon-deadline-cloud-jobs-api-openapi.yml
  format: yaml
  label: Amazon Deadline Cloud Jobs API
  slug: amazon-deadline-cloud-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/openapi/amazon-deadline-cloud-jobs-api-openapi.yml
- filename: amazon-deadline-cloud-queues-api-openapi.yml
  format: yaml
  label: Amazon Deadline Cloud Queues API
  slug: amazon-deadline-cloud-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/openapi/amazon-deadline-cloud-queues-api-openapi.yml
- filename: amazon-deadline-cloud-workers-api-openapi.yml
  format: yaml
  label: Amazon Deadline Cloud Workers API
  slug: amazon-deadline-cloud-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/openapi/amazon-deadline-cloud-workers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Deadline Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Deadline Cloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-deadline-cloud-openapi.yml
  type: apiKey
slug: amazon-deadline-cloud-authentication
source_filename: amazon-deadline-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-deadline-cloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-deadline-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/authentication/amazon-deadline-cloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compute
- Media
- Rendering
- Visual Effects
---
