---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-nova-async-api-openapi.yml
  format: yaml
  label: Amazon Nova Async API
  slug: amazon-nova-async-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-nova/openapi/amazon-nova-async-api-openapi.yml
- filename: amazon-nova-inference-api-openapi.yml
  format: yaml
  label: Amazon Nova Inference API
  slug: amazon-nova-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-nova/openapi/amazon-nova-inference-api-openapi.yml
auth_types:
- aws-sigv4
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Amazon Nova Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Nova secures its APIs with aws-sigv4 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amazon Nova
provider_slug: amazon-nova
scheme_count: 2
schemes:
- description: AWS Signature Version 4. Every Bedrock Runtime request is signed with the caller's AWS access key id and secret, scoped by region and the `bedrock` signing name. Credentials resolve from IAM roles, instance/task metadata, SSO, or a static key pair; the AWS SDKs and CLI do the signing.
  in: header
  name: SigV4
  parameter: Authorization
  signing_name: bedrock
  smithy_trait: aws.auth#sigv4
  sources:
  - openapi/amazon-nova-openapi.yml
  - aws/api-models-aws bedrock-runtime 2023-09-30
  type: aws-sigv4
- description: Amazon Bedrock API key. A long- or short-term bearer token generated in the Amazon Bedrock console that authenticates a Nova call without SigV4 signing — the path most third-party OpenAI-style clients use. Declared in Amazon's service model as a first-class alternative to SigV4.
  in: header
  name: BedrockApiKey
  parameter: Authorization
  scheme: bearer
  smithy_trait: smithy.api#httpBearerAuth
  sources:
  - aws/api-models-aws bedrock-runtime 2023-09-30
  type: http
slug: amazon-nova-authentication
source_filename: amazon-nova-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: openapi/amazon-nova-openapi.yml\ndocs: https://docs.aws.amazon.com/bedrock/latest/userguide/api-setup.html\nauthoritative_contract: https://github.com/aws/api-models-aws/blob/main/models/bedrock-runtime/service/2023-09-30/bedrock-runtime-2023-09-30.json\nnote: 'Upgraded from derived to searched on 2026-09-01. The prior derivation read only our own OpenAPI\n  and recorded a single apiKey scheme named SigV4, which understates the contract in two ways: SigV4 is\n  a request-signing scheme rather than a static header key, and Amazon''s own Smithy model declares a\n  SECOND supported scheme — smithy.api#httpBearerAuth, the Amazon Bedrock API key — that our spec does\n  not carry at all.'\nsummary:\n  types:\n  - aws-sigv4\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\n  service_scoped_oauth: false\nschemes:\n- name: SigV4\n  type: aws-sigv4\n  in: header\n  parameter: Authorization\n  signing_name: bedrock\n  smithy_trait:\
  \ aws.auth#sigv4\n  description: AWS Signature Version 4. Every Bedrock Runtime request is signed with the caller's AWS\n    access key id and secret, scoped by region and the `bedrock` signing name. Credentials resolve from\n    IAM roles, instance/task metadata, SSO, or a static key pair; the AWS SDKs and CLI do the signing.\n  sources:\n  - openapi/amazon-nova-openapi.yml\n  - aws/api-models-aws bedrock-runtime 2023-09-30\n- name: BedrockApiKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  smithy_trait: smithy.api#httpBearerAuth\n  description: Amazon Bedrock API key. A long- or short-term bearer token generated in the Amazon Bedrock\n    console that authenticates a Nova call without SigV4 signing — the path most third-party OpenAI-style\n    clients use. Declared in Amazon's service model as a first-class alternative to SigV4.\n  sources:\n  - aws/api-models-aws bedrock-runtime 2023-09-30\nauthorization:\n  model: aws-iam\n  actions:\n  - bedrock:InvokeModel\n\
  \  - bedrock:InvokeModelWithResponseStream\n  - bedrock:Converse\n  - bedrock:ConverseStream\n  - bedrock:StartAsyncInvoke\n  - bedrock:GetAsyncInvoke\n  - bedrock:ListAsyncInvokes\n  resource_form: arn:aws:bedrock:<region>::foundation-model/amazon.nova-<variant>-v1:0\n  note: Access is IAM policy, not OAuth scopes. There is no scopes/ artifact for Amazon Nova because the\n    API declares no oauth2 security scheme — the only OAuth in this provider's orbit belongs to the AWS\n    MCP Server, recorded in mcp/ and conformance/.\n  additional_gate: Beyond IAM, an account must explicitly enable model access for each Nova model in the\n    Amazon Bedrock console before any credential can invoke it.\ndocs_additional:\n- https://docs.aws.amazon.com/nova/latest/userguide/getting-started-api.html\n"
source_yaml_url: https://artifacts.apis.io/amazon-nova/authentication/amazon-nova-authentication.yml
summary_line: aws-sigv4/http-bearer · 2 schemes
tags:
- Amazon Web Services
- Foundation Models
- Generative AI
- Image Generation
- Machine Learning
- Multi-Modal
- Speech
- Video Generation
---
