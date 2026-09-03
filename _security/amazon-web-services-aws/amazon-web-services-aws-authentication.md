---
api_key_in:
- header
- query
api_specs:
- filename: amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
  format: yaml
  label: Amazon Web Services (AWS) Amazon EC2 API API
  slug: amazon-web-services-aws-amazon-ec2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services-aws/refs/heads/main/openapi/amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
auth_types:
- apiKey
- custom-request-signing
description: ''
kind: authentication
layout: security
method: searched
name: Amazon Web Services Aws Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Web Services (AWS) secures its APIs with apiKey and custom-request-signing across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amazon Web Services (AWS)
provider_slug: amazon-web-services-aws
scheme_count: 3
schemes:
- algorithm: AWS4-HMAC-SHA256
  description: AWS Signature Version 4. The client derives a signing key from its secret access key, the date, the Region and the service, signs a canonical request, and sends "AWS4-HMAC-SHA256 Credential=<access-key>/<date>/<region>/<service>/aws4_request, SignedHeaders=..., Signature=..." on the Authorization header.
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
  type: apiKey
- description: The same signature carried in the query string instead of the header, using X-Amz-Algorithm, X-Amz-Credential, X-Amz-Date, X-Amz-SignedHeaders and X-Amz-Signature. This is the mechanism behind pre-signed URLs.
  in: query
  name: SigV4-QueryString
  parameter: X-Amz-Signature
  sources:
  - https://docs.aws.amazon.com/AWSEC2/latest/APIReference/CommonParameters.html
  type: apiKey
- description: Temporary credentials issued by AWS STS (AssumeRole, AssumeRoleWithWebIdentity, AssumeRoleWithSAML, GetSessionToken) are sent as a session token alongside the signed request. This is the recommended path for anything that is not a long-lived human credential, and the only path for instance/task/pod roles and OIDC federation from GitHub Actions or Kubernetes.
  docs: https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html
  in: header
  name: STS-TemporaryCredentials
  parameter: X-Amz-Security-Token
  type: apiKey
slug: amazon-web-services-aws-authentication
source_filename: amazon-web-services-aws-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: >-\n  https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_sigv.html and\n  https://docs.aws.amazon.com/AWSEC2/latest/APIReference/CommonParameters.html, reconciled with the\n  securitySchemes declared in openapi/amazon-web-services-aws-amazon-ec2-api-api-openapi.yml\ndocs: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_sigv.html\nsummary:\n  types:\n  - apiKey\n  - custom-request-signing\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  note: >-\n    AWS does not use bearer tokens, API keys or OAuth on its control plane. Every request is SIGNED with\n    AWS Signature Version 4 using an access key pair, and authorization is decided separately by IAM\n    policy evaluation. The OpenAPI models this as an apiKey scheme on the Authorization header because\n    OpenAPI has no vocabulary for request signing — the scheme name SigV4 carries the real meaning.\nschemes:\n- name: SigV4\n  type: apiKey\n \
  \ in: header\n  parameter: Authorization\n  description: >-\n    AWS Signature Version 4. The client derives a signing key from its secret access key, the date, the\n    Region and the service, signs a canonical request, and sends\n    \"AWS4-HMAC-SHA256 Credential=<access-key>/<date>/<region>/<service>/aws4_request,\n    SignedHeaders=..., Signature=...\" on the Authorization header.\n  algorithm: AWS4-HMAC-SHA256\n  sources:\n  - openapi/amazon-web-services-aws-amazon-ec2-api-api-openapi.yml\n- name: SigV4-QueryString\n  type: apiKey\n  in: query\n  parameter: X-Amz-Signature\n  description: >-\n    The same signature carried in the query string instead of the header, using X-Amz-Algorithm,\n    X-Amz-Credential, X-Amz-Date, X-Amz-SignedHeaders and X-Amz-Signature. This is the mechanism behind\n    pre-signed URLs.\n  sources:\n  - https://docs.aws.amazon.com/AWSEC2/latest/APIReference/CommonParameters.html\n- name: STS-TemporaryCredentials\n  type: apiKey\n  in: header\n  parameter:\
  \ X-Amz-Security-Token\n  description: >-\n    Temporary credentials issued by AWS STS (AssumeRole, AssumeRoleWithWebIdentity,\n    AssumeRoleWithSAML, GetSessionToken) are sent as a session token alongside the signed request. This\n    is the recommended path for anything that is not a long-lived human credential, and the only path\n    for instance/task/pod roles and OIDC federation from GitHub Actions or Kubernetes.\n  docs: https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html\nauthorization:\n  model: IAM policy evaluation\n  note: >-\n    Authentication proves who the caller is; every AWS API call is then authorized by evaluating\n    identity-based policies, resource-based policies, permission boundaries, Organizations service\n    control policies and session policies together. There is no OAuth scope surface — the equivalent of\n    a scope is an IAM Action such as ec2:RunInstances, and the full action vocabulary is published in\n    the IAM service authorization\
  \ reference.\n  action_reference: https://docs.aws.amazon.com/service-authorization/latest/reference/reference_policies_actions-resources-contextkeys.html\n  machine_readable_action_index: https://servicereference.us-east-1.amazonaws.com/\n  machine_readable_note: >-\n    AWS publishes a machine-readable service reference at servicereference.us-east-1.amazonaws.com\n    (HTTP 200 anonymously on 2026-09-01) listing every service and the Actions it supports — the closest\n    thing AWS has to a published scope catalogue.\noauth:\n  supported: false\n  note: >-\n    Amazon Cognito is an OAuth 2.0 / OIDC authorization server that AWS OPERATES FOR CUSTOMERS' OWN\n    applications. It does not authenticate calls to AWS APIs, so no scopes/ artifact is emitted for this\n    provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services-aws/refs/heads/main/authentication/amazon-web-services-aws-authentication.yml
summary_line: apiKey/custom-request-signing · 3 schemes
tags:
- Analytics
- Artificial Intelligence
- Cloud Computing
- Computing
- Containers
- Databases
- DevOps
- Infrastructure-as-a-Service
- Infrastructure
- Machine-Learning
- Networking
- Platform-as-a-Service
- Security
- Serverless
- Storage
---
