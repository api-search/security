---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-lex-models-v2-openapi.yml
  format: yaml
  label: Amazon Lex Bots API
  slug: amazon-lex-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-models-v2-openapi.yml
- filename: amazon-lex-runtime-v2-openapi.yml
  format: yaml
  label: Amazon Lex Runtime V2 API
  slug: amazon-lex-runtime-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-runtime-v2-openapi.yml
auth_types:
- sigv4
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Amazon Lex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Lex secures its APIs with sigv4 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Lex
provider_slug: amazon-lex
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries the credential scope, signed headers and signature; x-amz-date is required alongside it. Temporary credentials add x-amz-security-token.
  in: header
  name: sigv4
  parameter: Authorization
  signing_name: lex
  signing_region: the calling AWS Region
  sources:
  - smithy/amazon-lex-models-v2-2020-08-07.json
  - openapi/amazon-lex-models-v2-openapi.yml
  - openapi/amazon-lex-runtime-v2-openapi.yml
  spec: https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html
  type: apiKey
slug: amazon-lex-authentication
source_filename: amazon-lex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://docs.aws.amazon.com/lexv2/latest/dg/security_iam_service-with-iam.html,\n  https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html,\n  https://servicereference.us-east-1.amazonaws.com/v1/lex/lex.json (AWS Service Reference, fetched\n  2026-09-17) — cross-checked against the aws.auth#sigv4 trait in\n  smithy/amazon-lex-models-v2-2020-08-07.json and derived from\n  openapi/amazon-lex-models-v2-openapi.yml + openapi/amazon-lex-runtime-v2-openapi.yml\nprovider: Amazon Lex\nproviderId: amazon-lex\nsummary:\n  types:\n  - sigv4\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  api_keys: false\n  mutual_tls: false\nmodel: >-\n  AWS Signature Version 4 over IAM credentials. There are no API keys, no OAuth flow, no bearer tokens\n  and no OIDC discovery document — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server 404 on every host probed. The OpenAPI securityScheme\
  \ is\n  typed apiKey/header only because OpenAPI has no native SigV4 type; the real mechanism is a signed\n  canonical request, and a caller cannot construct one from a static header value.\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  signing_name: lex\n  signing_region: the calling AWS Region\n  description: >-\n    AWS Signature Version 4. The Authorization header carries the credential scope, signed headers and\n    signature; x-amz-date is required alongside it. Temporary credentials add x-amz-security-token.\n  spec: https://docs.aws.amazon.com/general/latest/gr/signature-version-4.html\n  sources:\n  - smithy/amazon-lex-models-v2-2020-08-07.json\n  - openapi/amazon-lex-models-v2-openapi.yml\n  - openapi/amazon-lex-runtime-v2-openapi.yml\nauthorization:\n  model: IAM identity-based policy plus optional resource-based policy\n  actions_reference: https://servicereference.us-east-1.amazonaws.com/v1/lex/lex.json\n  action_count: 152\n  action_breakdown:\n\
  \    write: 75\n    list: 39\n    tagging_only: 2\n    permission_management: 0\n  resource_types: [bot, bot alias, bot version, channel, intent version, slottype version, test set]\n  note: >-\n    Worth calling out as a discoverability fact: AWS publishes the full permission surface\n    machine-readably and anonymously. The Service Reference document gives all 152 `lex:*` actions with\n    per-action write/list/tagging annotations and the resource types each one touches — an agent can\n    compute the exact least-privilege policy for a planned call sequence without reading a docs page.\n  managed_policies:\n  - name: AmazonLexFullAccess\n  - name: AmazonLexReadOnly\n  - name: AmazonLexRunBotsOnly\n  - name: AmazonLexReplicationPolicy\n  managed_policies_docs: https://docs.aws.amazon.com/lexv2/latest/dg/security-iam-awsmanpol.html\n  resource_based:\n    supported: true\n    operations: [CreateResourcePolicy, DescribeResourcePolicy, UpdateResourcePolicy, DeleteResourcePolicy, CreateResourcePolicyStatement,\
  \ DeleteResourcePolicyStatement]\n    note: Attachable to a bot or bot alias, for cross-account invocation.\n  service_role:\n    required: true\n    note: >-\n      CreateBot requires a roleArn — the IAM role Amazon Lex itself assumes to write conversation logs,\n      call Lambda code hooks and read S3 grammar files. This is a second, distinct identity from the\n      caller's, and a misconfigured one surfaces at runtime as DependencyFailedException (424), not as\n      an auth error at build time.\ndocs: https://docs.aws.amazon.com/lexv2/latest/dg/security_iam_service-with-iam.html\nscopes_artifact: null\nscopes_note: No OAuth scopes exist. Authorization granularity is the 152 IAM actions above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/authentication/amazon-lex-authentication.yml
summary_line: sigv4 · 1 scheme
tags:
- Artificial Intelligence
- Conversational AI
- Chatbots
- Natural Language Processing
- Speech
- Voice
- Contact Center
- Customer Service
---
