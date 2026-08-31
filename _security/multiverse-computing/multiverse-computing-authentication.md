---
api_key_in: []
api_specs:
- filename: multiverse-computing-audio-api-openapi.yml
  format: yaml
  label: Multiverse Computing Audio API
  slug: multiverse-computing-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/openapi/multiverse-computing-audio-api-openapi.yml
- filename: multiverse-computing-batches-api-openapi.yml
  format: yaml
  label: Multiverse Computing Batches API
  slug: multiverse-computing-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/openapi/multiverse-computing-batches-api-openapi.yml
- filename: multiverse-computing-completions-api-openapi.yml
  format: yaml
  label: Multiverse Computing Completions API
  slug: multiverse-computing-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/openapi/multiverse-computing-completions-api-openapi.yml
- filename: multiverse-computing-files-api-openapi.yml
  format: yaml
  label: Multiverse Computing Files API
  slug: multiverse-computing-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/openapi/multiverse-computing-files-api-openapi.yml
- filename: multiverse-computing-model-info-api-openapi.yml
  format: yaml
  label: Multiverse Computing Model info API
  slug: multiverse-computing-model-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/openapi/multiverse-computing-model-info-api-openapi.yml
- filename: multiverse-computing-responses-api-openapi.yml
  format: yaml
  label: Multiverse Computing Responses API
  slug: multiverse-computing-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/openapi/multiverse-computing-responses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Multiverse Computing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Multiverse Computing secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Multiverse Computing
provider_slug: multiverse-computing
scheme_count: 1
schemes:
- applied_to: all operations
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  in: header
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/multiverse-computing-compactifai-openapi.yml
  - https://docs.compactif.ai/authentication/
  type: http
slug: multiverse-computing-authentication
source_filename: multiverse-computing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.compactif.ai/authentication/\ndocs: https://docs.compactif.ai/authentication/\nsummary:\n  types:\n  - http\n  model: Single Bearer API key per account, issued from the CompactifAI Dashboard\n    (or via AWS Marketplace subscription through Multiverse IAM). No OAuth, no scopes,\n    no per-endpoint differentiation.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  applied_to: all operations\n  sources:\n  - openapi/multiverse-computing-compactifai-openapi.yml\n  - https://docs.compactif.ai/authentication/\nkey_issuance:\n  paths:\n  - name: Dashboard signup\n    url: https://auth.multiverseapp.ai/sign-up?redirect_url=https%3A%2F%2Fdashboard.compactif.ai%2F\n    steps:\n    - Create an account at dashboard.compactif.ai with an email address\n    - Add billing details and accept billing terms\n    - Add a payment\
  \ method\n    - Copy the API key from the Manage API Keys tab\n    note: No AWS account required.\n  - name: AWS Marketplace subscription\n    url: https://aws.amazon.com/marketplace/pp/prodview-ce2dp5ibd7lli\n    steps:\n    - Subscribe on the AWS Marketplace listing (pay-as-you-go plan only)\n    - Complete the \"Set up your account\" registration form\n    - Await manual approval (documented as typically within 24 hours)\n    - Sign in to dashboard.compactif.ai via Multiverse IAM with an emailed one-time\n      passcode (OTP)\n    note: Approval is manual, so key issuance on this path is not self-service.\nkey_policy:\n  tokens_per_account: 1\n  rotation: Self-service \"Rotate key\" in the Dashboard Manage API Keys tab\n  multi_user: Not supported per account; teammates must sign up separately or contact\n    support\n  compromise_procedure: Report through the technical support form (https://docs.compactif.ai/support-contact/)\n  source: https://docs.compactif.ai/authentication/\nerrors:\n\
  \  '401': authentication_error — no Bearer token supplied, malformed token, or the\n    token is not associated with a valid user\n  source: https://docs.compactif.ai/error-handling/\nnotes:\n- The OpenAPI document declares components.securitySchemes.HTTPBearer but sets no\n  top-level `security` requirement and no per-operation `security`, so the spec alone\n  does not show that auth is mandatory; the docs and a live 401 from GET\n  https://api.compactif.ai/v1/models both confirm it is.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multiverse-computing/refs/heads/main/authentication/multiverse-computing-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine Learning
- LLM Inference
- Model Compression
- Quantum Computing
- Speech to Text
- OpenAI Compatible
- Developer Tools
- Spain
- Company
---
