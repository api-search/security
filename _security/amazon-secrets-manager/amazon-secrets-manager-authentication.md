---
api_key_in: []
api_specs:
- filename: amazon-secrets-manager-openapi.yml
  format: yaml
  label: Amazon Secrets Manager API
  slug: amazon-secrets-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/openapi/amazon-secrets-manager-openapi.yml
auth_types:
- aws-sigv4
description: ''
kind: authentication
layout: security
method: searched
name: Amazon Secrets Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Secrets Manager secures its APIs with aws-sigv4 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
scheme_count: 1
schemes:
- description: Every request is signed with AWS Signature Version 4 using the caller's access key ID and secret access key (plus a session token for temporary credentials). The signature is carried in the Authorization header along with X-Amz-Date; the operation is selected via the X-Amz-Target header (e.g. secretsmanager.GetSecretValue).
  docs: https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html
  name: aws-sigv4
  region_scoped: true
  signing_name: secretsmanager
  type: sigv4
slug: amazon-secrets-manager-authentication
source_filename: amazon-secrets-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: >-\n  https://docs.aws.amazon.com/secretsmanager/latest/apireference/CommonParameters.html\n  and https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html — the\n  OpenAPI in this repo declares no securitySchemes (the AWS query protocol carries\n  auth in signed request headers rather than OpenAPI security objects), so this\n  profile is captured from the AWS documentation.\ndocs: https://docs.aws.amazon.com/secretsmanager/latest/userguide/auth-and-access.html\nsummary:\n  types: [aws-sigv4]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Amazon Secrets Manager uses AWS Signature Version 4 (SigV4) request signing,\n    not API keys or OAuth. Authorization is enforced by AWS IAM identity-based\n    policies and Secrets Manager resource-based (secret) policies. There is no\n    OAuth scope surface, so no scopes/ artifact is produced for this provider.\nschemes:\n  - name: aws-sigv4\n    type: sigv4\n    description:\
  \ >-\n      Every request is signed with AWS Signature Version 4 using the caller's\n      access key ID and secret access key (plus a session token for temporary\n      credentials). The signature is carried in the Authorization header along\n      with X-Amz-Date; the operation is selected via the X-Amz-Target header\n      (e.g. secretsmanager.GetSecretValue).\n    signing_name: secretsmanager\n    region_scoped: true\n    docs: https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html\nauthorization:\n  model: AWS IAM + resource-based policies\n  identity_based: >-\n    IAM identity-based policies grant secretsmanager:* actions (e.g.\n    secretsmanager:GetSecretValue, secretsmanager:CreateSecret) to users/roles.\n  resource_based: >-\n    Secret resource policies (PutResourcePolicy) enable cross-account and\n    fine-grained principal access to individual secrets.\n  kms: >-\n    Callers also need kms:Decrypt/kms:GenerateDataKey on the customer-managed KMS\n    key when\
  \ the secret is encrypted with a non-default key.\n  docs: https://docs.aws.amazon.com/secretsmanager/latest/userguide/auth-and-access.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/authentication/amazon-secrets-manager-authentication.yml
summary_line: aws-sigv4 · 1 scheme
tags:
- Configuration
- Credentials
- Rotation
- Secrets
- Security
---
