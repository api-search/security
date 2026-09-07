---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cloudfront-cachepolicies-api-openapi.yml
  format: yaml
  label: CloudFront CachePolicies API
  slug: cloudfront-cachepolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-cachepolicies-api-openapi.yml
- filename: cloudfront-distributions-api-openapi.yml
  format: yaml
  label: CloudFront Distributions API
  slug: cloudfront-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-distributions-api-openapi.yml
- filename: cloudfront-functions-api-openapi.yml
  format: yaml
  label: CloudFront Functions API
  slug: cloudfront-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-functions-api-openapi.yml
- filename: cloudfront-invalidations-api-openapi.yml
  format: yaml
  label: CloudFront Invalidations API
  slug: cloudfront-invalidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-invalidations-api-openapi.yml
- filename: cloudfront-originaccesscontrol-api-openapi.yml
  format: yaml
  label: CloudFront OriginAccessControl API
  slug: cloudfront-originaccesscontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-originaccesscontrol-api-openapi.yml
- filename: cloudfront-publickeys-api-openapi.yml
  format: yaml
  label: CloudFront PublicKeys API
  slug: cloudfront-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-publickeys-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudfront Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudFront secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudFront
provider_slug: cloudfront
scheme_count: 1
schemes:
- description: 'AWS Signature Version 4. Signing service name is `cloudfront`,

    signing region is `us-east-1` regardless of the caller''s location —

    CloudFront is a global service. Authorization is supplied via

    `Authorization` and `X-Amz-Date` headers (and `X-Amz-Security-Token`

    when using temporary credentials).'
  in: header
  name: sigv4
  parameter: Authorization
  smithy_trait: aws.auth#sigv4
  sources:
  - openapi/_original/cloudfront-openapi.yml
  - smithy/cloudfront-2020-05-31.json
  type: apiKey
slug: cloudfront-authentication
source_filename: cloudfront-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/_original/cloudfront-openapi.yml + smithy/cloudfront-2020-05-31.json\ndocs: https://docs.aws.amazon.com/cloudfront/latest/APIReference/CommonParameters.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    CloudFront has NO OAuth and NO OpenID Connect surface — /.well-known/openid-configuration\n    and /.well-known/oauth-authorization-server returned 404 on all five probed hosts\n    (well-known/cloudfront-well-known.yml). Authorization is IAM policy evaluated\n    against a SigV4-signed request, so there is no scope vocabulary and scopes/ is\n    deliberately absent from this repo. The unit of permission is an IAM action\n    (cloudfront:CreateDistribution and 166 siblings), enumerated by AWS in the\n    machine-readable AWS Service Reference saved at\n    smithy/cloudfront-aws-service-reference.json.\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter:\
  \ Authorization\n  description: |-\n    AWS Signature Version 4. Signing service name is `cloudfront`,\n    signing region is `us-east-1` regardless of the caller's location —\n    CloudFront is a global service. Authorization is supplied via\n    `Authorization` and `X-Amz-Date` headers (and `X-Amz-Security-Token`\n    when using temporary credentials).\n  smithy_trait: aws.auth#sigv4\n  sources:\n  - openapi/_original/cloudfront-openapi.yml\n  - smithy/cloudfront-2020-05-31.json\ncredentials:\n  kinds:\n    - IAM user long-lived access key (access key id + secret access key)\n    - IAM role temporary credentials via STS (adds X-Amz-Security-Token)\n    - IAM Identity Center / SSO session credentials\n  rotation: Managed by IAM; AWS publishes no CloudFront-specific key lifetime.\nauthorization:\n  model: iam-policy\n  actions_reference: https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazoncloudfront.html\n  machine_readable_actions: smithy/cloudfront-aws-service-reference.json\n\
  \  managed_policies:\n    - CloudFrontFullAccess\n    - CloudFrontReadOnlyAccess\n  note: >-\n    The AWS Service Reference document (probed 200 at\n    https://servicereference.us-east-1.amazonaws.com/v1/cloudfront/cloudfront.json\n    on 2026-09-05) is the authoritative machine-readable list of CloudFront IAM\n    actions, the resources each acts on, and the condition keys available — the\n    closest thing CloudFront has to a published scope catalog.\nendpoints:\n  standard: https://cloudfront.amazonaws.com\n  dualstack: https://cloudfront.global.api.aws\n  fips: https://cloudfront-fips.global.api.aws\n  china: https://cloudfront.cn-northwest-1.amazonaws.com.cn\n"
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
