---
api_key_in:
- header
api_specs:
- filename: amazon-codeguru-profiler-internal-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler Internal API
  slug: amazon-codeguru-profiler-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-internal-api-openapi.yml
- filename: amazon-codeguru-profiler-profilinggroups-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler ProfilingGroups API
  slug: amazon-codeguru-profiler-profilinggroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-profilinggroups-api-openapi.yml
- filename: amazon-codeguru-profiler-profilinggroups-clienttoken-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler ProfilingGroups#clientToken API
  slug: amazon-codeguru-profiler-profilinggroups-clienttoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-profilinggroups-clienttoken-api-openapi.yml
- filename: amazon-codeguru-profiler-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Profiler Tags API
  slug: amazon-codeguru-profiler-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/openapi/amazon-codeguru-profiler-tags-api-openapi.yml
auth_types:
- apiKey
description: Authentication and authorization profile for Amazon CodeGuru Profiler. Every request is signed with AWS Signature Version 4 using IAM credentials — there is no API key, bearer token, OAuth flow or OIDC discovery document. Authorization is expressed as IAM actions on codeguru-profiler:*, plus an optional resource-based policy on each profiling group for cross-principal access.
kind: authentication
layout: security
method: searched
name: Amazon Codeguru Profiler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeGuru Profiler secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  note: 'Modelled as apiKey-in-header because that is the closest OpenAPI 3.x securityScheme to SigV4. It is NOT a static key: the Authorization header carries a per-request HMAC signature derived from an access key, secret key, optional session token, the request canonicalisation, the region and the date.'
  parameter: Authorization
  signing_name: codeguru-profiler
  sources:
  - openapi/amazon-codeguru-profiler-openapi-original.yaml
  type: apiKey
slug: amazon-codeguru-profiler-authentication
source_filename: amazon-codeguru-profiler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/security-iam-awsmanpol.html\nderived_from: openapi/amazon-codeguru-profiler-openapi-original.yaml\ndescription: >-\n  Authentication and authorization profile for Amazon CodeGuru Profiler. Every request is signed\n  with AWS Signature Version 4 using IAM credentials — there is no API key, bearer token, OAuth\n  flow or OIDC discovery document. Authorization is expressed as IAM actions on\n  codeguru-profiler:*, plus an optional resource-based policy on each profiling group for\n  cross-principal access.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: hmac\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: Amazon Signature authorization v4\n    signing_name: codeguru-profiler\n    sources:\n      - openapi/amazon-codeguru-profiler-openapi-original.yaml\n\
  \    note: >-\n      Modelled as apiKey-in-header because that is the closest OpenAPI 3.x securityScheme to\n      SigV4. It is NOT a static key: the Authorization header carries a per-request HMAC\n      signature derived from an access key, secret key, optional session token, the request\n      canonicalisation, the region and the date.\ncredential_sources:\n  - IAM user long-lived access keys\n  - IAM role temporary credentials (STS)\n  - IAM Identity Center / AWS SSO\n  - EC2 / ECS / Lambda instance and task roles\nauthorization:\n  model: iam-policy\n  service_prefix: codeguru-profiler\n  resource_arn_pattern: 'arn:aws:codeguru-profiler:{region}:{account}:profilingGroup/{name}'\n  managed_policies:\n    - name: AmazonCodeGuruProfilerFullAccess\n      description: >-\n        Provides full access to CodeGuru Profiler, including permissions to create, update, and\n        delete profiling groups.\n      actions:\n        - 'codeguru-profiler:*'\n        - 'codeguru:*'\n        - 'iam:ListRoles'\n\
  \        - 'iam:ListUsers'\n      resource: '*'\n    - name: AmazonCodeGuruProfilerReadOnlyAccess\n      description: >-\n        Grants read-only access to CodeGuru Profiler and related resources in other AWS services.\n      actions:\n        - 'codeguru-profiler:Get*'\n        - 'codeguru-profiler:Describe*'\n        - 'codeguru-profiler:List*'\n        - 'codeguru:*'\n        - 'iam:ListRoles'\n        - 'iam:ListUsers'\n      resource: '*'\n    - name: AmazonCodeGuruProfilerAgentAccess\n      description: >-\n        Added to the execution role of AWS Lambda functions onboarded to CodeGuru Profiler via\n        the Lambda console monitoring page. Allows the agent to create a profiling group, refresh\n        its configuration and submit agent profiles.\n      actions:\n        - 'codeguru-profiler:ConfigureAgent'\n        - 'codeguru-profiler:CreateProfilingGroup'\n        - 'codeguru-profiler:PostAgentProfile'\n      resource: 'arn:aws:codeguru-profiler:*:*:profilingGroup/*'\n  \
  \    least_privilege: true\n      note: >-\n        This is the policy an autonomous agent workload should be given. It is the only one of\n        the three scoped to a resource ARN rather than '*', and it grants exactly the three\n        operations a running profiler needs — no read of findings, no delete.\n  resource_based_policy:\n    supported: true\n    operations:\n      - PutPermission\n      - GetPolicy\n      - RemovePermission\n    concurrency: revisionId (optimistic lock; ConflictException 409 on a stale revision)\n    note: >-\n      A profiling group can carry its own resource policy granting an actionGroup to named\n      principals, which is how cross-account agent submission is enabled without sharing IAM\n      credentials.\ndiscovery:\n  openid_configuration: null\n  oauth_authorization_server: null\n  note: >-\n    Probed 2026-09-01 on codeguru-profiler.us-east-1.amazonaws.com (403 SigV4 front door),\n    docs.aws.amazon.com (404) and aws.amazon.com (301 -> 404). No\
  \ OAuth/OIDC discovery document\n    exists, which is expected for a SigV4 service.\n  see: well-known/amazon-codeguru-profiler-well-known.yml\ndocs:\n  - https://docs.aws.amazon.com/codeguru/latest/profiler-ug/security-iam-awsmanpol.html\n  - https://docs.aws.amazon.com/codeguru/latest/profiler-api/CommonParameters.html\n  - https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_PutPermission.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/authentication/amazon-codeguru-profiler-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine-Learning
---
