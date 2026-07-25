---
api_key_in:
- header
api_specs:
- filename: amazon-ebs-amazon-ebs-amazon-elastic-block-store-ebs-api-api-openapi.yml
  format: yaml
  label: Amazon EBS Amazon EBS Amazon Elastic Block Store (EBS) API API
  slug: amazon-ebs-amazon-ebs-amazon-elastic-block-store-ebs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/openapi/amazon-ebs-amazon-ebs-amazon-elastic-block-store-ebs-api-api-openapi.yml
- filename: amazon-ebs-attachvolume-api-openapi.yml
  format: yaml
  label: 'Amazon EBS #AttachVolume API'
  slug: amazon-ebs-attachvolume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/openapi/amazon-ebs-attachvolume-api-openapi.yml
- filename: amazon-ebs-createsnapshot-api-openapi.yml
  format: yaml
  label: 'Amazon EBS #CreateSnapshot API'
  slug: amazon-ebs-createsnapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/openapi/amazon-ebs-createsnapshot-api-openapi.yml
- filename: amazon-ebs-deletevolume-api-openapi.yml
  format: yaml
  label: 'Amazon EBS #DeleteVolume API'
  slug: amazon-ebs-deletevolume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/openapi/amazon-ebs-deletevolume-api-openapi.yml
- filename: amazon-ebs-describesnapshots-api-openapi.yml
  format: yaml
  label: 'Amazon EBS #DescribeSnapshots API'
  slug: amazon-ebs-describesnapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/openapi/amazon-ebs-describesnapshots-api-openapi.yml
- filename: amazon-ebs-detachvolume-api-openapi.yml
  format: yaml
  label: 'Amazon EBS #DetachVolume API'
  slug: amazon-ebs-detachvolume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/openapi/amazon-ebs-detachvolume-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ebs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EBS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EBS
provider_slug: amazon-ebs
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-ebs-openapi.yml
  type: apiKey
slug: amazon-ebs-authentication
source_filename: amazon-ebs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ebs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-ebs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/authentication/amazon-ebs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Block Storage
- EBS
- EC2
- Snapshots
- Storage
- Volumes
---
