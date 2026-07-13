---
api_key_in:
- header
api_specs:
- filename: cloudfront-openapi.yml
  format: yaml
  label: AWS CloudFront API (canonical)
  slug: canonical
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudfront Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudFront secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudFront
provider_slug: cloudfront
scheme_count: 1
schemes:
- description: 'AWS Signature Version 4. Signing service name is `cloudfront`,

    signing region is `us-east-1`. Authorization is supplied via

    `Authorization` and `X-Amz-Date` headers (and `X-Amz-Security-Token`

    when using temporary credentials).'
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/cloudfront-openapi.yml
  type: apiKey
slug: cloudfront-authentication
source_filename: cloudfront-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudfront-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    AWS Signature Version 4. Signing service name is `cloudfront`,\n    signing region is `us-east-1`. Authorization is supplied via\n    `Authorization` and `X-Amz-Date` headers (and `X-Amz-Security-Token`\n    when using temporary credentials).\n  sources:\n  - openapi/cloudfront-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/authentication/cloudfront-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alias
- CDN
- Caching
- Content Delivery
- Edge Computing
- Lambda@Edge
- Network
---
